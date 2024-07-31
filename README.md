# aibjj
This is a repository for trying to make ai learn bjj. Using mujoco to simulate humanoid robots to figure out how to get from one position in bjj to the next.

# Overview
This repository contains an xml file that has 2 humanoids in bjj positions (closed guard, mount etc.). 

If you want to add new positions you will have to add new key frames to that xml using mujoco viewer. 
If you want to train an AI agent this should be possible in a colab notebook (so that you don't have to setup a local install and can just use GPUs from google).

#TO DO:
1) After researching a bit more it is probably easier to learn and use BRAX for making RL. Use this colab notebook instead https://colab.research.google.com/github/google-deepmind/mujoco/blob/main/mjx/tutorial.ipynb#scrollTo=xLiddQYPApBw
2) 




# Instructions
pip install mujoco (or pip install -r requirements.txt)
Use python -m mujoco.viewer and drag in drop the 2_humanoids.xml file and cycle through the key frames to see the different positions of bjj


Old TODO (it was too hard to try and setup a gym env)

1) figure out how to make a gym environment using this tutorial notebook https://colab.research.google.com/github/google-deepmind/dm_control/blob/main/tutorial.ipynb#scrollTo=ggVbQr5hZFl5
2) figure out how to use reinforcement learning using in colab notebook using this tutorial https://colab.research.google.com/github/jeffheaton/app_deep_learning/blob/main/t81_558_class_12_1_ai_gym.ipynb#scrollTo=UImTzmGTIeX9
3) figure out how to make a reward function that works on both humanoid agents so that they are rewarded for going to a dominant position (to basically fight each other).
4) figure out how to make a points system for bjj.
