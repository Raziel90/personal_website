---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Master of Puppets: Multi-modal Robot Activity Segmentation from Teleoperated
  Demonstrations'
subtitle: ''
summary: "The paper proposes a method using motion and tactile features to automatically segment atomic actions from teleoperated demonstrations for complex robotic tasks, provides a dataset of pick-and-place teleoperation with a dexterous hand, and shows the proposed features generalize between episodes and similar objects while tactile sensing improves activity recognition within demonstrations."
abstract: 'Programming robots for complex tasks in unstructured settings (e.g., light manufacturing, extreme environments) cannot be accomplished solely by analytical methods. Learning from teleoperated human demonstrations is a promising approach to decrease the programming burden and to obtain more effective controllers. However, the recorded demonstrations need to be decomposed into atomic actions to facilitate the representation of the desired behaviour, which can be very challenging in real-world settings. In this study, we propose a method that uses features extracted from robot motion and tactile data to automatically segment atomic actions from a teleoperation sequence. We created a publicly available dataset with demonstrations of robotic pick-and-place of three different objects in single-object and cluttered situations. We use a custom-built teleoperation system that maps the user’s hand and fingertips poses into a three-fingered dexterous robot hand equipped with tactile sensors. Our findings suggest that the proposed feature set generalises the activities in different episodes of the same object and between items of similar size. Furthermore, they suggest that tactile sensing contributes to higher performance in recognising activities within demonstrations.'
authors:
- Claudio Coppola
- Lorenzo Jamone
tags: ['Learning-from-Demonstrations', 'Teleoperation', 'Tactile-Sensing', 'Activity-Recognition', 'Activity-Segmentation', 'Robot-Manipulation']
categories: []
date: '2022-01-01'
lastmod: 2023-08-18T13:00:07+01:00
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  filename: ''
  caption: Overview of the proposed robot activity recognition system. The demonstrations are collected through with our RoboPuppetteer teleoperation system. The data collected during the demonstrations is processed to extract geometric and tactile features used to detect the demonstration sub-tasks
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ['MAN^3']
publishDate: '2023-08-18T12:00:07.339506Z'
publication_types:
- '1'
publication: 'IEEE International Conference of Development and Learning 2022'
url_dataset: 'https://github.com/ARQ-CRISP/CRISP_teleoperated_fruit_picking_dataset'
url_video: 'https://www.youtube.com/watch?v=nUusxghqhME'
---
