---
title: A Monolingual Approach to Contextualized Word Embeddings for Mid-Resource Languages
event: The 58th Annual Meeting of the Association for Computational Linguistics
event_url: https://acl2020.org

location: Online
# address:
#   street: 31 Rue Bichat
#   city: Paris
#   region: Île-de-France
#   postcode: '75010'
#   country: France

summary: We explore the impact of the training corpus on contextualized word embeddings in five mid-resource languages.
abstract: We use the multilingual OSCAR corpus, extracted from Common Crawl via language classification, filtering and cleaning, to train monolingual contextualized word embeddings (ELMo) for five mid-resource languages. We then compare the performance of OSCAR-based and Wikipedia-based ELMo embeddings for these languages on the part-of-speech tagging and parsing tasks. We show that, despite the noise in the Common-Crawl-based OSCAR data, embeddings trained on OSCAR perform much better than monolingual embeddings trained on Wikipedia. They actually equal or improve the current state of the art in tagging and parsing for all five languages. In particular, they also improve over multilingual Wikipedia-based contextual embeddings (multilingual BERT), which almost always constitutes the previous state of the art, thereby showing that the benefit of a larger, more diverse corpus surpasses the cross-lingual benefit of multilingual embedding architectures.

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
date: "2020-07-06T11:00:00Z"
date_end: "2020-07-06T14:00:00Z"
all_day: false

# Schedule page publish date (NOT talk date).
publishDate: "2017-01-01T00:00:00Z"

authors: [pedro, Laurent Romary, Benoît Sagot]
tags: []

# Is this a featured talk? (true/false)
featured: true

#image:
#  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/bzdhc5b3Bxs)'
#  focal_point: Right

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/pjox13
#url_code: "https://github.com/pjox/goclassy"
#url_pdf: ""
url_slides: "https://docs.google.com/presentation/d/1vvamtDo5mcTtZ8hBbNMZk0tidiUgYfANNUMplMG4a9g/edit?usp=sharing"
url_video: "http://slideslive.com/38929074"

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
