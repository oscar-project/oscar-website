---
title: "Asynchronous Pipeline for Processing Huge Corpora on Medium to Low Resource Infrastructures"
authors:
- pedro
- Benoît Sagot
- Laurent Romary
date: "2019-07-22T00:00:00Z"
doi: "10.14618/IDS-PUB-9021"

# Schedule page publish date (NOT publication's date).
publishDate: "2017-01-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *7th Workshop on the Challenges in the Management of Large Corpora*
publication_short: In *CMLC-7*

abstract: Common Crawl is a considerably large, heterogeneous multilingual corpus comprised of crawled documents from the internet, surpassing 20TB of data and distributed as a set of more than 50 thousand plain text files where each contains many documents written in a wide variety of languages. Even though each document has a metadata block associated to it, this data lacks any information about the language in which each document is written, making it extremely difficult to use Common Crawl for monolingual applications. We propose a general, highly parallel, multithreaded pipeline to clean and classify Common Crawl by language; we specifically design it so that it runs efficiently on medium to low resource infrastructures where I/O speeds are the main constraint. We develop the pipeline so that it can be easily reapplied to any kind of  heterogeneous corpus and so that it can be parameterised to a wide range of infrastructures. We also distribute a 6.3TB version of Common Crawl, filtered, classified by language, shuffled at line level in order to avoid copyright issues, and ready to be used for NLP applications.

# Summary. An optional shortened abstract.
summary: We propose a new pipeline to filter, clean and classify Common Crawl by language, we publish the final corpus under the name OSCAR.

tags:
featured: true

links:
- name: CMLC-7
  url: https://ids-pub.bsz-bw.de/frontdoor/index/index/docId/8998
- name: HAL
  url: https://hal.inria.fr/hal-02148693
url_pdf: https://ids-pub.bsz-bw.de/frontdoor/deliver/index/docId/9021/file/Suarez_Sagot_Romary_Asynchronous_Pipeline_for_Processing_Huge_Corpora_2019.pdf
url_code: 'https://github.com/pjox/goclassy'
url_dataset: 'https://traces1.inria.fr/oscar/'
#url_poster: '#'
#url_project: ''
url_slides: '/files/CMLC_7_slides.pdf'
#url_source: '#'
#url_video: '#'

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
 caption: 'Image credit: [**Alix Chagué**](https://alix-tz.github.io/en/index.html)'
 focal_point: ""
 preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides:
---
