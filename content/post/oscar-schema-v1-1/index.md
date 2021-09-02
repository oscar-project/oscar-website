---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Oscar Schema v1.1"
subtitle: "The new OSCAR Schema brings metadata while staying backward compatible."
summary: "The new OSCAR Schema brings metadata while staying backward compatible."
authors: []
tags: []
categories: ["schema", "update"]
date: 2021-09-02T15:02:03+02:00
lastmod: 2021-09-02T15:02:03+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
# OSCAR Schema v1.1.0

[OSCAR][oscar] (Open Super-large Crawled Aggregated coRpus) is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus using the goclassy architecture.

The new OSCAR schema incorporates backward-compatible changes.

## Changes

The old OSCAR Schema v1.0 featured the following file hierarchy, in an uncompressed form:

```sh
/
├── af
│   ├── af_sha256.txt
│   └── af.txt.gz
├── de
│   ├── de_sha256.txt    # Checksum file 
│   └── de.txt.gz        # Textual content
├── en
│   ├── en_part_1.txt.gz        # Multipart example
│   ├── en_part_2.txt.gz
│   └── en_sha256.txt
├── yi
│   ├── yi_sha256.txt
│   └── yi.txt.gz
└── zh
    ├── zh_sha256.txt
    └── zh.txt.gz
```

The new OSCAR Schema v1.1 features the following file hierarchy (some languages omitted):

```sh
/
├── af
│   ├── af_meta.jsonl.gz
│   ├── af_sha256.txt
│   └── af.txt.gz
├── de
│   ├── de_meta.jsonl.gz # Metadata, in JSONLines format
│   ├── de_sha256.txt    # Checksum file 
│   └── de.txt.gz        # Textual content
├── en
│   ├── en_meta_part_1.jsonl.gz # Multipart example
│   ├── en_meta_part_2.jsonl.gz # Each part is independent,
│   ├── en_part_1.txt.gz        # Ex: en_part_2.txt.gz and en_meta_part_2.jsonl.gz
│   ├── en_part_2.txt.gz
│   └── en_sha256.txt
├── yi
│   ├── yi_meta.jsonl.gz
│   ├── yi_sha256.txt
│   └── yi.txt.gz
└── zh
    ├── zh_meta.jsonl.gz
    ├── zh_sha256.txt
    └── zh.txt.gz
```

## File formats

### `.txt` files

Lines are newline-separated, and documents are double-newline separated. 
In other terms, there is a blank line between each document.

### `.jsonl` files

These are the metadata, in [JSONLines](https://jsonlines.org/) format.

Each line follows the following JSON Scheme:

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "Metadata",
  "description": "Holds record headers.\n\nEach metadata is linked to a specific paragraph/text zone",
  "type": "object",
  "required": [
    "headers",
    "nb_sentences",
    "offset"
  ],
  "properties": {
    "headers": {
      "type": "object",
      "additionalProperties": {
        "type": "string"
      }
    },
    "nb_sentences": {
      "type": "integer",
      "format": "uint",
      "minimum": 0.0
    },
    "offset": {
      "type": "integer",
      "format": "uint",
      "minimum": 0.0
    }
  }
}
```

Example:
```js
{
   "headers":{                  // these headers keys are *almost* always present.
      "content-length":"11062", // the content length is not changed and reflects the 
                                // length before filtering and eventual deduplication.
      "warc-target-uri":"...",
      "warc-type":"conversion",
      "content-type":"text/plain",
      "warc-date":"2021-02-24T17:55:29Z", // Following WARC specification, it is the crawl date.
      "warc-identified-content-language":"eng,zho",
      "warc-refers-to":"<urn:uuid:c649de0e-42a3-4e69-b675-98e28e084698>",
      "warc-block-digest":"sha1:V4PYYGYA6ZYA2WACDKSNL6NXGDN6XK6X",
      "warc-record-id":"<urn:uuid:121a822f-5362-4559-8891-d085415cdd90>"
   },
   "offset":0, // Related text is in the text file, from lines offset+1 to lines offset+nb_sentences.
   "nb_sentences":9
}
```

### `<lang>_sha256.txt` files

These are used to check for eventual corruption during download.
They can be used by running `sha256sum -c <lang>_sha256.txt`.


[oscar]: https://oscar-corpus.com