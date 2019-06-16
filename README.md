[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/42135622-e55fb586-7d12-11e8-8a54-3c31da15a90a.gif "Soccer"

# udacity nd893 project 3
nd893 Deep Reinforcement Learning - Project 3 - Collaboration and Competition

## Project Detail
Work on the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment and solve it using RLdeep learning based models for multi-agent continuous controls and actions.

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

![Trained Agent][image1]

## Coding

I wrote this code on the online workspace @ udacity. 

Still try to figure out how to build this environment on my machines.

## Installation
(this is referred to online resource, not fully tested yet)

The environment can be downloaded from one of the links below for all operating systems:
- Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
- Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
- Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
- Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
- _For AWS_: To train the agent on AWS (without [enabled virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment.  The agent can **not** be watched without a virtual screen, but can be trained.  (_To watch the agent, one can follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)
    
## Run Training

Run `Tennis.ipynb` for step-by-step details.

`model.py` contains neural network classes for Actor and Critic functional approximatior.

`MADDPG_agent.py` is the implementation of Multi Agent Deep Deterministic Policy Gradients (MADDPG) [paper](https://papers.nips.cc/paper/7217-multi-agent-actor-critic-for-mixed-cooperative-competitive-environments.pdf). In this model every agent itself is modeled as a Deep Deterministic Policy Gradient (DDPG) agent [paper](https://arxiv.org/pdf/1509.02971.pdf)

## Report

Please refer to `REPORT.md`

## Future Work

TBD, need more time
