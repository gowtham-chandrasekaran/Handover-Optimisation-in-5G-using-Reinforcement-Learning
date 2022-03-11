# Handover Optimization using Reinforcement Learning

In this project, we are trying to optimize the number of handovers in a dense 5G network by using reinforcement learning. 
We have utilized the Q-learning of RL to create a model. 
We have performed 5000 iterations for the agent to learn all the available states and antennas.

# Purpose

The purpose of the project is to build an agent that will understand the placement of several 5G antennas, and build an optimum path to take from source to destination to avoid the number of handovers on the go. We created a gridworld environment to train the agent.

# Environment

We have created a 3 x 6 gridworld environment with antennas on different coordinates and the agent is placed in one position.
State space: Coordinates of the gridworld
Action Space: Connecting to one antenna
The Q-table is created after every episode determining the Q values of the antennas available at a coordinate.

# Learning the environment

The agent performs random walk at each episode and can take upto 150 steps per episode. The agent takes a random action that can be up, down, left or right. The agent will end up at a different state for every action taken. The agent will connect to one of the available antennas at that particular state. 

# Reward Function

The agent get +1 when there is no handover, i.e, when the antenna does not change even after taking a step and gets -1 when there is a handover, i.e, when the agent connects to a new antenna upon taking a random step.

# Output
For viewing the output results, visit https://colab.research.google.com/drive/1VUr7mj28Po3vcTRq9aNps8X_f_aRBGxU 
