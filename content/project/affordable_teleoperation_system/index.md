---
title: Teleoperation of dexterous robotic hands using Leap Motion and vibrotactile feedback.
summary: Teleoperation system for arm-hand dexterous manipulator
tags:
  - robotics
date: '2022-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

# image:
#   caption: Screenshot of the training environment.
#   focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: https://linkedin.com/in/clcoppola
url_code: 'https://github.com/ARQ-CRISP/teleoperation_ur5_allegro_leap'
url_pdf: 'https://ieeexplore.ieee.org/abstract/document/9900583'
url_slides: ''
url_video: 'https://youtu.be/xiJxB5OeEs8'

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
Teleoperation system for a dexterous manipulator composed of an UR5 arm and an Allegro Robot hand.
The teleoperation system uses the movement of the tracked hand in combination of the keyboard to generate the robot arm and finger movements. The tactile sensors on the fingertips generates the data used to activate the vibrator on the haptic glove. The latter is used as haptic feedback to the user for a more reactive and accurate teleoperations.

{{< video src="https://user-images.githubusercontent.com/8159414/159833096-a2a14748-be1a-4aec-83a6-37b8b14de98c.mp4" controls="yes" >}}
