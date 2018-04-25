# Reinformcement Learning Tutorial

## Introduction

In reinforcement learning, the observations are taken by the agent, who then takes actions within the environment. In return for those actions, the agent receives a reward.

### The Elements

Between the environment and the agent, there are four main elements that are part of every reinforcement learning system.

**A Policy** - The policy represents the way the agent behaves at a given time.

**A Reward Signal** - This represents the goal of the problem. With each step, the agent is given a reward by the environment. the main objective of the agent is to ensure maximization of the reward in the long run.

**A Value Function** - If the reward signal determines what is good at the moment, the value function indicates what is good in the long run.

**A Model of the Environment** - This is what usually mimics the environment's behavior. These models are used for planning since they can predict the next state and reward.

## The Simulated Environment

Having an environment to train the agent in is an absolute must in reinforcement learning.

The best toolkit for developing RL algorithms that also provides a number of simulated environments is OpenAIgym.

To install this toolkit, simply use pip:

	$ pip3 install --upgrade gym


Let's open the Python shell to create the environment. For this example, we want to train our model so it can balance a moving cart's pole.

	>>> import gym
	>>> env = gym.make("CartPole-v0")
	[2018-04-24 17:03:23,199] Making new env: MsPacman-v0
	>>> obs = env.reset()
	>>> obsarray([-0.03799846, -0.03288115, 0.0237094, 0.00720711])
	>>> env.render()



