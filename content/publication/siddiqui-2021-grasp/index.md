---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Grasp stability prediction for a dexterous robotic hand combining depth vision
  and haptic bayesian exploration
subtitle: ''
summary: 'The paper presents an approach using depth sensing and tactile feedback to predict safe robotic grasps of completely unknown objects through haptic exploration and comparing grid search, standard Bayesian Optimization, and unscented Bayesian Optimization, with results showing unscented Bayesian Optimization provides higher confidence grasps with fewer exploratory observations.'
authors:
- Muhammad Sami Siddiqui
- Claudio Coppola
- Gokhan Solak
- Lorenzo Jamone

author_notes:
  - 'Equal contribution'
  - 'Equal contribution'
tags: ['Grasping', 'Grasp-metric', 'Dexterous-Manipulation', 'Haptics', 'Manipulation', 'Tactile-Sensing', 'Bayesian-Optimization']
categories: []
date: '2021-01-01'
lastmod: 2023-08-18T13:00:06+01:00
featured: true
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: ['MAN^3']
publishDate: '2023-08-18T12:00:05.945332Z'
publication_types:
- '2'
abstract: 'Grasp stability prediction of unknown objects is crucial to enable autonomous robotic manipulation in an unstructured environment. Even if prior information about the object is available, real-time local exploration  might be necessary to mitigate object modelling inaccuracies. This paper presents an approach to predict safe grasps of unknown objects using depth vision and a dexterous robot hand equipped with tactile feedback. Our approach does not assume any prior knowledge about the objects. First, an object pose estimation is obtained from RGB-D sensing; then, the object is explored haptically to maximise a given grasp metric. We compare two probabilistic methods (i.e. standard and unscented Bayesian Optimisation) against random exploration (i.e. uniform grid search). Our experimental results demonstrate that these probabilistic methods can provide confident predictions after a limited number of exploratory observations, and that unscented Bayesian Optimisation can find safer grasps, taking into account the uncertainty in robot sensing and grasp execution.'
publication: 'Frontiers in Robotics and AI'
url_video: 'https://www.youtube.com/watch?v=M1-UWiRCqbs'
url_pdf: 'https://www.frontiersin.org/articles/10.3389/frobt.2021.703869/full'
url_code: 'https://github.com/ARQ-CRISP/bopt_grasp_quality'
---
