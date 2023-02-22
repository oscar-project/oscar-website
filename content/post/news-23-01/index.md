---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "News: OSCAR 23.01 Release"
subtitle: ""
summary: "New filters, new categories, more compression, a fresh corpus and more"
authors: ["julien", "pedro"]
tags: []
categories: ["news"]
date: 2023-02-22T15:02:11+02:00
lastmod: 2023-02-22T15:02:11+02:00
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

{{% callout note %}}
The new OSCAR 23.01 is finally available, check it out [here](https://oscar-project.github.io/documentation/versions/oscar-2301/)! :rocket:
{{% /callout %}}

After one year of work, we're happy to announce the release of OSCAR 23.01! :rocket: OSCAR 23.01 is the January 2023 version of the OSCAR Corpus based on the [November/December 2022 dump of Common Crawl](https://commoncrawl.org/2022/12/nov-dec-2022-crawl-archive-now-available/). While being quite similar to OSCAR 22.01, it contains several new features, including:

1. [KenLM](https://kheafield.com/code/kenlm/)-based adult content detection :eyes:
2. Precomputed [Locality-Sensitive Hashes](https://fr.wikipedia.org/wiki/Locality_sensitive_hashing) for near deduplication :round_pushpin:
3. [Blocklist](https://dsi.ut-capitole.fr/blacklists/index_en.php)-based categories :books:
4. [Zstandard compression](https://facebook.github.io/zstd/) :package:
5. A new blocklist specifically made for Japanese :jp:
6. Language naming changes to better respect the BCP47 standard :pencil2::nerd_face:

To get access to this version and more information about it, please visit our documentation [here](https://oscar-project.github.io/documentation/versions/oscar-2301/).
