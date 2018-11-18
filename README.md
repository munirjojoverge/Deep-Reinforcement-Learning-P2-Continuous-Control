---
typora-root-url: ./
---

# Continuous Control: Reacher
------
## Deep Reinforcement Learning Nano-degree - Udacity

### Created/Modified on: November 11th, 2018

### Author: Munir Jojo-Verge
----



## Problem & Environment Introduction
[Reacher Environment]![Trained Agent](/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif)
Brief Description:

1. Set-up: Double-jointed arm which can move to target locations.
2. Goal: The agents must move it's hand to the goal location, and keep it there.
3. Agents: The environment contains 1 or 20 agents linked to a single Brain. (Udacity implementation version. Look below for more details)
4. Agent Reward Function (independent): +0.1 Each step agent's hand is in goal location.
5. Brains: One Brain with the following observation/action space.
6. Vector Observation space: 33 variables corresponding to position, rotation, velocity, and angular velocities of the two arm Rigidbodies.[ I left a question in the forum for a detailed description since my count didn't add up]
7. Vector Action space: (Continuous) Size of 4, corresponding to a 2D torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1
8. Visual Observations: None.
9. Reset Parameters: Two, corresponding to goal size, and goal movement speed.
10. Benchmark Mean Reward: 30

## Installation
Follow the instructions below to explore the environment on your own machine! You will also learn how to use the Python API to control your agent.

* **Step 1: Activate the Environment**
If you haven't already, please follow the instructions in the [DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies)  to set up your Python environment. These instructions can be found in README.md at the root of the repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

(For Windows users) The ML-Agents toolkit supports Windows 10. While it might be possible to run the ML-Agents toolkit using other versions of Windows, it has not been tested on other versions. Furthermore, the ML-Agents toolkit has not been tested on a Windows VM such as Bootcamp or Parallels.

* **Step 2: Download the Unity Environment**
For this project, you will not need to install Unity - this is because we have already built the environment for you, and you can download it from one of the links below. You need only select the environment that matches your operating system:
	* Version 1: One (1) Agent
		* Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip) 
		* Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
		* Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip) 
		* Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip) 
	* Version 2: Twenty (20) Agents
		* Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip) 
		* Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip) 
		* Windows (32-bit):[click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip) 
		* Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip) 

	Then, place the file in the "p2_continuous-control/" folder in the DRLND GitHub repository, and unzip (or decompress) the file.

	(For Windows users) Check out this link if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

	(For AWS) If you'd like to train the agent on AWS (and have not enabled a virtual screen), then please use this link (version 1) or this link (version 2) to obtain the "headless" version of the environment. You will not be able to watch the agent without enabling a virtual screen, but you will be able to train the agent. (To watch the agent, you should follow the instructions to enable a virtual screen, and then download the environment for the Linux operating system above.)

* **Step 3: Run this Solution and Explore the Environment**
Now you need to clone this repository. After you have followed the instructions above, open **Continuous_Control.ipynb** (located in this repository - This is the solution) and follow the instructions to run it.

Watch the (silent) video below to see what kind of output to expect from the notebook (for version 2 of the environment), if everything is working properly! Version 1 will look very similar (where you'll see a single agent, instead of 20!).
![Video](https://youtu.be/i2gVvXgOMnc)

## Report
If you are interested in more information about this implementation, please read the Report.pdf on this repository.

## Credits
Most of the code is based on the Udacity code for DDPG and recommendations ofered on the lectures. The rest is based on lots of reading and research around the topic.
