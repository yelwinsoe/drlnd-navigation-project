# DRL Navigation Project
This project is for the Udacity Deep Reinforcement Learning Nano Degree program. The goal of this project is to train the agent to collection as many yellow banana as possible using Deep-Q Network.

![Yellow Banana](yellow-banana.png)

## Getting Started
Following the instruction below to setup your development environment.
1. Follow the instruction from [this link](https://github.com/udacity/deep-reinforcement-learning#dependencies) to setup your python development and install dependencies.
2. Download this repository.
3. Download one of the Unity Environment based on your operating system pre-build by Udacity.
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

    Put the file in this repository folder and unzip the file.
4. Run jupyter notebook in the root of this repository, if you don't have it yet you can [click here](https://jupyter.org/install) to install.
5. Follow along the instruction in Navigation.ipynb to train and test the model.

## Environment Details
There are 4 actions and 37 state space in ths simulatt.
The actions being -
1. Walk foward
2. Walk backward
3. Turn Left
4.Turn Right

The states contains agent's velocity, ray-based perception of objects around agent's forward directionn.

A  reward +1 is provided for collecting banana and -1 for collecting a blue banana.

The environment is coosidered solved when the agent is able to collect +13 rewards on average of 100 plays.