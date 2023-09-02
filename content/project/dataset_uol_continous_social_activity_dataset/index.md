---
title: UoL 3D Continuous Social Activity Dataset
summary: Dataset is composed of 20 long RGB-D videos. Each video provides RGB-D images and tracked skeleton of different social and individual activities performed by two people.
tags:
  - activity-recognition
date: '2019-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: 'https://lcas.lincoln.ac.uk/wp/research/data-sets-software/continuous-social-activity-dataset'

image:
  caption: Screenshot of the training environment.
  focal_point: Smart

links:
  - name: Dataset
    url: https://lcas.lincoln.ac.uk/owncloud/index.php/s/JCDkNNES7IscJzs
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: https://linkedin.com/in/clcoppola
url_code: 'https://github.com/Raziel90/Social-Interaction-Detection-Code'
url_pdf: 'https://link.springer.com/article/10.1007/s12369-019-00541-y'
url_slides: ''
url_video: 'https://youtu.be/GI38VAXOMwc'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

The dataset is composed of 20 long RGB-D videos. Each video provides RGB-D images and tracked skeleton of different social and individual activities performed by two people.
Each session is in a separate folder, which contains compressed full HD RGB and depth images, and two files for the skeletons of the two actors in the scene. Each row of the skeleton text file contains information about positions (6 DoF) of 25 joints.
Each video provides a labelling file containing the time intervals of each social activity in the video.
```
@Article{Coppola2019,
Title = {Social Activity Recognition on Continuous RGB-D Video Sequences},
Author = {C. Coppola and S. Cosar and D. Faria and N. Bellotto},
Journal = {International Journal of Social Robotics},
Year = {2019},
Doi = {https://doi.org/10.1007/s12369-019-00541-y}
}
```
