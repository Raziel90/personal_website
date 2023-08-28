---
title: UoL 3D Social Interaction Dataset
summary: Dataset of 10 episodes containing a sequence of individual/social interactions in an indoor environment.
tags:
  - activity-recognition
date: '2017-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Screenshot of the training environment.
  focal_point: Smart

links:
  - name: Dataset
    url: https://lcas.lincoln.ac.uk/owncloud/index.php/s/FNb00ukctLRzxJW
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: https://linkedin.com/in/clcoppola
url_code: 'https://github.com/Raziel90/Social-Interaction-Detection-Code'
url_pdf: 'https://publications.aston.ac.uk/id/eprint/31612/1/Automatic_Detection_of_Human_Interactions_from_RGB_D_Data_for_Social_Activity_Classification.pdf'
url_slides: ''
url_video: 'https://youtu.be/KPmKn9icCMc'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
The dataset is composed of 10 sessions. Each session provides RGB-D images and skeleton tracks of 2 long videos of different activities performed by two people. Each session is zipped in a separate file, which contains a folder that has skeleton tracks in a text format and RGB (24 bits) and depth images. Each row of the skeleton text file contains information about positions (6 DoF) of 25 joints.

```
@InProceedings{Coppola2017,
Title = {Automatic Detection of Human Interactions from RGB-D Data for Social Activity Classification},
Author = {C. Coppola and S. Cosar and D. Faria and N. Bellotto},
Booktitle = {IEEE Int. Symposium on Robot and Human Interactive Communication (RO-MAN)},
Year = {2017},
Pages = {871-876}
}
```
