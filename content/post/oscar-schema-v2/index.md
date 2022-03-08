---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "OSCAR Schema v2"
subtitle: "A new, document oriented corpus layout with more metadata."
summary: "A new, document oriented corpus layout with more metadata."
authors: ["julien"]
tags: []
categories: ["schema", "update"]
date: 2022-01-01T15:02:03+02:00
lastmod: 2022-01-01T15:02:03+02:00
featured: false
draft: true

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
# OSCAR Schema v2

[OSCAR][oscar] (Open Super-large Crawled Aggregated coRpus) is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus using the goclassy architecture.

The new OSCAR schema is a major, breaking change from the previous ones, adding more metadata and laying out documents rather than lines.


## Changes

OSCAR Schema v2 groups text and metadata in JSON dictionnaries, in [JSONLines](https://jsonlines.org/) format.

```sh
/
├── af
│   ├── af_sha256.txt
│   └── af.jsonl.gz
├── de
│   ├── de_sha256.txt    # Checksum file 
│   └── de.jsonl.gz        # Textual content
├── en
│   ├── en_part_1.jsonl.gz        # Multipart example
│   ├── en_part_2.jsonl.gz
│   └── en_sha256.txt
├── yi
│   ├── yi_sha256.txt
│   └── yi.jsonl.gz
└── zh
    ├── zh_sha256.txt
    └── zh.jsonl.gz
```

## File formats

### `.jsonl` files

These are the metadata, in [JSONLines](https://jsonlines.org/) format.

Each line follows the following JSON Scheme:

```json
{
  "$schema": "http://json-schema.org/draft-07/schema#",
  "title": "Document",
  "description": "Serializable version of [Document].",
  "type": "object",
  "required": [
    "content",
    "metadata",
    "warc_headers"
  ],
  "properties": {
    "content": {
      "type": "string"
    },
    "metadata": {
      "$ref": "#/definitions/Metadata"
    },
    "warc_headers": {
      "type": "object",
      "additionalProperties": {
        "type": "string"
      }
    }
  },
  "definitions": {
    "Identification": {
      "type": "object",
      "required": [
        "label",
        "prob"
      ],
      "properties": {
        "label": {
          "$ref": "#/definitions/Lang"
        },
        "prob": {
          "type": "number",
          "format": "float"
        }
      }
    },
    "Lang": {
      "type": "string",
      "enum": [
        "Af",
        "Als",
        "...",
        "Yue",
        "Zh",
        "Multi"
      ]
    },
    "Metadata": {
      "description": "OSCAR-specific metadata",
      "type": "object",
      "required": [
        "identification",
        "sentence_identifications"
      ],
      "properties": {
        "annotation": {
          "type": [
            "array",
            "null"
          ],
          "items": {
            "type": "string"
          }
        },
        "identification": {
          "$ref": "#/definitions/Identification"
        },
        "sentence_identifications": {
          "type": "array",
          "items": {
            "anyOf": [
              {
                "$ref": "#/definitions/Identification"
              },
              {
                "type": "null"
              }
            ]
          }
        }
      }
    }
  }
}
```

Example:
```js
{

  // text is here, separated by \n characters that have been removed here for lisibility
  "content": "Adopt-a-user Home • Talk || Adoptee's Area • Resources || Adopter's Area • Resources • List of Adopters || Teahouse || Live Help Chat (IRC)\n
  Shortcuts\n
  WP:AAU\n
  WP:ADOPT\n
  WP:ADOPTION\n
  WP:WIKIADOPT\n
  The Adopt-a-user program is designed to help new and inexperienced users by pairing them with more experienced Wikipedians. These editors (referred to as adopters or mentors) will \"adopt\" newer users, guiding them along the way as they learn about Wikipedia and its various aspects.\n
  The project aims to inform new users about the ins and outs of Wikipedia and steer them away from making less-than-constructive edits or misplaced test edits. Well over a thousand users have been involved in the program at one time or another.\n
  So, if you're new or inexperienced and would like to:\nAsk questions about editing, contributing to Wikipedia and creating your first article\n
  Learn to navigate processes and policies and guidelines\n
  Get help with article creation or image uploads or any other activities on Wikipedia\n
  . . .then an adopter should be able to help you. Adoption lasts as long as the adopter and adoptee want to continue, so you can stop any time if you feel you've learned enough, or you'd like to take a break.\n
  If you are looking to contribute to Wikipedia but do not intend to remain as an active user well after adoption, then this program is not for you. Adoption is for users who intend to be long-term contributors and members of the community, so if you are simply here to create one article, see this page for help and do not request adoption.\n
  Users who don't want adopting – but who do need help with one-off problems – might like to consider whether the Teahouse question forum, the Help desk, or a {{Help me}} request might be better ways to get quick answers.\n
  Participation\n
  Being adopted is easy and fun. Why not select an adopter from the list of adopters and contact them directly to request adoption? If you choose an adopter who shares your interests, they will be more able to assist you while you learn under their tutelage.\n
  View the list of adopters!\n
  ...",

  // WARC Headers are extracted and put there untouched.
  // The content-length shoud not be understood as the current document length, but as the original document length.
  "warc_headers": {
    "warc-block-digest": "sha1:U2OJPXXE3JCPSLAB6UPB3TEGBDHKPTAO",
    "warc-record-id": "<urn:uuid:fec8808f-96ef-4ae5-8a57-df5b44e42dcf>",
    "warc-identified-content-language": "eng,nno",
    "content-type": "text/plain",
    "warc-refers-to": "<urn:uuid:2f59440d-3700-418c-aa94-5c63bab316c3>",
    "warc-date": "2021-09-16T12:40:45Z",
    "warc-target-uri": "https://en.wikipedia.org/wiki/Wikipedia:Adopt-a-user",
    "content-length": "5385",
    "warc-type": "conversion"
  },

  // OSCAR metadata
  "metadata": {

    // Document identification
    "identification": {
      "label": "en",
      "prob": 0.6775619
    },

    // Annotations of the document
    "annotation": [
      "short_sentences",
      "header",
      "footer"
    ],

    // Sentence identifications.
    // null: identification confidence too low (<0.8)
    // There is exactly one identification per line.
    "sentence_identifications": [
      null,
      null,
      {
        "label": "en",
        "prob": 0.89475197
      },
      {
        "label": "en",
        "prob": 0.9124037
      },
      {
        "label": "en",
        "prob": 0.8080786
      },
      null,
      {
        "label": "en",
        "prob": 0.9665413
      }, 
    ]
  }
}
```

### `<lang>_sha256.txt` files

These are used to check for eventual corruption during download.
They can be used by running `sha256sum -c <lang>_sha256.txt`.

[oscar]: https://oscar-corpus.com