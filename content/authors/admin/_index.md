---
# Display name
title: OSCAR

# Is this the primary user of the site?
superuser: true

# Role/position
role: "Humongous Corpus"

# Organizations/Affiliations
organizations: 
- name: Inria
  url: "https://www.inria.fr/en/"
- name: ALMAnaCH
  url: "https://team.inria.fr/almanach/"

# Short bio (displayed in user profile at end of posts)
bio: Humongous multilingual Corpus put together by Pedro J. Ortiz Suárez, Benoît Sagot and Laurent Romary, researchers at the ALMAnaCH research team at Inria

#interests:
#- Corpus Linguistics
#- Deep Learning
#- Text Mining
#- NLP

#education:
#  courses:
#  - course: PhD in Computer Science
#    institution: Sorbonne Université
#  - course: BASc MIASHS
#    institution: Université Paris 8
#    year: 2018
#  - course: MSc in Mathematics
#    institution: Aix-Marseille Université
#    year: 2017
#  - course: BSc in Mathematics
#    institution: Universidad Nacional de Colombia
#    year: 2016

# Social/Academic Networking
# For available icons, see: https://sourcethemes.com/academic/docs/page-builder/#icons
#   For an email link, use "fas" icon pack, "envelope" icon, and a link in the
#   form "mailto:your-email@example.com" or "#contact" for contact widget.
social:
- icon: envelope
  icon_pack: fas
  link: '#contact'  # For a direct email link, use "mailto:test@example.org".
#- icon: twitter
#  icon_pack: fab
#  link: https://twitter.com/pjox13
#- icon: google-scholar
#  icon_pack: ai
#  link: https://scholar.google.co.uk/citations?user=sIwtMXoAAAAJ
- icon: github
  icon_pack: fab
  link: https://github.com/pjox/goclassy
#- icon: "key"
#  icon_pack: "fas"
#  link: files/PedroJOrtiz.asc
# Link to a PDF of your resume/CV from the About widget.
# To enable, copy your resume/CV to `static/files/cv.pdf` and uncomment the lines below.
#- icon: cv
#  icon_pack: ai
#  link: files/cv.pdf

# Enter email to display Gravatar (if Gravatar enabled in Config)
email: ""

# Highlight the author in author lists? (true/false)
highlight_name: false

# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.  
#user_groups:
#- Researchers
#- Visitors
---

OSCAR or **O**pen **S**uper-large **C**rawled **A**gregated co**R**pus is a huge multilingual corpus obtained by language classification and filtering of the [Common Crawl](https://commoncrawl.org/) corpus using the [goclassy](https://github.com/pjox/goclassy) architecture.

OSCAR is currently shuffled at line level and no metadata is provided. Thus it is mainly intended to be used in the training of unsupervised language models for NLP.

Data is distributed by language in both original and deduplicated form. There are currently 166 different languages available. If you use OSCAR please consider giving us some feedback using the [contact form](#contact) down below. Also consider citing our [paper](https://hal.inria.fr/hal-02148693).

If you want to contribute to OSCAR, for example by tokenizing one of the corpora for a particular language, or by helping us translate our webpage, please open a pull request [here](https://github.com/pjox/oscar-website).

The corpus was put together by [Pedro J. Ortiz](https://pjortiz.com/), [Benoît Sagot](http://alpage.inria.fr/~sagot/), and [Laurent Romary](https://cv.archives-ouvertes.fr/laurentromary).

If you need the unshuffled version of OSCAR, please contact us using the contact form down below. Please include your name, affiliation, contact details, which languages do you need and a brief description of how you intend to use OSCAR. You can also download it using [HuggingFace’s datasets library](https://huggingface.co/datasets/oscar).

Even though OSCAR is not [Postcardware](https://en.wikipedia.org/wiki/Shareware#Postcardware), we do appreciate when our users send us a postcard. If you want to send us one, you can find the address in the contact section down below.
