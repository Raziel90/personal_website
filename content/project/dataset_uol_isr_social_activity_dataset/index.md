---
title: ISR-UoL 3D Social Activity Dataset
summary: This is a social interaction dataset between two subjects. This dataset consists of RGB and depth images, and tracked skeleton data (i.e. joints 3D coordinates and rotations) acquired by an RGB-D sensor.
tags:
  - activity-recognition
date: '2016-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Screenshot of the training environment.
  focal_point: Smart

links:
  - name: Dataset
    url: https://lcas.lincoln.ac.uk/owncloud/index.php/s/Ql44U8Py7WO4zk5
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: https://linkedin.com/in/clcoppola
url_code: 'https://github.com/Raziel90/Social-Interaction-Detection-Code'
url_pdf: 'https://publications.aston.ac.uk/id/eprint/29781/1/Social_activity_recognition_probabilistic_merging_of_skeleton_features_proximity_priors_from_RGB_D_data.pdf'
url_slides: ''
url_video: 'https://youtu.be/BmoiBus7yi8'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---

This is a social interaction dataset between two subjects. This dataset consists of RGB and depth images, and tracked skeleton data (i.e. joints 3D coordinates and rotations) acquired by an RGB-D sensor. It includes 8 social activities: {handshake, greeting hug, help walk, help stand-up, fight, push, conversation, call attention}. Each activity was recorded in a period around 40 to 60 seconds of repetitions within the same session at a frame rate of 30 frames per second. The only exceptions are help walking (at a short distance) and help stand-up, which were recorded 4 times to the same session, regardless of the time spent on it.

The activities were selected to address the assisted living scenario (e.g. happening in a health care environment: help walking, help stand-up and call attention), with potential harm situations, such as aggression (e.g. fighting, pushing), and casual activities of social interactions (e.g. handshake, greeting hug and conversation). The activities were performed by 6 persons, 4 males and  2 females with an average age of  29 years old, from different nationalities (Italian, Brazilian and Portuguese). A total of 10 different combinations of individuals (or sessions) were performed, with variation of the roles (active or passive person) between the subjects. Each subject has participated at least with 3 combinations, acting each role at least once. Half of the recorded sessions have been performed by a pair of persons whom never met before the interaction, This was done in order to increase the generalization of the study regarding individual behavior.

#### Dataset structure, download and conditions of use
The dataset is composed of 10 sessions. Each session provides RGB-D images and skeleton tracks of 8 different activities performed by two people. Each session is zipped in a separate file, which contains a folder that has skeleton tracks in a text format and RGB (24 bits) and depth (both 8 and 16 bit resolution) images. Each row of the skeleton text file contains information about positions (6 DoF) of 15 joints.


```
@INPROCEEDINGS{Coppola2016a,
author = {C. Coppola and D. Faria and U. Nunes and N. Bellotto},
title = {Social Activity Recognition based on Probabilistic Merging of Skeleton
Features with Proximity Priors from RGB-D Data},
booktitle = {Proc. of IEEE/RSJ Int. Conf. on Intelligent Robots and Systems (IROS)},
pages = {5055-5061},
year = {2016}
}
```
*Institute of Systems and Robotics (ISR-UC), University of Coimbra, Portugal  and  L-CAS, University of Lincoln, UK.
Contact: Claudio Coppola, PhD Candidate <ccoppola@lincoln.ac.uk> – Dr Diego R. Faria <d.faria@aston.ac.uk> – Dr Nicola Bellotto <nbellotto@lincoln.ac.uk>*
