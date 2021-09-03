---
title: Asynchronous Pipeline for Processing Huge Corpora on Medium to Low Resource Infrastructures
event: 7th Workshop on the Challenges in the Management of Large Corpora
event_url: http://corpora.ids-mannheim.de/cmlc-2019.html
location: Cardiff, UK
summary: We propose a new pipeline to filter, clean and classify Common Crawl by language, we publish the final corpus under the name OSCAR.
abstract: Common Crawl is a considerably large, heterogeneous multilingual corpus comprised of crawled documents from the internet, surpassing 20TB of data and distributed as a set of more than 50 thousand plain text files where each contains many documents written in a wide variety of languages. Even though each document has a metadata block associated to it, this data lacks any information about the language in which each document is written, making it extremely difficult to use Common Crawl for monolingual applications. We propose a general, highly parallel, multithreaded pipeline to clean and classify Common Crawl by language; we specifically design it so that it runs efficiently on medium to low resource infrastructures where I/O speeds are the main constraint. We develop the pipeline so that it can be easily reapplied to any kind of  heterogeneous corpus and so that it can be parameterised to a wide range of infrastructures. We also distribute a 6.3TB version of Common Crawl, filtered, classified by language, shuffled at line level in order to avoid copyright issues, and ready to be used for NLP applications.


# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2019-07-22T09:30:00Z"
date_end: "2019-07-22T10:00:00Z"
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2017-01-01T00:00:00Z"

authors: [pedro, benoit, laurent]
tags: []

# Is this a featured talk? (true/false)
featured: true

#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
#  focal_point: Right

links:
- name: Workshop
  url: http://corpora.ids-mannheim.de/cmlc-2019.html
url_code: "https://github.com/oscar-corpus/goclassy"
url_pdf: "http://corpora.ids-mannheim.de/CMLC7-final/CMLC-7_2019-Oritz_et_al.pdf"
url_slides: ""
url_video: ""

# Markdown Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
#slides: example

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
#projects:
#- internal-project

# Enable math on this page?
math: true
---
