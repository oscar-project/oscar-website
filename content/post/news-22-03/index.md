---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "OSCAR News: March 2022"
subtitle: ""
summary: "New corpus, new paper and new tools."
authors: ["julien", "pedro"]
tags: []
categories: ["news"]
date: 2022-03-10T15:45:55+02:00
lastmod: 2022-03-10T15:45:55+02:00
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

The last release of the OSCAR Corpus dates back to September, 2021. 
Since then, we worked on producing a new pipeline, containing many changes.


{{% toc %}}

## New corpus 

{{% callout note %}}
The new OSCAR Corpus 22.01 is available [here](oscar-v22-01).
{{% /callout %}}
The new OSCAR Corpus exhibit several changes compared to the previous ones: it is not backward compatible, is document-oriented and contains more metadata.

Also, documents identified as `<lang>` are *not* guaranteed to hold only sentences identified as `<lang>`, as we use an internal language content threshold. 
### Format details

The corpus was first stored in plaintext files, with a double newline separating sentences from different documents. The 21.09 corpus introducted metadata that we stored in a separate file, using [JSONLines](https://jsonlines.org/).

The latest corpus is directly distributed via JSONLines files, merging documents and its metadata together.

```json
{
  "content":"newline\nseparaaaaaaaaaaated\ncontent", //content itself
  // Headers from the crawler
  // Note that nothing is changed, so the content length may be incorrect.
  "warc_headers":{ 
    "warc-refers-to":"<urn:uuid:83f2e1d4-5ed3-41db-86ff-f7826c4c20f9>",
    "warc-date":"2021-09-16T11:07:14Z",
    "warc-block-digest":"sha1:X3OWP47FG2O5LBNMFSNB44FJF2SSRC26",
    "warc-type":"conversion",
    "warc-identified-content-language":"eng",
    "content-length":"1694",
    "warc-target-uri":"https://foo.bar",
    "warc-record-id":"<urn:uuid:3304bc27-17d0-4ffd-a692-340381478a5f>",
    "content-type":"text/plain"
  },
  "metadata":{
    // Document-wide identification.
    // The "prob" is the weighted average of the identified lines.
    "identification":{
      "label":"en",
      "prob":0.6268374
    },

    // Annotations. Can be null if no annotations have been added.
    "annotation":[
      "short_sentences",
      "footer"
    ],

    // Line-by-line identifications
    // Can have null values for lines that did not get an identification.
    "sentence_identifications":[
      {
        "label":"en",
        "prob":0.93925816
      },
      null,
      {
        "label":"en",
        "prob":0.9606543
      }
    ]
  }
}
```

The drawback is that using the corpus now requires a bit more tooling/coding, to extract the information you are interested in.

### Feature highlight: Annotations

TODO

## Tools

TODO

### `oscar-tools`

TODO

### Deduplication?

TODO explain no dedup, tools will be provided

### What do you need?

TODO

## Paper