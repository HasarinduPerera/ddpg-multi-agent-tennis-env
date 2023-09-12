[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135623-e770e354-7d12-11e8-998d-29fc74429ca2.gif "Trained Agent"


# DDPG: Multi-Agent Tennis Environment (Unity)

## Introduction

![Trained Agent][image1]

### Project Overview

Welcome to the Tennis Agent project README! This project involves creating intelligent agents that can play a virtual game of tennis within the [Tennis environment](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis). The agents will control rackets to keep a ball in motion over a net. Successfully hitting the ball over the net results in a reward of +0.1, while letting the ball hit the ground or go out of bounds incurs a penalty of -0.01. The primary objective is to train the agents to work collaboratively and keep the ball in play as long as possible.

### Environment Details

The Tennis environment revolves around observation and action. Agents perceive their surroundings through 8 variables that capture the position and velocity of both the ball and racket. Each agent receives its own set of observations, enabling them to have individual perspectives.

In terms of action, agents have the capability to make continuous movements towards or away from the net, and they can also jump.

### Project Objective

The ultimate goal is to train the agents to achieve an average score of +0.5 over a span of 100 consecutive episodes. This score is computed by summing up the rewards earned by each agent in an episode, without discounting. At the end of each episode, two scores are generated – one for each agent. The higher of the two scores is selected, resulting in a single **score** for that specific episode.

The project is considered successfully completed when the average of these **scores** over the course of 100 episodes reaches a minimum of +0.5. This signifies that the agents have become proficient at working collaboratively to maintain the ball's movement within the court.


## Getting Started

To get started with this repository, follow the instructions below to install the necessary dependencies and set up the project environment.

### Prerequisites

- Python 3.6.13
- PyTorch 0.4.0
- Unityagents 0.4.0

### Installation

1. Clone the repository to your local machine using the following command:

   ```
   git clone https://github.com/HasarinduPerera/ddpg-multi-agent-tennis-env
   ```

2. Change into the project directory:

   ```
   cd ddpg-multi-agent-tennis-env
   ```

3. Start the project without any additional work as the required environment, "Banana.app," is already uploaded in this project.

## Instructions

To train and test the agent, follow the instructions below.

1. Make sure you have completed the installation steps mentioned above.

2. Open the `Tennis.ipynb` notebook. It serves as the entry point for the project and contains two modes: one for training and one for testing.

3. If you already have a pre-trained model, make sure you have the `checkpoint.pth` file in your project directory. This file saves the weights of the trained model.

4. If you want to train the DQN-Agent, run the training mode in the `Tennis.ipynb` notebook. This will train the agent using reinforcement learning techniques.

5. If you only want to test the agent using a pre-trained model, load the `checkpoint.pth` file and start the test mode in the `Tennis.ipynb` notebook. This will evaluate the agent's performance in the environment.

Alternatively, you can use the `Tennis.py` file if you prefer not to use a Jupyter Notebook. It contains the same code as in the `Tennis.ipynb` notebook.

Congratulations! You have successfully trained and tested the agent in the project environment. Feel free to explore the code, experiment with different configurations, and adapt it to your specific requirements.

If you have any questions or encounter any issues while using this repository, please don't hesitate to open an issue.

