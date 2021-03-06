# Udacity Continuous Control

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The challenge of this project is to ensure that the agent (20 double-jointed arms) maintain its position at the target location for as many time steps as possible. A reward of +0.1 is provided for each step that the agent's hand is in the goal location.

The program was developed with the DDPG algorithm, based on the course code (https://github.com/udacity/deep-reinforcement-learning/tree/master/ddpg-pendulum).


## Getting started

The project is written using Jupyter Notebook (Continuous_solution.ipynb). 

In order for it to work properly you must install Python 3.6, PyTorch ((https://pytorch.org/), the ML-Agents toolkit (Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md), Numpy ((http://www.numpy.org/) and a few more Python packages required to complete the project.

See the instrucions here to set up your environment ( https://github.com/udacity/deep-reinforcement-learning#dependencies):


1.	Create (and activate) a new environment with Python 3.6.

Linux or Mac:

conda create --name drlnd python=3.6

source activate drlnd

Windows:

conda create --name drlnd python=3.6 

activate drlnd


2.	Follow the instructions in this repository to perform a minimal install of OpenAI gym: https://github.com/openai/gym 

Next, install the classic control environment group.

Then, install the box2d environment group.


3.	Clone the repository (if you haven't already!), and navigate to the python/ folder. Then, install several dependencies.

git clone https://github.com/udacity/deep-reinforcement-learning.git

cd deep-reinforcement-learning/python

pip install .


4.	Create an IPython kernel for the drlnd environment.

python -m ipykernel install --user --name drlnd --display-name "drlnd"


5.	Before running code in a notebook, change the kernel to match the drlnd environment by using the drop-down Kernel menu.

Running all the cells in the notebook (Continuous_solution.ipynb) will install it automatically.

The Reacher file is a Unity environment that will be activated when running the Jupyter file and will be able to show the agent performing the challenge of the game.

## Detail of files and project

These are the steps that execute the Jupyter file:

1. Import the Necessary Packages
2. Instantiate the Environment and agent
3. Examine the State and Action Spaces
4. Take random actions in the environment
5. Train the agent with DDPG
6. Plot the scores
7. Test agent


The project contains 8 files:

Continuous_solution.ipynb: Jupyter Notebook

ddpg_agent.py: The Agent class

model.py: The DDPG models

checkpoint_actor.pth and checkpoint_critic.pth: Saved trained model to use

Report.md: Results of the implementation

Results: Image with the results of an agent training

Reacher.app: The Game Unity Environment

