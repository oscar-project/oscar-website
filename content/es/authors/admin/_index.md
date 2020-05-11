---
# Display name
title: OSCAR

# Username (this should match the folder name)
authors:
- admin

# Is this the primary user of the site?
superuser: true

# Role/position
role: "Corpus Gigantesco"

# Organizations/Affiliations
organizations: 
- name: Inria
  url: "https://www.inria.fr/en/"
- name: ALMAnaCH
  url: "https://team.inria.fr/almanach/"

# Short bio (displayed in user profile at end of posts)
bio: Corpus plurilingüe y gigantesco curado por Pedro J. Ortiz Suárez, Benoît Sagot y Laurent Romary, investigadores del equipo ALMAnaCH en Inria.

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

OSCAR o **O**pen **S**uper-large **C**rawled [**A**LMAnaCH](https://team.inria.fr/almanach/) co**R**pus en Inglés, es un enorme corpus plurilingüe obtenido a partir de [Common Crawl](https://commoncrawl.org/) tras realizar operaciones de filtraje, limpieza y clasificación por idioma  utilizando la arquitectura [goclassy](https://github.com/pjox/goclassy).

El orden de las lineas para todos los subcorpus de OSCAR ha sido aleatorizado y los metadatos no han sido publicados. Por tanto, OSCAR está destinado principalmente a ser utilizado en el entrenamiento de modelos de lenguaje no supervisados para NLP.

Los datos se distribuyen por idioma en formato original y deduplicado. Actualmente hay 166 idiomas diferentes disponibles. Si usa OSCAR, por favor considere darnos su opinión utilizando el [formulario de contacto](#contact) al final de la página. Considere también citar nuestro [artículo](https://hal.inria.fr/hal-02148693).

Si desea contribuir a OSCAR, por ejemplo, tokenizando uno de los corpus para un idioma en particular o ayudándonos a traducir nuestra página web, abra una pull request [aquí](https://github.com/pjox/oscar-website).

El corpus fue creado por [Pedro J. Ortiz](https://pjortiz.com/), [Benoît Sagot](http://alpage.inria.fr/~sagot/) y [Laurent Romary](https://cv.archives-ouvertes.fr/laurentromary).
