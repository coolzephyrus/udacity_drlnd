# Project 2: Continuous_Control

### Introduction

We wll be working with the [Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher) environment. 

In this environment, a double-jointed arm can move to target locations. 

![Reacher](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/images/reacher.png)

A reward of +0.1 is provided for each step that the agent's hands is in the goal location.
Thus, the goal of the agent is to maintain its position at
the target location for as many
steps as possible.

The observation space consists of 33 variables corresponding to position, 
rotation, velocity, and angular velocities of the arm. 
Each action is a vector with four numbers, corresponding to torque
applicable to two joints. Every 
entry in the action vector should be a number between -1 and 1. 

The task is episodic, with 1000 timesteps per episode. In order to solve
the environment, the agent must get an average score of +30 over 100 consecutive
episodes

### Dependencies

To be able to run this code, you will need an environment with Python 3 and 
the other dependencies are provided in the /python folder

Alternately the dependencies are listed in the `requirements.txt` file so that you can install them
using the following command: 
```
pip install requirements.txt
``` 
This would require to have the unity agents installed manually from the below:

1. Activate the environment:

    Please follow the instructions in the [DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

    (For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels. 

2. Download the environment from one of the links below. You need only select the environment that matches your operating system:

      Version 1: One agent

      * Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
      * Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
      * Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)


### Instructions

Run the cells in the notebook `Continuous_Control.ipynb` to train an agent that solves our required
task of moving the double-jointed arm.

### Files 
- `Continuous_Control.ipynb`: Notebook used to control and train the agent 
- `ddpg_agent.py`: Create an Agent class that interacts with and learns from the environment 
- `model.py`: Actor and Critic classes  
- `report.pdf`: Technical report
- `actor_weights.pth`: Saved model weights of the successful actor agent
- `critic_weights.pth`: Saved model weights of the successful critic agent

