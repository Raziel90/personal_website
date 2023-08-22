---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Discovering stable robot grasps for unknown objects in presence of uncertainty
  using bayesian models
subtitle: ''
summary: 'The paper presents a pipeline to predict safe robotic grasps of unknown objects using depth and tactile sensing. Three methods are compared to find optimal grasp points during tactile exploration - grid search, standard Bayesian Optimization, and Unscented Bayesian Optimization. Results show Unscented Bayesian Optimization provides higher confidence in discovering safe grasps with fewer exploratory observations. It converges faster to robust grasp points away from edges compared to other methods.'
authors:
- Muhammad Sami Siddiqui
- Claudio Coppola
- Gokhan Solak
- Lorenzo Jamone
tags: ['Grasping', 'Grasp-metric', 'Dexterous-Manipulation', 'Haptics', 'Manipulation', 'Tactile-Sensing']
categories: ['Grasp-Exploration', 'Manipulation', 'Bayesian-Optimization', 'Tactile-Sensing']
date: '2021-01-01'
lastmod: 2023-08-18T13:00:06+01:00
featured: false
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
publishDate: '2023-08-18T12:00:06.365710Z'
publication_types:
- '1'
abstract: 'Autonomous grasping of unknown objects is challenging due to the uncertainty in robotic sensing and action generation. This paper presents a pipeline for predicting a safe grasp in unknown objects using depth and tactile sensing. The main objective of the work is to explore haptically to maximise a given grasp metric, such that the probability of dropping the object after lifting from the surface is minimal. The performance of the uniform grid search method is compared with probabilistic methods (i.e. standard and unscented Bayesian Optimisation) to discover safe points. The results show that unscented Bayesian Optimisation provides better confidence in finding a safe grasp. This is demonstrated by observing optimum points being far from the edges and the exploration converging sooner than other methods in a limited number of exploratory observations.'
publication: 'Annual Conference Towards Autonomous Robotic Systems'
url_video: 'https://www.youtube.com/watch?v=M1-UWiRCqbs'
---
