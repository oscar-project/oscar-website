---
# Display name
name: OSCAR

# Username (this should match the folder name)
authors:
- admin

# Is this the primary user of the site?
superuser: true

# Role/position
role: "Corpus gigantesque"

# Organizations/Affiliations
organizations: 
- name: Inria
  url: "https://www.inria.fr/"
- name: ALMAnaCH
  url: "https://team.inria.fr/almanach/fr/"

# Short bio (displayed in user profile at end of posts)
bio: Corpus polyglotte et gigantesque créé par Pedro J. Ortiz Suárez, Benoît Sagot et Laurent Romary, chercheurs de l'équipe de recherche ALMAnaCH à Inria Paris.

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
# For available icons, see: https://sourcethemes.com/academic/docs/widgets/#icons
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
  
# Organizational groups that you belong to (for People widget)
#   Set this to `[]` or comment out if you are not using People widget.  
#user_groups:
#- Researchers
#- Visitors
---

OSCAR ou **O**pen **S**uper-large **C**rawled [**A**LMAnaCH](https://team.inria.fr/almanach/) co**R**pus en anglais, est un énorme corpus multilingue obtenu par classification et filtrage du corpus [Common Crawl](https://commoncrawl.org/) à l'aide de l'architecture [goclassy](https://github.com/pjox/goclassy).

OSCAR est actuellement mélangé au niveau de ligne et aucune métadonnée n’est fournie. Ainsi, il est principalement destiné à être utilisé dans l'entraînement de modèles de langage non supervisés pour le TAL.

Les données sont distribuées par langue sous forme originale et sous forme dédupliquée. Il y a actuellement 166 langues différentes disponibles. Si vous utilisez OSCAR, pensez à de nous laisser des commentaires en utilisant le [formulaire de contact](#contact) en bas. Pensez également à citer notre [article](https://hal.inria.fr/hal-02148693).

Si vous souhaitez contribuer à OSCAR, par exemple en segmentant l'un des corpus d'une langue en tokens ou en nous aidant à traduire notre site Web, veuillez ouvrir un pull request [ici] (https://github.com/pjox/oscar-website).

Le corpus a été constitué par [Pedro J. Ortiz](https://pjortiz.com/), [Benoît Sagot](http://alpage.inria.fr/~sagot/) et [Laurent Romary](https://cv.archives-ouvertes.fr/laurentromary).
