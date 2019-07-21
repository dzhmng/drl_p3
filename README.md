# drl_p3

# Summary
Repository for the 3rd project for Deep Reinforcement Learning nanodegree on Udacity.

We apply DDPG to solve a multi-agent problem, where two agents control rackets to bounce a ball over a net.

The observation space consists of 8 variables corresponding to position and velocity of the ball, and each agent receives a local version of the observation. Each action is a vector with two numbers, corresponding to movement toward (or away from) the net, and jumping. If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play. After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.

The task is episodic, and in order to solve the environment, the agent must get an average score of +0.5 over 100 consecutive episodes.

# Contents

Contains the agent code (`ddpg_agent.py`), neural net code (`model.py`), training notebook (`Tennis.ipynb`), trained model weights for actor (`checkpoint_actor.pth`) and critic (`checkpoint_critic.pth`), and report (`Report.pdf`).

# Instructions

To set up the Unity environment, please follow the instructions from [Udacity's project description](https://github.com/udacity/deep-reinforcement-learning/tree/master/p3_collab-compet#getting-started)

For setting up the Python environment, please follow the dependencies instructions from [Udacity's Deep Reinforcement Learning Nanodegree materials](https://github.com/udacity/deep-reinforcement-learning#dependencies)

Follow the instructions in `Tennis.ipynb` to train the agent.
