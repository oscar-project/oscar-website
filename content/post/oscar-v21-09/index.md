---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "OSCAR 21.09"
subtitle: "The September, 2021 version of the OSCAR Corpus."
summary: "The September, 2021 version of the OSCAR Corpus."
authors: ["julien", "pedro"]
tags: []
categories: ["corpus", "update"]
date: 2021-09-02T15:02:11+02:00
lastmod: 2021-09-02T15:02:11+02:00
featured: true
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
If you want to get the new corpus please send us a mail using the [mail in our homepage](/#contact), with "OSCAR Access Request" as mail title. Please include your name, last name, affiliation, contact details, which languages do you need and a brief description of how you intend to use OSCAR.
{{% /callout %}}

{{% callout warning %}}
Please do not create a new Huma-Num account by yourself, this will delay your access to the corpus by weeks! We will create an account for you.
{{% /callout %}}

OSCAR or Open Super-large Crawled Aggregated coRpus is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus using [Ungoliant](https://github.com/oscar-corpus/ungoliant).

This release of OSCAR is the second one, and is versioned using [CalVer](https://calver.org/).

## Features

These are the versions of tooling, schemes and data

- CommonCrawl version: February/March 2021 ([2021.10](https://commoncrawl.org/2021/03/february-march-2021-crawl-archive-now-available/))
- OSCAR Schema version: [v1.1](../oscar-schema-v1-1) : Incorporates metadata in a backward compatible manner.
- Ungoliant version: [v1](../ungoliant-v1) : New generation tool, faster and better documented/tested than the previous one: [goclassy](https://github.com/oscar-corpus/goclassy).

## Changes

- As per [OSCAR Schema v1.1](../oscar-schema-v1-1), each document/record has associated metadata.
- New languages: Manx, Rusyn, Scots and West Flemish. **Their size and quality still has to be assessed.**
- Removed languages: Central Bikol and Cantonese. Cantonsese was of a very [low quality](https://github.com/oscar-corpus/oscar-website/issues/11). **Central Bikol corpus is still available on [OSCAR 2019](../oscar-2019).**

## Table

|         | Language                    | OSCAR 2019 | OSCAR 2019 deduplicated | OSCAR 21.09 | OSCAR 21.09 deduplicated | Issues |
|---------|-----------------------------|------------|-------------------------|-------------|--------------------------|--------|
| af      | Afrikaans                   | 251MB      | 170MB                   | 258MB       | 157MB                    |        |
| sq      | Albanian                    | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| am      | Amharic                     | 377MB      | 215MB                   | 405MB       | 241MB                    |        |
| ar      | Arabic                      | 87GB       | 33GB                    | 69GB        | 35GB                     |        |
| an      | Aragonese                   | 1MB        | 822KB                   | 1MB         | 608KB                    |        |
| hy      | Armenian                    | 3GB        | 1GB                     | 4GB         | 1GB                      |        |
| as      | Assamese                    | 117MB      | 73MB                    | 135MB       | 95MB                     |        |
| ast     | Asturian                    | 2MB        | 2MB                     | 7MB         | 4MB                      |        |
| av      | Avaric                      | 418KB      | 331KB                   | 421KB       | 325KB                    |        |
| az      | Azerbaijani                 | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| bn      | Bangla                      | 10GB       | 6GB                     | 14GB        | 7GB                      |        |
| ba      | Bashkir                     | 133MB      | 93MB                    | 110MB       | 77MB                     |        |
| eu      | Basque                      | 889MB      | 358MB                   | 900MB       | 503MB                    |        |
| bar     | Bavarian                    | 507B       | 507B                    | 2KB         | 1KB                      |        |
| be      | Belarusian                  | 1GB        | 1GB                     | 2GB         | 1GB                      |        |
| bh      | Bihari languages            | 112KB      | 34KB                    | 579KB       | 120KB                    |        |
| bpy     | Bishnupriya                 | 4MB        | 1MB                     | 11MB        | 4MB                      |        |
| bs      | Bosnian                     | 459KB      | 120KB                   | 310KB       | 175KB                    |        |
| br      | Breton                      | 29MB       | 16MB                    | 49MB        | 23MB                     |        |
| bg      | Bulgarian                   | 33GB       | 14GB                    | 34GB        | 15GB                     |        |
| my      | Burmese                     | 2GB        | 1GB                     | 2GB         | 1GB                      |        |
| yue     | Cantonese                   | 3KB        | 2KB                     | -           | -                        |        |
| ca      | Catalan                     | 8GB        | 4GB                     | 13GB        | 6GB                      |        |
| ceb     | Cebuano                     | 40MB       | 24MB                    | 81MB        | 58MB                     |        |
| bcl     | Central Bikol               | 886B       | 886B                    | -           | -                        |        |
| ckb     | Central Kurdish             | 509MB      | 236MB                   | 784MB       | 367MB                    |        |
| cbk     | Chavacano                   | 521B       | 521B                    | 168B        | 168B                     |        |
| ce      | Chechen                     | 8MB        | 6MB                     | 29MB        | 20MB                     |        |
| zh      | Chinese                     | 544GB      | 267GB                   | 500GB       | 266GB                    |        |
| cv      | Chuvash                     | 40MB       | 27MB                    | 60MB        | 41MB                     |        |
| kw      | Cornish                     | 44KB       | 14KB                    | 119KB       | 72KB                     |        |
| hr      | Croatian                    | 237MB      | 115MB                   | 361MB       | 169MB                    |        |
| cs      | Czech                       | 56GB       | 25GB                    | 72GB        | 33GB                     |        |
| da      | Danish                      | 16GB       | 10GB                    | 18GB        | 10GB                     |        |
| diq     | Dimli (individual language) | 147B       | 147B                    | 294B        | 147B                     |        |
| dv      | Divehi                      | 131MB      | 81MB                    | 143MB       | 111MB                    |        |
| nl      | Dutch                       | 82GB       | 41GB                    | 97GB        | 47GB                     |        |
| mhr     | Eastern Mari                | 7MB        | 6MB                     | 15MB        | 10MB                     |        |
| arz     | Egyptian Arabic             | 68MB       | 34MB                    | 48MB        | 21MB                     |        |
| en      | English                     | 2520GB     | 1294GB                  | 2936GB      | 1342GB                   |        |
| myv     | Erzya                       | 1KB        | 1KB                     | 29KB        | 2KB                      |        |
| eo      | Esperanto                   | 312MB      | 238MB                   | 560MB       | 390MB                    |        |
| et      | Estonian                    | 5GB        | 2GB                     | 7GB         | 3GB                      |        |
| tl      | Filipino                    | 601MB      | 426MB                   | 699MB       | 383MB                    |        |
| fi      | Finnish                     | 28GB       | 13GB                    | 35GB        | 20GB                     |        |
| fr      | French                      | 302GB      | 147GB                   | 340GB       | 161GB                    |        |
| gl      | Galician                    | 650MB      | 402MB                   | 989MB       | 549MB                    |        |
| ka      | Georgian                    | 3GB        | 1GB                     | 6GB         | 2GB                      |        |
| de      | German                      | 330GB      | 155GB                   | 433GB       | 184GB                    |        |
| gom     | Goan Konkani                | 2MB        | 1MB                     | 3MB         | 2MB                      |        |
| el      | Greek                       | 66GB       | 28GB                    | 72GB        | 30GB                     |        |
| gn      | Guarani                     | 36KB       | 23KB                    | 32KB        | 25KB                     |        |
| gu      | Gujarati                    | 1GB        | 756MB                   | 1GB         | 950MB                    |        |
| ht      | Haitian Creole              | 3KB        | 3KB                     | 2KB         | 1KB                      |        |
| he      | Hebrew                      | 21GB       | 10GB                    | 29GB        | 11GB                     |        |
| hi      | Hindi                       | 17GB       | 9GB                     | 26GB        | 13GB                     |        |
| hu      | Hungarian                   | 42GB       | 18GB                    | 60GB        | 29GB                     |        |
| is      | Icelandic                   | 1GB        | 887MB                   | 2GB         | 1GB                      |        |
| io      | Ido                         | 151KB      | 133KB                   | 276KB       | 221KB                    |        |
| ilo     | Iloko                       | 896KB      | 653KB                   | 1MB         | 857KB                    |        |
| id      | Indonesian                  | 32GB       | 16GB                    | 40GB        | 22GB                     |        |
| ia      | Interlingua                 | 678KB      | 368KB                   | 291KB       | 172KB                    |        |
| ie      | Interlingue                 | 24KB       | 1KB                     | 7KB         | 2KB                      |        |
| ga      | Irish                       | 91MB       | 62MB                    | 131MB       | 69MB                     |        |
| it      | Italian                     | 146GB      | 73GB                    | 192GB       | 94GB                     |        |
| ja      | Japanese                    | 231GB      | 112GB                   | 208GB       | 96GB                     |        |
| jv      | Javanese                    | 675KB      | 598KB                   | 858KB       | 728KB                    |        |
| xal     | Kalmyk                      | 115KB      | 114KB                   | 62KB        | 62KB                     |        |
| kn      | Kannada                     | 1GB        | 1GB                     | 2GB         | 1GB                      |        |
| krc     | Karachay-Balkar             | 2MB        | 2MB                     | 2MB         | 2MB                      |        |
| kk      | Kazakh                      | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| km      | Khmer                       | 1GB        | 608MB                   | 1GB         | 860MB                    |        |
| kv      | Komi                        | 2MB        | 1MB                     | 1MB         | 588KB                    |        |
| ko      | Korean                      | 25GB       | 11GB                    | 35GB        | 15GB                     |        |
| ku      | Kurdish                     | 98MB       | 62MB                    | 152MB       | 108MB                    |        |
| ky      | Kyrgyz                      | 629MB      | 406MB                   | 485MB       | 334MB                    |        |
| lo      | Lao                         | 181MB      | 118MB                   | 287MB       | 163MB                    |        |
| la      | Latin                       | 26MB       | 8MB                     | 103MB       | 9MB                      |        |
| lv      | Latvian                     | 4GB        | 1GB                     | 6GB         | 2GB                      |        |
| lez     | Lezghian                    | 3MB        | 3MB                     | 2MB         | 2MB                      |        |
| li      | Limburgish                  | 29KB       | 27KB                    | 76KB        | 54KB                     |        |
| lt      | Lithuanian                  | 9GB        | 4GB                     | 12GB        | 5GB                      |        |
| jbo     | Lojban                      | 753KB      | 694KB                   | 929KB       | 731KB                    |        |
| lmo     | Lombard                     | 454KB      | 444KB                   | 1MB         | 1MB                      |        |
| nds     | Low German                  | 18MB       | 13MB                    | 25MB        | 17MB                     |        |
| dsb     | Lower Sorbian               | 13KB       | 7KB                     | 31KB        | 14KB                     |        |
| lb      | Luxembourgish               | 30MB       | 21MB                    | 54MB        | 37MB                     |        |
| mk      | Macedonian                  | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| mai     | Maithili                    | 324KB      | 10KB                    | 685KB       | 24KB                     |        |
| mg      | Malagasy                    | 21MB       | 13MB                    | 59MB        | 38MB                     |        |
| ms      | Malay                       | 116MB      | 43MB                    | 146MB       | 60MB                     |        |
| ml      | Malayalam                   | 5GB        | 2GB                     | 4GB         | 2GB                      |        |
| mt      | Maltese                     | 24MB       | 17MB                    | 51MB        | 26MB                     |        |
| gv      | Manx                        | -          | -                       | 1KB         | 907B                     |        |
| mr      | Marathi                     | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| mzn     | Mazanderani                 | 708KB      | 617KB                   | 1MB         | 1MB                      |        |
| min     | Minangkabau                 | 622KB      | 317KB                   | 8MB         | 1MB                      |        |
| xmf     | Mingrelian                  | 6MB        | 4MB                     | 16MB        | 10MB                     |        |
| mwl     | Mirandese                   | 1KB        | 1KB                     | 3KB         | 2KB                      |        |
| mn      | Mongolian                   | 2GB        | 879MB                   | 1GB         | 912MB                    |        |
| nah     | Nahuatl languages           | 11KB       | 10KB                    | 34KB        | 21KB                     |        |
| nap     | Neapolitan                  | 17KB       | 13KB                    | 1KB         | 1KB                      |        |
| ne      | Nepali                      | 1GB        | 1GB                     | 3GB         | 2GB                      |        |
| new     | Newari                      | 5MB        | 4MB                     | 6MB         | 4MB                      |        |
| frr     | Northern Frisian            | 4KB        | 4KB                     | 7KB         | 5KB                      |        |
| lrc     | Northern Luri               | 77KB       | 64KB                    | 183B        | 183B                     |        |
| no      | Norwegian Bokmål            | 8GB        | 5GB                     | 9GB         | 4GB                      |        |
| nn      | Norwegian Nynorsk           | 88MB       | 56MB                    | 123MB       | 66MB                     |        |
| oc      | Occitan                     | 6MB        | 3MB                     | 12MB        | 5MB                      |        |
| or      | Odia                        | 259MB      | 196MB                   | 538MB       | 357MB                    |        |
| os      | Ossetic                     | 12MB       | 10MB                    | 11MB        | 6MB                      |        |
| pam     | Pampanga                    | 763B       | 307B                    | 3KB         | 3KB                      |        |
| ps      | Pashto                      | 378MB      | 253MB                   | 404MB       | 286MB                    |        |
| fa      | Persian                     | 84GB       | 39GB                    | 79GB        | 35GB                     |        |
| pms     | Piedmontese                 | 2MB        | 1MB                     | 4MB         | 3MB                      |        |
| pl      | Polish                      | 116GB      | 50GB                    | 122GB       | 48GB                     |        |
| pt      | Portuguese                  | 132GB      | 67GB                    | 159GB       | 71GB                     |        |
| pa      | Punjabi                     | 799MB      | 481MB                   | 769MB       | 430MB                    |        |
| qu      | Quechua                     | 80KB       | 68KB                    | 322KB       | 230KB                    |        |
| ro      | Romanian                    | 26GB       | 11GB                    | 37GB        | 15GB                     |        |
| rm      | Romansh                     | 7KB        | 6KB                     | 3KB         | 3KB                      |        |
| bxr     | Russia Buriat               | 12KB       | 10KB                    | 22KB        | 18KB                     |        |
| ru      | Russian                     | 1239GB     | 609GB                   | 1201GB      | 542GB                    |        |
| rue     | Rusyn                       | -          | -                       | 247B        | 247B                     |        |
| sah     | Sakha                       | 43MB       | 27MB                    | 57MB        | 39MB                     |        |
| sa      | Sanskrit                    | 96MB       | 38MB                    | 72MB        | 43MB                     |        |
| sco     | Scots                       | -          | -                       | 1KB         | 1KB                      |        |
| gd      | Scottish Gaelic             | 1MB        | 1MB                     | 2MB         | 1MB                      |        |
| sr      | Serbian                     | 4GB        | 2GB                     | 6GB         | 3GB                      |        |
| sh      | Serbian (Latin)             | 25MB       | 6MB                     | 13MB        | 9MB                      |        |
| scn     | Sicilian                    | 3KB        | 2KB                     | 4KB         | 3KB                      |        |
| sd      | Sindhi                      | 363MB      | 274MB                   | 75MB        | 50MB                     |        |
| si      | Sinhala                     | 1GB        | 840MB                   | 1GB         | 791MB                    |        |
| sk      | Slovak                      | 9GB        | 4GB                     | 14GB        | 6GB                      |        |
| sl      | Slovenian                   | 2GB        | 1GB                     | 4GB         | 1GB                      |        |
| so      | Somali                      | 62KB       | 15KB                    | 15KB        | 13KB                     |        |
| azb     | South Azerbaijani           | 28MB       | 19MB                    | 47MB        | 29MB                     |        |
| es      | Spanish                     | 297GB      | 159GB                   | 342GB       | 160GB                    |        |
| su      | Sundanese                   | 216KB      | 145KB                   | 397KB       | 274KB                    |        |
| sw      | Swahili                     | 13MB       | 8MB                     | 11MB        | 7MB                      |        |
| sv      | Swedish                     | 46GB       | 26GB                    | 43GB        | 19GB                     |        |
| tg      | Tajik                       | 396MB      | 260MB                   | 985MB       | 321MB                    |{{< issue tg >}}|
| ta      | Tamil                       | 9GB        | 5GB                     | 10GB        | 5GB                      |        |
| tt      | Tatar                       | 701MB      | 319MB                   | 947MB       | 424MB                    |        |
| te      | Telugu                      | 2GB        | 1GB                     | 3GB         | 1GB                      |        |
| th      | Thai                        | 38GB       | 17GB                    | 62GB        | 26GB                     |        |
| bo      | Tibetan                     | 195MB      | 144MB                   | 439MB       | 358MB                    |        |
| gsw[^1] | Alemannic German            | 5MB        | 2MB                     | 7MB         | 5MB                      |        |
| tr      | Turkish                     | 63GB       | 28GB                    | 73GB        | 33GB                     |{{< issue tr >}}|
| tk      | Turkmen                     | 10MB       | 7MB                     | 25MB        | 20MB                     |        |
| tyv     | Tuvinian                    | 11KB       | 8KB                     | 9KB         | 7KB                      |        |
| uk      | Ukrainian                   | 56GB       | 29GB                    | 53GB        | 28GB                     |        |
| eml     | Emiliano-Romagnolo[^2]      | 25KB       | 23KB                    | 22KB        | 20KB                     |        |
| hsb     | Upper Sorbian               | 4MB        | 1MB                     | 2MB         | 1MB                      |        |
| ur      | Urdu                        | 2GB        | 1GB                     | 2GB         | 1GB                      |        |
| ug      | Uyghur                      | 127MB      | 86MB                    | 187MB       | 123MB                    |        |
| uz      | Uzbek                       | 21MB       | 11MB                    | 56MB        | 28MB                     |        |
| vec     | Venetian                    | 18KB       | 16KB                    | 37KB        | 28KB                     |        |
| vi      | Vietnamese                  | 72GB       | 33GB                    | 87GB        | 42GB                     |        |
| vo      | Volapük                     | 2MB        | 2MB                     | 2MB         | 2MB                      |        |
| wa      | Walloon                     | 280KB      | 207KB                   | 511KB       | 329KB                    |        |
| war     | Waray                       | 2MB        | 2MB                     | 4MB         | 4MB                      |        |
| cy      | Welsh                       | 223MB      | 139MB                   | 307MB       | 180MB                    |        |
| vls     | West Flemish                | -          | -                       | 134B        | 134B                     |{{< issue vls >}}|
| fy      | Western Frisian             | 35MB       | 26MB                    | 82MB        | 57MB                     |        |
| mrj     | Western Mari                | 1MB        | 1MB                     | 645KB       | 521KB                    |        |
| pnb     | Western Panjabi             | 11MB       | 9MB                     | 68MB        | 45MB                     |        |
| wuu     | Wu Chinese                  | 111KB      | 32KB                    | 145KB       | 69KB                     |{{< issue wuu >}}|
| yi      | Yiddish                     | 146MB      | 87MB                    | 199MB       | 93MB                     |        |
| yo      | Yoruba                      | 56KB       | 26KB                    | 229KB       | 120KB                    |        |



[^1]: `gsw` is [ISO 639-2](https://www.loc.gov/standards/iso639-2/php/langcodes_name.php?code_ID=177) for Alemannic German. It was previously identified as `als` in previous OSCAR versions, due to a [bug](https://github.com/facebookresearch/fastText/issues/482) in fasttext.
[^2]: `eml` identification tag is deprecated and corresponds to `rgn` and `egl` tags in [ISO 639-3](https://iso639-3.sil.org/request/2008-040) 
