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

|     | language                    | size   | words           | size (dedup)   | words (dedup)   |
|:----|:----------------------------|:-------|:----------------|:---------------|:----------------|
| af  | Afrikaans                   | 258MB  | 44,628,392      | 157MB          | 27,057,785      |
| als | Tosk Albanian               | 7MB    | 1,212,699       | 5MB            | 871,664         |
| am  | Amharic                     | 405MB  | 30,991,914      | 241MB          | 18,326,043      |
| an  | Aragonese                   | 1MB    | 115,938         | 608KB          | 89,043          |
| ar  | Arabic                      | 69GB   | 6,494,332,191   | 35GB           | 3,365,025,866   |
| arz | Egyptian Arabic             | 48MB   | 4,998,963       | 21MB           | 2,341,904       |
| ast | Asturian                    | 7MB    | 1,085,670       | 4MB            | 776,069         |
| as  | Assamese                    | 135MB  | 7,917,923       | 95MB           | 5,605,207       |
| av  | Avaric                      | 421KB  | 25,104          | 325KB          | 19,133          |
| azb | South Azerbaijani           | 47MB   | 3,595,569       | 29MB           | 2,243,562       |
| az  | Azerbaijani                 | 3GB    | 344,187,319     | 1GB            | 169,655,478     |
| bar | Bavarian                    | 2KB    | 247             | 1KB            | 245             |
| ba  | Bashkir                     | 110MB  | 8,121,603       | 77MB           | 5,625,158       |
| be  | Belarusian                  | 2GB    | 168,911,341     | 1GB            | 98,212,442      |
| bg  | Bulgarian                   | 34GB   | 2,994,775,106   | 15GB           | 1,315,091,995   |
| bh  | Bihari languages            | 579KB  | 46,436          | 120KB          | 9,181           |
| bn  | Bangla                      | 14GB   | 814,550,777     | 7GB            | 466,289,242     |
| bo  | Tibetan                     | 439MB  | 3,751,935       | 358MB          | 2,797,085       |
| bpy | Bishnupriya                 | 11MB   | 558,819         | 4MB            | 280,825         |
| br  | Breton                      | 49MB   | 8,067,480       | 23MB           | 4,032,467       |
| bs  | Bosnian                     | 310KB  | 50,266          | 175KB          | 25,157          |
| bxr | Russia Buriat               | 22KB   | 1,625           | 18KB           | 1,335           |
| ca  | Catalan                     | 13GB   | 2,110,833,307   | 6GB            | 1,012,770,904   |
| cbk | Chavacano                   | 168B   | 2               | 168B           | 2               |
| ceb | Cebuano                     | 81MB   | 12,921,589      | 58MB           | 9,201,870       |
| ce  | Chechen                     | 29MB   | 2,283,093       | 20MB           | 1,638,963       |
| ckb | Central Kurdish             | 784MB  | 63,417,572      | 367MB          | 29,355,017      |
| cs  | Czech                       | 72GB   | 9,996,052,434   | 33GB           | 4,739,928,730   |
| cv  | Chuvash                     | 60MB   | 4,592,449       | 41MB           | 3,141,872       |
| cy  | Welsh                       | 307MB  | 50,606,998      | 180MB          | 30,198,860      |
| da  | Danish                      | 18GB   | 2,892,004,180   | 10GB           | 1,704,605,898   |
| de  | German                      | 433GB  | 58,716,727,164  | 184GB          | 25,446,071,671  |
| diq | Dimli (individual language) | 294B   | 38              | 147B           | 19              |
| dsb | Lower Sorbian               | 31KB   | 4,115           | 14KB           | 1,873           |
| dv  | Divehi                      | 143MB  | 8,293,093       | 111MB          | 6,481,260       |
| el  | Greek                       | 72GB   | 6,024,414,850   | 30GB           | 2,539,719,195   |
| eml | Unknown language [eml]      | 22KB   | 4,360           | 20KB           | 3,876           |
| en  | English                     | 2936GB | 488,723,815,522 | 1342GB         | 223,669,114,922 |
| eo  | Esperanto                   | 560MB  | 84,432,772      | 390MB          | 59,411,208      |
| es  | Spanish                     | 342GB  | 54,715,337,438  | 160GB          | 25,877,724,186  |
| et  | Estonian                    | 7GB    | 954,732,803     | 3GB            | 455,553,053     |
| eu  | Basque                      | 900MB  | 110,676,692     | 503MB          | 62,812,888      |
| fa  | Persian                     | 79GB   | 8,566,653,720   | 35GB           | 3,902,206,854   |
| fi  | Finnish                     | 35GB   | 4,074,911,658   | 20GB           | 2,357,264,196   |
| frr | Northern Frisian            | 7KB    | 1,702           | 5KB            | 1,267           |
| fr  | French                      | 340GB  | 52,839,365,242  | 161GB          | 25,245,127,073  |
| fy  | Western Frisian             | 82MB   | 13,094,538      | 57MB           | 9,329,828       |
| ga  | Irish                       | 131MB  | 20,142,627      | 69MB           | 10,835,410      |
| gd  | Scottish Gaelic             | 2MB    | 332,946         | 1MB            | 173,588         |
| gl  | Galician                    | 989MB  | 155,030,216     | 549MB          | 87,015,417      |
| gn  | Guarani                     | 32KB   | 3,828           | 25KB           | 3,056           |
| gom | Goan Konkani                | 3MB    | 177,357         | 2MB            | 148,801         |
| gu  | Gujarati                    | 1GB    | 124,652,589     | 950MB          | 63,150,641      |
| gv  | Manx                        | 1KB    | 264             | 907B           | 141             |
| he  | Hebrew                      | 29GB   | 2,829,132,925   | 11GB           | 1,156,588,919   |
| hi  | Hindi                       | 26GB   | 2,009,754,819   | 13GB           | 1,038,914,735   |
| hr  | Croatian                    | 361MB  | 51,654,735      | 169MB          | 24,583,270      |
| hsb | Upper Sorbian               | 2MB    | 305,176         | 1MB            | 207,715         |
| ht  | Haitian Creole              | 2KB    | 592             | 1KB            | 351             |
| hu  | Hungarian                   | 60GB   | 7,415,936,687   | 29GB           | 3,765,883,306   |
| hy  | Armenian                    | 4GB    | 322,429,587     | 1GB            | 124,515,953     |
| ia  | Interlingua                 | 291KB  | 74,696          | 172KB          | 41,625          |
| id  | Indonesian                  | 40GB   | 5,767,715,387   | 22GB           | 3,126,926,138   |
| ie  | Interlingue                 | 7KB    | 1,432           | 2KB            | 424             |
| ilo | Iloko                       | 1MB    | 275,029         | 857KB          | 140,579         |
| io  | Ido                         | 276KB  | 46,463          | 221KB          | 36,976          |
| is  | Icelandic                   | 2GB    | 290,997,158     | 1GB            | 176,018,529     |
| it  | Italian                     | 192GB  | 29,252,541,808  | 94GB           | 14,426,829,908  |
| ja  | Japanese                    | 208GB  | 5,357,000,179   | 96GB           | 1,319,938,248   |
| jbo | Lojban                      | 929KB  | 179,684         | 731KB          | 140,749         |
| jv  | Javanese                    | 858KB  | 121,271         | 728KB          | 101,386         |
| ka  | Georgian                    | 6GB    | 304,329,117     | 2GB            | 116,422,468     |
| kk  | Kazakh                      | 3GB    | 236,767,203     | 1GB            | 126,886,720     |
| km  | Khmer                       | 1GB    | 28,188,612      | 860MB          | 13,408,408      |
| kn  | Kannada                     | 2GB    | 111,460,546     | 1GB            | 56,801,321      |
| ko  | Korean                      | 35GB   | 3,367,279,749   | 15GB           | 1,475,474,588   |
| krc | Karachay-Balkar             | 2MB    | 193,207         | 2MB            | 153,755         |
| ku  | Kurdish                     | 152MB  | 23,845,402      | 108MB          | 17,264,310      |
| kv  | Komi                        | 1MB    | 89,105          | 588KB          | 46,219          |
| kw  | Cornish                     | 119KB  | 20,775          | 72KB           | 12,687          |
| ky  | Kyrgyz                      | 485MB  | 33,401,287      | 334MB          | 23,102,129      |
| la  | Latin                       | 103MB  | 15,869,314      | 9MB            | 1,488,545       |
| lb  | Luxembourgish               | 54MB   | 7,953,887       | 37MB           | 5,454,220       |
| lez | Lezghian                    | 2MB    | 214,890         | 2MB            | 198,433         |
| li  | Limburgish                  | 76KB   | 12,105          | 54KB           | 8,472           |
| lmo | Lombard                     | 1MB    | 203,002         | 1MB            | 182,533         |
| lo  | Lao                         | 287MB  | 6,928,229       | 163MB          | 3,620,360       |
| lrc | Northern Luri               | 183B   | 26              | 183B           | 26              |
| lt  | Lithuanian                  | 12GB   | 1,573,926,673   | 5GB            | 701,326,575     |
| lv  | Latvian                     | 6GB    | 799,923,431     | 2GB            | 352,753,044     |
| mai | Maithili                    | 685KB  | 144,859         | 24KB           | 1,916           |
| mg  | Malagasy                    | 59MB   | 8,103,631       | 38MB           | 5,220,655       |
| mhr | Eastern Mari                | 15MB   | 1,170,650       | 10MB           | 784,071         |
| min | Minangkabau                 | 8MB    | 451,591         | 1MB            | 74,882          |
| mk  | Macedonian                  | 3GB    | 261,571,966     | 1GB            | 134,544,934     |
| ml  | Malayalam                   | 4GB    | 182,898,691     | 2GB            | 87,615,430      |
| mn  | Mongolian                   | 1GB    | 143,244,180     | 912MB          | 71,138,550      |
| mrj | Western Mari                | 645KB  | 51,812          | 521KB          | 41,950          |
| mr  | Marathi                     | 3GB    | 173,001,078     | 1GB            | 99,858,901      |
| ms  | Malay                       | 146MB  | 20,433,250      | 60MB           | 8,301,250       |
| mt  | Maltese                     | 51MB   | 6,162,888       | 26MB           | 3,179,815       |
| mwl | Mirandese                   | 3KB    | 419             | 2KB            | 302             |
| my  | Burmese                     | 2GB    | 54,624,239      | 1GB            | 35,969,724      |
| myv | Erzya                       | 29KB   | 2,844           | 2KB            | 236             |
| mzn | Mazanderani                 | 1MB    | 134,128         | 1MB            | 106,533         |
| nah | Nahuatl languages           | 34KB   | 3,664           | 21KB           | 2,363           |
| nap | Neapolitan                  | 1KB    | 550             | 1KB            | 235             |
| nds | Low German                  | 25MB   | 3,998,912       | 17MB           | 2,868,608       |
| ne  | Nepali                      | 3GB    | 207,891,824     | 2GB            | 142,087,100     |
| new | Newari                      | 6MB    | 433,880         | 4MB            | 254,711         |
| nl  | Dutch                       | 97GB   | 15,248,924,083  | 47GB           | 7,584,055,321   |
| nn  | Norwegian Nynorsk           | 123MB  | 20,629,675      | 66MB           | 11,095,804      |
| no  | Norwegian Bokmål            | 9GB    | 1,492,984,384   | 4GB            | 776,354,517     |
| oc  | Occitan                     | 12MB   | 1,822,595       | 5MB            | 834,187         |
| or  | Odia                        | 538MB  | 30,838,706      | 357MB          | 20,357,839      |
| os  | Ossetic                     | 11MB   | 911,794         | 6MB            | 536,525         |
| pam | Pampanga                    | 3KB    | 405             | 3KB            | 405             |
| pa  | Punjabi                     | 769MB  | 59,031,334      | 430MB          | 33,413,527      |
| pl  | Polish                      | 122GB  | 16,120,806,481  | 48GB           | 6,496,098,108   |
| pms | Piedmontese                 | 4MB    | 804,600         | 3MB            | 644,017         |
| pnb | Western Panjabi             | 68MB   | 7,757,785       | 45MB           | 5,221,168       |
| ps  | Pashto                      | 404MB  | 49,643,597      | 286MB          | 35,345,424      |
| pt  | Portuguese                  | 159GB  | 24,770,395,312  | 71GB           | 11,190,148,216  |
| qu  | Quechua                     | 322KB  | 40,691          | 230KB          | 29,108          |
| rm  | Romansh                     | 3KB    | 512             | 3KB            | 429             |
| ro  | Romanian                    | 37GB   | 5,629,438,576   | 15GB           | 2,387,230,734   |
| rue | Rusyn                       | 247B   | 14              | 247B           | 14              |
| ru  | Russian                     | 1201GB | 89,568,364,811  | 542GB          | 41,194,052,384  |
| sah | Sakha                       | 57MB   | 2,600,989       | 39MB           | 1,944,651       |
| sa  | Sanskrit                    | 72MB   | 3,288,786       | 43MB           | 1,998,089       |
| scn | Sicilian                    | 4KB    | 712             | 3KB            | 516             |
| sco | Scots                       | 1KB    | 523             | 1KB            | 282             |
| sd  | Sindhi                      | 75MB   | 8,937,427       | 50MB           | 6,064,102       |
| sh  | Serbian (Latin)             | 13MB   | 2,164,175       | 9MB            | 1,461,045       |
| si  | Sinhala                     | 1GB    | 91,456,436      | 791MB          | 47,770,919      |
| sk  | Slovak                      | 14GB   | 2,002,088,524   | 6GB            | 865,456,498     |
| sl  | Slovenian                   | 4GB    | 610,843,131     | 1GB            | 288,222,997     |
| so  | Somali                      | 15KB   | 849             | 13KB           | 449             |
| sq  | Albanian                    | 3GB    | 493,861,192     | 1GB            | 257,278,518     |
| sr  | Serbian                     | 6GB    | 574,460,746     | 3GB            | 289,211,579     |
| su  | Sundanese                   | 397KB  | 54,420          | 274KB          | 37,082          |
| sv  | Swedish                     | 43GB   | 6,542,433,732   | 19GB           | 2,964,887,952   |
| sw  | Swahili                     | 11MB   | 1,853,022       | 7MB            | 1,279,350       |
| ta  | Tamil                       | 10GB   | 438,489,984     | 5GB            | 215,856,584     |
| te  | Telugu                      | 3GB    | 182,268,133     | 1GB            | 73,193,605      |
| tg  | Tajik                       | 985MB  | 79,016,232      | 321MB          | 26,069,632      |
| th  | Thai                        | 62GB   | 1,694,658,532   | 26GB           | 635,230,676     |
| tk  | Turkmen                     | 25MB   | 2,693,720       | 20MB           | 2,221,760       |
| tl  | Filipino                    | 699MB  | 115,471,760     | 383MB          | 62,473,283      |
| tr  | Turkish                     | 73GB   | 8,763,467,387   | 33GB           | 3,950,989,357   |
| tt  | Tatar                       | 947MB  | 68,793,924      | 424MB          | 31,485,000      |
| tyv | Tuvinian                    | 9KB    | 638             | 7KB            | 542             |
| ug  | Uyghur                      | 187MB  | 12,786,741      | 123MB          | 8,410,269       |
| uk  | Ukrainian                   | 53GB   | 4,014,675,914   | 28GB           | 2,131,491,321   |
| ur  | Urdu                        | 2GB    | 354,937,986     | 1GB            | 234,111,239     |
| uz  | Uzbek                       | 56MB   | 6,237,371       | 28MB           | 3,327,595       |
| vec | Venetian                    | 37KB   | 6,694           | 28KB           | 5,139           |
| vi  | Vietnamese                  | 87GB   | 14,523,772,784  | 42GB           | 7,011,404,625   |
| vls | West Flemish                | 134B   | 2               | 134B           | 2               |
| vo  | Volapük                     | 2MB    | 426,052         | 2MB            | 410,688         |
| war | Waray                       | 4MB    | 750,162         | 4MB            | 702,336         |
| wa  | Walloon                     | 511KB  | 93,163          | 329KB          | 59,906          |
| wuu | Wu Chinese                  | 145KB  | 9,130           | 69KB           | 3,031           |
| xal | Kalmyk                      | 62KB   | 5,495           | 62KB           | 5,495           |
| xmf | Mingrelian                  | 16MB   | 807,158         | 10MB           | 510,700         |
| yi  | Yiddish                     | 199MB  | 18,699,112      | 93MB           | 8,716,366       |
| yo  | Yoruba                      | 229KB  | 34,468          | 120KB          | 17,487          |
| zh  | Chinese                     | 500GB  | 10,118,381,906  | 266GB          | 3,898,987,727   |
