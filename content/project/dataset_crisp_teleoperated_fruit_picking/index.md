---
title: CRISP Teleoperated Fruit Picking Dataset
summary: Dataset containing the demonstration data collected with a teleoperation system. The CRISP teleoperated fruit picking dataset contains real-world teleoperated demonstration recordings of teleoperated grasping and manipulation sequences. The dataset offers recordings of RGB-D, Tactile and kinematic data collected during fruit pick-and-place tasks. Our items are placed in the workspace as single or as a clutter to simulate real-world food manufacturing scenarios.
tags:
  - robotics
date: '2022-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: 'https://github.com/ARQ-CRISP/CRISP_teleoperated_fruit_picking_dataset/tree/main'

# image:
#   caption: Screenshot of the training environment.
#   focal_point: Smart

links:
  - name: Dataset
    url: https://github.com/ARQ-CRISP/CRISP_teleoperated_fruit_picking_dataset
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
  - icon: linkedin
    icon_pack: fab
    name: Connect
    url: https://linkedin.com/in/clcoppola
url_code: ''
url_pdf: 'https://ieeexplore.ieee.org/abstract/document/9962193'
url_slides: ''
url_video: 'https://user-images.githubusercontent.com/8159414/165047534-401706df-a4b2-4379-b00c-971ade4cd4e6.mp4'


# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
{{< video src="https://user-images.githubusercontent.com/8159414/165047534-401706df-a4b2-4379-b00c-971ade4cd4e6.mp4" controls="yes" >}}

## Intro
Dataset containing the demonstration data collected with a teleoperation system. The CRISP teleoperated fruit picking dataset contains real-world teleoperated demonstration recordings of teleoperated grasping and manipulation sequences. The dataset offers recordings of RGB-D, Tactile and kinematic data collected during fruit pick-and-place tasks. Our items are placed in the workspace as single or as a clutter to simulate real-world food manufacturing scenarios.

It comprehends 10 recordings for 3 different objects (Avocado, Banana, Blueberry Box) in 2 different scenarios (Single, Clutter) for a total of 60 demonstrations.

The dataset includes 6 activities:

- `move-in` is the act of approaching with the arm to the item the operator wants to grasp or manipulate.
- `move-out` is the opposite of the previous. It corresponds to when the robot arm is leaving the workspace, with or without the item in hand.
- `manipulate` occurs during the successful and unsuccessful manoeuvres for workspace decluttering.
- `grasp` corresponds to the act of performing a closure around the item. This activity terminates when the hand lifts with or without the item.
- `pick-up` starts at the end of the previous. It corresponds to the act of lifting the item vertically within the workspace.
- `drop` terminates all the demonstrations. It occurs after a
 while carrying the item. It terminates when the item gets in contact with a surface outside of the workspace.

Check the [dataset page](https://github.com/ARQ-CRISP/CRISP_teleoperated_fruit_picking_dataset) for more details.
