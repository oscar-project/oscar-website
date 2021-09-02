---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Ungoliant v1"
subtitle: "The first version of the new pipeline generation tool."
summary: "The first version of the new pipeline generation tool."
authors: []
tags: []
categories: ["tool", "update"]
date: 2021-09-02T14:59:23+02:00
lastmod: 2021-09-02T14:59:23+02:00
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

# Ungoliant v1.0.0

This is the first release of Ungoliant, a project that provides tools to generate corpora from CommonCrawl.
Ungoliant also includes already established pipeline(s), in particular to generate [OSCAR][oscar]-like corpora. 

Ungoliant also replaces [`goclassy`](https://github.com/oscar-corpus/goclassy). 

Get the release from the [Releases]() tab or via cargo: `cargo install ungoliant`.

## Features

* **Feature: Downloading of CommonCrawl**. Ungoliant features an asynchronous multithreaded downloader that is faster than the previous solution used for [OSCAR][oscar].
* **Feature: Generation of both OSCAR v1 and OSCAR v1.1 corpora.** The new OSCAR v1.1 is a backward compatible corpus including metadata.
* **Feature: Deduplication using [runiq](https://github.com/whitfin/runiq).** Ungoliant currently uses a [fork](https://github.com/uinelj/runiq) that enables library access.
* **Feature: Splitting, compression and packaging**. These three operations facilitates generated corpora preparation for ulterior distribution. _Note that these operations are not yet performed on the fly, and may need huge free space._ 

## Changes

_These changes are feature evolutions from `goclassy`_

* **Pipelines and tools are available through the `ungoliant` command-line interface:** Downloading, corpus generation, deduplication and packaging are all available through Ungoliant's CLI.
* **Downloading and compilation of [fasttext](https://fasttext.cc) is not needed anymore.** Be sure to have `cmake` installed if you plan on compiling Ungoliant yourself. 
* **General performance improvements when using implemented pipelines.** This has been possible by using a multithreading of a finer granularity, using [rayon.rs](https://rayon.rs).

[oscar]: https://oscar-corpus.com