---
title: CRISP Teleoperated Fruit Picking Dataset
summary: Dataset containing the demonstration data collected with a teleoperation system. The CRISP teleoperated fruit picking dataset contains real-world teleoperated demonstration recordings of teleoperated grasping and manipulation sequences. The dataset offers recordings of RGB-D, Tactile and kinematic data collected during fruit pick-and-place tasks. Our items are placed in the workspace as single or as a clutter to simulate real-world food manufacturing scenarios.
tags:
  - robotics
date: '2022-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

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

<p align="left">
<img src="https://user-images.githubusercontent.com/8159414/160737307-b697d4ef-38dd-4dae-8462-6f2a58e23ec7.jpg" width="250">
<img src="https://user-images.githubusercontent.com/8159414/160737333-fd431d5d-6fcc-4c06-bc8b-baf9a157c0f5.jpg" width="250"> <img src="https://user-images.githubusercontent.com/8159414/160737357-1b468612-64c4-401f-b699-704eaefb7544.jpg" width="250">
<img src="https://user-images.githubusercontent.com/8159414/160737376-1381a664-d08e-4c7b-8d09-e8960c27d854.jpg" width="250"> <img src="https://user-images.githubusercontent.com/8159414/160737387-900cec29-1712-4090-afdf-26502b4cbd7c.jpg" width="250"> <img src="https://user-images.githubusercontent.com/8159414/160737395-2d649ddd-2a0b-4acb-91e4-2c137705f133.jpg" width="250">
</p>


It comprehends 10 recordings for 3 different objects (Avocado, Banana, Blueberry Box) in 2 different scenarios (Single, Clutter) for a total of 60 demonstrations.

The dataset includes 6 activities:

- *move-in* is the act of approaching with the arm to the item the operator wants to grasp or manipulate.
- *move-out* is the opposite of the previous. It corresponds to when the robot arm is leaving the workspace, with or without the item in hand.
- *manipulate* occurs during the successful and unsuccessful manoeuvres for workspace decluttering.
- *grasp* corresponds to the act of performing a closure around the item. This activity terminates when the hand lifts with or without the item.
- *pick-up* starts at the end of the previous. It corresponds to the act of lifting the item vertically within the workspace.
- *drop* terminates all the demonstrations. It occurs after a
 while carrying the item. It terminates when the item gets in contact with a surface outside of the workspace.

--

Data Modalities
The dataset provides the following modelities:

- RGB-D
- TF (Robot hand palm, Robot Fingertips, Leap Motion tracked fingertips)
- Tactile Data
- Kinematic state of Robot hand and Arm RGB is currently available as jpegs. In case another format of RGB, Depth and ROS version of the dataset is required, please email.
- For every item and scenario, there are 10 demonstrated episodes. The dataset is organised as following:
```
avocado
    └─ single
         └── 1
             ├── allegro_fingertips.csv
             ├── allegro_joints.csv
             ├── camera_compressed
             │   ├── 1634755101828721375.jpg
             │   ├── 1634755101861649368.jpg
             │   ├── 1634755101893623525.jpg
             │   ├── 1634755101927505682.jpg
             │   ├── .................
             │   ├──
             │
             ├── labels
             ├── leap_fingertips.csv
             ├── optoforce_data.csv
             └── ur5_joints.csv
```
The demonstration activities are manually annotated with the following format: `tstamp_begin:tstamp_end;activity`.
For example, the content of the `labels` file may look like this.
```
1634844105833881526:1634844131785567065;move-in
1634844131785567065:1634844140912956220;manipulate
1634844140912956220:1634844148261190867;move-out
1634844148261190867:1634844161656180720;move-in
1634844161656180720:1634844169650791017;manipulate
1634844169650791017:1634844180109491830;move-out
1634844180109491830:1634844215461427984;move-in
1634844215461427984:1634844227849974205;grasp
1634844227849974205:1634844231262897166;pick-up
1634844231262897166:1634844242894455258;move-out
1634844242894455258:1634844247330759033;drop
```
This format has been chosen to cope with the different framerate of the different modalities.

The images of the `RGB` modalities are saved with their timestamp in the filename inside the `camera_compressed` folder.
In the other modalities, the timestamp is provided in the `time` column.
To synchronize the different modalities, you can use the `merge_as_of` function in the `pandas` package.

`allegro_fingertips.csv` - contains cartesian poses of the palm wtr of the robot base and the fingertips in the frame of the wrist.
`leap_fingertips.csv` - contains cartesian poses of the palm wtr in the leap motion frame and the fingertips in the frame of the wrist.
These are organised with the following columns

```pose_x pose_y pose_z	pose_qx	pose_qy	pose_qz	pose_qw```

the first 3 columns are the cartesian position of the other are orientation expressed in quaternions.

`allegro_joints.csv` - contains the joint states of the allegro hand (16 joints - position, velocity, effort)
`ur5_joints.csv`- contains the joint states of the allegro hand (6 joints - position, velocity, effort)
`optoforce_data.csv` - contains the tactile data obtained with the optoforce sensor placed on the manipulator fingertip.
Tactile data contains the following columns (3 components per finger x fingers).

``` index_x index_y index_z middle_x middle_y middle_z ring_x ring_y ring_z thumb_x thumb_y thumb_z ```

#### Important Note (READ HERE!)

Because of a technical fault the ring finger of the robot was not used during the collection of this dataset.
Thus, all the fields referring to the index should be ignored (e.g., `ring_x ring_y ring_z`).
These columns are kept only for compatibility with future updates of the dataset, which will include the ring finger.
