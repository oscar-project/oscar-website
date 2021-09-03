---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Oscar 21.08"
subtitle: "The August, 2021 version of the OSCAR Corpus."
summary: "The August, 2021 version of the OSCAR Corpus."
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
# OSCAR 21.08

OSCAR or Open Super-large Crawled Aggregated coRpus is a huge multilingual corpus obtained by language classification and filtering of the Common Crawl corpus using [Ungoliant](https://github.com/oscar-corpus/ungoliant).

This release of OSCAR is the second one, and is versioned using [CalVer](https://calver.org/).

## Features

These are the versions of tooling, schemes and data

- CommonCrawl version: February/March 2021 ([2021.10](https://commoncrawl.org/2021/03/february-march-2021-crawl-archive-now-available/))
- OSCAR Schema version: [v1.1](../oscar-schema-v1-1) : Incorporates metadata in a backward compatible manner.
- Ungoliant version: [v1](../ungoliant-v1) : New generation tool, faster and better documented/tested than the previous one: [goclassy](https://github.com/oscar-corpus/goclassy).

## Changes

- As per [OSCAR Schema v1.1](TODO), each document/record has associated metadata.
- New languages: Manx, Rusyn, Scots and West Flemish
- Removed languages: Central Bikol and Cantonese

## Table

|     | fullname                    | before   | after   | before_dedup   | after_dedup   |
|:----|:----------------------------|:---------|:--------|:---------------|:--------------|
| af  | Afrikaans                   | 251MB    | 258MB   | 170MB          | 157MB         |
| sq  | Albanian                    | 2GB      | 3GB     | 1GB            | 1GB           |
| am  | Amharic                     | 377MB    | 405MB   | 215MB          | 241MB         |
| ar  | Arabic                      | 87GB     | 69GB    | 33GB           | 35GB          |
| an  | Aragonese                   | 1MB      | 1MB     | 822KB          | 608KB         |
| hy  | Armenian                    | 3GB      | 4GB     | 1GB            | 1GB           |
| as  | Assamese                    | 117MB    | 135MB   | 73MB           | 95MB          |
| ast | Asturian                    | 2MB      | 7MB     | 2MB            | 4MB           |
| av  | Avaric                      | 418KB    | 421KB   | 331KB          | 325KB         |
| az  | Azerbaijani                 | 2GB      | 3GB     | 1GB            | 1GB           |
| bn  | Bangla                      | 10GB     | 14GB    | 6GB            | 7GB           |
| ba  | Bashkir                     | 133MB    | 110MB   | 93MB           | 77MB          |
| eu  | Basque                      | 889MB    | 900MB   | 358MB          | 503MB         |
| bar | Bavarian                    | 507B     | 2KB     | 507B           | 1KB           |
| be  | Belarusian                  | 1GB      | 2GB     | 1GB            | 1GB           |
| bh  | Bihari languages            | 112KB    | 579KB   | 34KB           | 120KB         |
| bpy | Bishnupriya                 | 4MB      | 11MB    | 1MB            | 4MB           |
| bs  | Bosnian                     | 459KB    | 310KB   | 120KB          | 175KB         |
| br  | Breton                      | 29MB     | 49MB    | 16MB           | 23MB          |
| bg  | Bulgarian                   | 33GB     | 34GB    | 14GB           | 15GB          |
| my  | Burmese                     | 2GB      | 2GB     | 1GB            | 1GB           |
| yue | Cantonese                   | 3KB      | 0B      | 2KB            | 0B            |
| ca  | Catalan                     | 8GB      | 13GB    | 4GB            | 6GB           |
| ceb | Cebuano                     | 40MB     | 81MB    | 24MB           | 58MB          |
| bcl | Central Bikol               | 886B     | 0B      | 886B           | 0B            |
| ckb | Central Kurdish             | 509MB    | 784MB   | 236MB          | 367MB         |
| cbk | Chavacano                   | 521B     | 168B    | 521B           | 168B          |
| ce  | Chechen                     | 8MB      | 29MB    | 6MB            | 20MB          |
| zh  | Chinese                     | 544GB    | 500GB   | 267GB          | 266GB         |
| cv  | Chuvash                     | 40MB     | 60MB    | 27MB           | 41MB          |
| kw  | Cornish                     | 44KB     | 119KB   | 14KB           | 72KB          |
| hr  | Croatian                    | 237MB    | 361MB   | 115MB          | 169MB         |
| cs  | Czech                       | 56GB     | 72GB    | 25GB           | 33GB          |
| da  | Danish                      | 16GB     | 18GB    | 10GB           | 10GB          |
| diq | Dimli (individual language) | 147B     | 294B    | 147B           | 147B          |
| dv  | Divehi                      | 131MB    | 143MB   | 81MB           | 111MB         |
| nl  | Dutch                       | 82GB     | 97GB    | 41GB           | 47GB          |
| mhr | Eastern Mari                | 7MB      | 15MB    | 6MB            | 10MB          |
| arz | Egyptian Arabic             | 68MB     | 48MB    | 34MB           | 21MB          |
| en  | English                     | 2520GB   | 2936GB  | 1294GB         | 1342GB        |
| myv | Erzya                       | 1KB      | 29KB    | 1KB            | 2KB           |
| eo  | Esperanto                   | 312MB    | 560MB   | 238MB          | 390MB         |
| et  | Estonian                    | 5GB      | 7GB     | 2GB            | 3GB           |
| tl  | Filipino                    | 601MB    | 699MB   | 426MB          | 383MB         |
| fi  | Finnish                     | 28GB     | 35GB    | 13GB           | 20GB          |
| fr  | French                      | 302GB    | 340GB   | 147GB          | 161GB         |
| gl  | Galician                    | 650MB    | 989MB   | 402MB          | 549MB         |
| ka  | Georgian                    | 3GB      | 6GB     | 1GB            | 2GB           |
| de  | German                      | 330GB    | 433GB   | 155GB          | 184GB         |
| gom | Goan Konkani                | 2MB      | 3MB     | 1MB            | 2MB           |
| el  | Greek                       | 66GB     | 72GB    | 28GB           | 30GB          |
| gn  | Guarani                     | 36KB     | 32KB    | 23KB           | 25KB          |
| gu  | Gujarati                    | 1GB      | 1GB     | 756MB          | 950MB         |
| ht  | Haitian Creole              | 3KB      | 2KB     | 3KB            | 1KB           |
| he  | Hebrew                      | 21GB     | 29GB    | 10GB           | 11GB          |
| hi  | Hindi                       | 17GB     | 26GB    | 9GB            | 13GB          |
| hu  | Hungarian                   | 42GB     | 60GB    | 18GB           | 29GB          |
| is  | Icelandic                   | 1GB      | 2GB     | 887MB          | 1GB           |
| io  | Ido                         | 151KB    | 276KB   | 133KB          | 221KB         |
| ilo | Iloko                       | 896KB    | 1MB     | 653KB          | 857KB         |
| id  | Indonesian                  | 32GB     | 40GB    | 16GB           | 22GB          |
| ia  | Interlingua                 | 678KB    | 291KB   | 368KB          | 172KB         |
| ie  | Interlingue                 | 24KB     | 7KB     | 1KB            | 2KB           |
| ga  | Irish                       | 91MB     | 131MB   | 62MB           | 69MB          |
| it  | Italian                     | 146GB    | 192GB   | 73GB           | 94GB          |
| ja  | Japanese                    | 231GB    | 208GB   | 112GB          | 96GB          |
| jv  | Javanese                    | 675KB    | 858KB   | 598KB          | 728KB         |
| xal | Kalmyk                      | 115KB    | 62KB    | 114KB          | 62KB          |
| kn  | Kannada                     | 1GB      | 2GB     | 1GB            | 1GB           |
| krc | Karachay-Balkar             | 2MB      | 2MB     | 2MB            | 2MB           |
| kk  | Kazakh                      | 2GB      | 3GB     | 1GB            | 1GB           |
| km  | Khmer                       | 1GB      | 1GB     | 608MB          | 860MB         |
| kv  | Komi                        | 2MB      | 1MB     | 1MB            | 588KB         |
| ko  | Korean                      | 25GB     | 35GB    | 11GB           | 15GB          |
| ku  | Kurdish                     | 98MB     | 152MB   | 62MB           | 108MB         |
| ky  | Kyrgyz                      | 629MB    | 485MB   | 406MB          | 334MB         |
| lo  | Lao                         | 181MB    | 287MB   | 118MB          | 163MB         |
| la  | Latin                       | 26MB     | 103MB   | 8MB            | 9MB           |
| lv  | Latvian                     | 4GB      | 6GB     | 1GB            | 2GB           |
| lez | Lezghian                    | 3MB      | 2MB     | 3MB            | 2MB           |
| li  | Limburgish                  | 29KB     | 76KB    | 27KB           | 54KB          |
| lt  | Lithuanian                  | 9GB      | 12GB    | 4GB            | 5GB           |
| jbo | Lojban                      | 753KB    | 929KB   | 694KB          | 731KB         |
| lmo | Lombard                     | 454KB    | 1MB     | 444KB          | 1MB           |
| nds | Low German                  | 18MB     | 25MB    | 13MB           | 17MB          |
| dsb | Lower Sorbian               | 13KB     | 31KB    | 7KB            | 14KB          |
| lb  | Luxembourgish               | 30MB     | 54MB    | 21MB           | 37MB          |
| mk  | Macedonian                  | 2GB      | 3GB     | 1GB            | 1GB           |
| mai | Maithili                    | 324KB    | 685KB   | 10KB           | 24KB          |
| mg  | Malagasy                    | 21MB     | 59MB    | 13MB           | 38MB          |
| ms  | Malay                       | 116MB    | 146MB   | 43MB           | 60MB          |
| ml  | Malayalam                   | 5GB      | 4GB     | 2GB            | 2GB           |
| mt  | Maltese                     | 24MB     | 51MB    | 17MB           | 26MB          |
| gv  | Manx                        | 0B       | 1KB     | 0B             | 907B          |
| mr  | Marathi                     | 2GB      | 3GB     | 1GB            | 1GB           |
| mzn | Mazanderani                 | 708KB    | 1MB     | 617KB          | 1MB           |
| min | Minangkabau                 | 622KB    | 8MB     | 317KB          | 1MB           |
| xmf | Mingrelian                  | 6MB      | 16MB    | 4MB            | 10MB          |
| mwl | Mirandese                   | 1KB      | 3KB     | 1KB            | 2KB           |
| mn  | Mongolian                   | 2GB      | 1GB     | 879MB          | 912MB         |
| nah | Nahuatl languages           | 11KB     | 34KB    | 10KB           | 21KB          |
| nap | Neapolitan                  | 17KB     | 1KB     | 13KB           | 1KB           |
| ne  | Nepali                      | 1GB      | 3GB     | 1GB            | 2GB           |
| new | Newari                      | 5MB      | 6MB     | 4MB            | 4MB           |
| frr | Northern Frisian            | 4KB      | 7KB     | 4KB            | 5KB           |
| lrc | Northern Luri               | 77KB     | 183B    | 64KB           | 183B          |
| no  | Norwegian Bokmål            | 8GB      | 9GB     | 5GB            | 4GB           |
| nn  | Norwegian Nynorsk           | 88MB     | 123MB   | 56MB           | 66MB          |
| oc  | Occitan                     | 6MB      | 12MB    | 3MB            | 5MB           |
| or  | Odia                        | 259MB    | 538MB   | 196MB          | 357MB         |
| os  | Ossetic                     | 12MB     | 11MB    | 10MB           | 6MB           |
| pam | Pampanga                    | 763B     | 3KB     | 307B           | 3KB           |
| ps  | Pashto                      | 378MB    | 404MB   | 253MB          | 286MB         |
| fa  | Persian                     | 84GB     | 79GB    | 39GB           | 35GB          |
| pms | Piedmontese                 | 2MB      | 4MB     | 1MB            | 3MB           |
| pl  | Polish                      | 116GB    | 122GB   | 50GB           | 48GB          |
| pt  | Portuguese                  | 132GB    | 159GB   | 67GB           | 71GB          |
| pa  | Punjabi                     | 799MB    | 769MB   | 481MB          | 430MB         |
| qu  | Quechua                     | 80KB     | 322KB   | 68KB           | 230KB         |
| ro  | Romanian                    | 26GB     | 37GB    | 11GB           | 15GB          |
| rm  | Romansh                     | 7KB      | 3KB     | 6KB            | 3KB           |
| bxr | Russia Buriat               | 12KB     | 22KB    | 10KB           | 18KB          |
| ru  | Russian                     | 1239GB   | 1201GB  | 609GB          | 542GB         |
| rue | Rusyn                       | 0B       | 247B    | 0B             | 247B          |
| sah | Sakha                       | 43MB     | 57MB    | 27MB           | 39MB          |
| sa  | Sanskrit                    | 96MB     | 72MB    | 38MB           | 43MB          |
| sco | Scots                       | 0B       | 1KB     | 0B             | 1KB           |
| gd  | Scottish Gaelic             | 1MB      | 2MB     | 1MB            | 1MB           |
| sr  | Serbian                     | 4GB      | 6GB     | 2GB            | 3GB           |
| sh  | Serbian (Latin)             | 25MB     | 13MB    | 6MB            | 9MB           |
| scn | Sicilian                    | 3KB      | 4KB     | 2KB            | 3KB           |
| sd  | Sindhi                      | 363MB    | 75MB    | 274MB          | 50MB          |
| si  | Sinhala                     | 1GB      | 1GB     | 840MB          | 791MB         |
| sk  | Slovak                      | 9GB      | 14GB    | 4GB            | 6GB           |
| sl  | Slovenian                   | 2GB      | 4GB     | 1GB            | 1GB           |
| so  | Somali                      | 62KB     | 15KB    | 15KB           | 13KB          |
| azb | South Azerbaijani           | 28MB     | 47MB    | 19MB           | 29MB          |
| es  | Spanish                     | 297GB    | 342GB   | 159GB          | 160GB         |
| su  | Sundanese                   | 216KB    | 397KB   | 145KB          | 274KB         |
| sw  | Swahili                     | 13MB     | 11MB    | 8MB            | 7MB           |
| sv  | Swedish                     | 46GB     | 43GB    | 26GB           | 19GB          |
| tg  | Tajik                       | 396MB    | 985MB   | 260MB          | 321MB         |
| ta  | Tamil                       | 9GB      | 10GB    | 5GB            | 5GB           |
| tt  | Tatar                       | 701MB    | 947MB   | 319MB          | 424MB         |
| te  | Telugu                      | 2GB      | 3GB     | 1GB            | 1GB           |
| th  | Thai                        | 38GB     | 62GB    | 17GB           | 26GB          |
| bo  | Tibetan                     | 195MB    | 439MB   | 144MB          | 358MB         |
| als | Tosk Albanian               | 5MB      | 7MB     | 2MB            | 5MB           |
| tr  | Turkish                     | 63GB     | 73GB    | 28GB           | 33GB          |
| tk  | Turkmen                     | 10MB     | 25MB    | 7MB            | 20MB          |
| tyv | Tuvinian                    | 11KB     | 9KB     | 8KB            | 7KB           |
| uk  | Ukrainian                   | 56GB     | 53GB    | 29GB           | 28GB          |
| eml | Unknown language [eml]      | 25KB     | 22KB    | 23KB           | 20KB          |
| hsb | Upper Sorbian               | 4MB      | 2MB     | 1MB            | 1MB           |
| ur  | Urdu                        | 2GB      | 2GB     | 1GB            | 1GB           |
| ug  | Uyghur                      | 127MB    | 187MB   | 86MB           | 123MB         |
| uz  | Uzbek                       | 21MB     | 56MB    | 11MB           | 28MB          |
| vec | Venetian                    | 18KB     | 37KB    | 16KB           | 28KB          |
| vi  | Vietnamese                  | 72GB     | 87GB    | 33GB           | 42GB          |
| vo  | Volapük                     | 2MB      | 2MB     | 2MB            | 2MB           |
| wa  | Walloon                     | 280KB    | 511KB   | 207KB          | 329KB         |
| war | Waray                       | 2MB      | 4MB     | 2MB            | 4MB           |
| cy  | Welsh                       | 223MB    | 307MB   | 139MB          | 180MB         |
| vls | West Flemish                | 0B       | 134B    | 0B             | 134B          |
| fy  | Western Frisian             | 35MB     | 82MB    | 26MB           | 57MB          |
| mrj | Western Mari                | 1MB      | 645KB   | 1MB            | 521KB         |
| pnb | Western Panjabi             | 11MB     | 68MB    | 9MB            | 45MB          |
| wuu | Wu Chinese                  | 111KB    | 145KB   | 32KB           | 69KB          |
| yi  | Yiddish                     | 146MB    | 199MB   | 87MB           | 93MB          |
| yo  | Yoruba                      | 56KB     | 229KB   | 26KB           | 120KB         |