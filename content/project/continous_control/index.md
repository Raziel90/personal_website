---
title: Continuous Control with Reinforcement Learning
summary: Reinforcement Learning algorithm to control a 2 jointed robot.
tags:
  - reinforcement-learning
date: '2022-08-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Screenshot of the training environment.
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/ClaudioInClouds
url_code: 'https://github.com/Raziel90/DeepRL_Continuous_Control'
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
# slides: example
---
## Intro
In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The first version contains a single agent.
The second version contains 20 identical agents, each with its own copy of the environment.
We focus on the latter, but the code provided can be used to solve the first environment as well. To solve this environment we must:

The agents must get an average score of +30 (over 100 consecutive episodes, and over all agents).

## Environment
![screen reader text](continous_control_environment.gif "caption")

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

## Solution
### PPO
PPO is an on-policy algorithm based on policy gradient. Here we propose an actor-critic formulation. The actor calculates the action from the state while the Critic generates the value of the state.
This implementation uses a parametrized log standard deviation used for exploring the environment. Specifically the the parameters are used on a log scale so that (after exponentiation) we guarantee strictly positive values.

### DDPG
Deep Deterministic Policy Gradient is an off-policy actor-critic Deep RL algorithm that interconnects the input and outputs of the two networks to select better policy and better value estimation iteratively. $\varepsilon$ $\pi(a|s)$.
Specifically, The actor maps state to action ($s$ -> $\pi(a|s)$) and the critic maps state action pairs to Q returns ($(s,a)$ -> $\hat{Q}(s,a)$).
```mermaid
flowchart LR
A(Actor) --> B["π(a|s)"]
s[s] --> A(Actor)
sa["(s, a)"] --> C(Critic)
C(Critic) --> q["Q(s, a)"]

style A fill:#,stroke-width:4px
style C fill:#,stroke-width:4px

style s fill:#00000000,stroke-width:0px
style sa fill:#00000000,stroke-width:0px
style q fill:#00000000,stroke-width:0px

style B fill:#00000000,stroke-width:0px
```
```mermaid
flowchart LR
A(Actor)
C(Critic)
pi["π(a|s)"]
Q["Q(s,a)"]

s --> A & C;
A --> pi;
pi --> |a|C;

Q .-> |"argmin MSE(Q(s,a), Q_target)"|C
C --> Q;
Q .-> |"argmax Q(s,a)"|A;

style pi fill:#00000000,stroke-width:0px
style Q fill:#00000000,stroke-width:0px
style s fill:#00000000,stroke-width:0px
style A fill:#,stroke-width:4px
style C fill:#,stroke-width:4px
```

## Results
### PPO
![screen reader text](PPO_Training_progression.png "Training progression of the PPO Algorithm")
<!-- <img src="PPO_Training_progression.png" alt="DDPG Training progression" style="border: 5px solid  gray; background: white"> -->

### DDPG
![screen reader text](DDPG_Training_progression.png "Training progression of the PPO Algorithm")
