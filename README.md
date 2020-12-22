[//]: # (Image References)

[image1]: https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif "Reacher"
# Deep Reinforcement Learning Nanodegree Project 2 Continuous Control
This repository contains submission of the project 2 of Udacity's [Deep Reinforcement learning Nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893) program.
![Reacher][image1]
### Problem description
This implementation of DDPG network to control 20 agents *(robotic manipulator)* to reach its goal position.
A reward of +0.1 is provided for each step that the agent's end-effect has reached its goal position. Thus, the goal of all agents is to maintain its position at the target location for as many time steps as possible.
#### states
For each agent, there are 33 continuous states, including agent's velocity, ray-based perception around the agent's forward direction.
#### actions
There are 4 continuous actions for each agent, these fours numbers represent the agents' joint torque value.

#### goal
The environment can be considered as solved when all agents has an average score over 30.

### Getting Started
#### local environment set up
1. Create and activate a new environment with Python 3.6 using  [Anaconda](https://www.anaconda.com/).
  - **Linux** or **Mac**
  ```bash
  conda create --name drlnd python=3.6
  source activate drlnd
  ```
  - **Windows**
  ```bash
  conda create --name drlnd python=3.6
  activate drlnd
  ```
2. Install OpenAI gym, the instruction can be find [here](https://github.com/openai/gym)
3. Install **classic control** environment group by following the instructions [here](https://github.com/openai/gym#classic-control)
4. Install the **box2d** environment by following the instructions [here](https://github.com/openai/gym#box2d).


As this submission is done using the workspace provided by the Udacity, the Unity environment is not included. If you wish to interact with the Unity environment, feel free to download the compiled Unity environment here.
- Linux: [Click Here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
- Mac OSX: [Click Here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
- Windows (64 bit): [Click Here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)   

After you have downloaded these compiled Unity environment, you need to specify the file path in the line of `Continuous_Control.ipynb`
### Instructions
follow the instruction of `Continuous_Control.ipynb`, simply run the code cell with sequential manner.
**Note**: please run the Jupyter notebook under drlnd environment.


### Results
In the end, the agents have more than 32 points on average over 132 consecutive episodes. It takes 2198 seconds to solve for this environment.
