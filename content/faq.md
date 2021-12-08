---
title: "Frequently Asked Questions"
date: 2021-09-03T10:33:56+02:00
draft: false
---

{{< toc >}}

## How can I get the original files using the HuggingFace datasets platform?

[HuggingFace](https://huggingface.co/)'s [datasets](https://huggingface.co/docs/datasets/) library internally uses [Apache arrow](https://arrow.apache.org/) files, different from the `txt.gz`/`jsonl.gz` pair that we use. 
These `.arrow` files can usually be found in `~/.cache/huggingface/datasets/` subfolders.

However, it is possible to get the original (`txt.gz`/`jsonl.gz`) files using Git LFS.

The following steps assume you have [`git`](https://git-scm.com/) and [`git-lfs`](https://git-lfs.github.com/) installed, and are on a UNIX system.
The procedure should roughly be the same on Windows, but hasn't been attempted.

```sh
$> GIT_LFS_SKIP_SMUDGE=1 git clone https://huggingface.co/datasets/oscar-corpus/OSCAR-2109 # clone the repository, ignoring LFS files
$> cd OSCAR-2109 # go inside the directory
$> git lfs pull --include packaged/eu/eu.txt.gz # pull the required file(s) (here the Basque corpus). Check with the manpage for pull options
```

You're all set! Decompress the files and you are ready to use the corpus.

## How can I decompress OSCAR Corpus files?

OSCAR is distributed in split files that are compressed in order to save spave. However, some decompression programs have trouble dealing with `gz` files.
Here are some programs that work well for the three mainstream operating systems:

- OSX/Linux-based: Use `gzip -d FILE.gz`.
- Windows: Use [7zip](https://www.7-zip.org/)

## Having a question or an issue with OSCAR?

Send us your question via our [contact form](/#contact)!
