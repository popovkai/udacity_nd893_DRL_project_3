#  Project Report

Use Multi Agent Deep Deterministic Policy Gradients (MADDPG) in this project.

Every agent is modeled as a Deep Deterministic Policy Gradient (DDPG2).
Compare to project-2, the difference is some information is shared between the agents. 
Each of the agents has its own actor and critic model.

The actors each receive as input the individual state (observations) of the agent and output a (two-dimensional) action.
The critic model of each actor receives the states and actions of all actors concatenated.
This facilitates the information sharing between the agents.


NN info:

- Two identical neural network configurations for both Actor and Critic.
- It contains 2 fully connected hidden layers (FC) followed by ReLU none-linear activation layers.
- Also add batch normailzation during training.


Parameters:

- Replay buffer size = 10^5
- Minibatch size = 256
- Discount factor = 0.99
- Soft update of target parameters = 1e-3
- Learning rate of the actor = 1e-4
- Learning rate of the critic = 1e-3
- L2 weight decay = 0


## Result
```
Episode 200	Average Score: 0.020
Episode 400	Average Score: 0.049
Episode 600	Average Score: 0.033
Episode 800	Average Score: 0.037
Episode 1000	Average Score: 0.045
Episode 1200	Average Score: 0.078
Episode 1400	Average Score: 0.092
Episode 1600	Average Score: 0.095
Episode 1800	Average Score: 0.095
Episode 2000	Average Score: 0.102
Episode 2200	Average Score: 0.086
Episode 2400	Average Score: 0.112
Episode 2600	Average Score: 0.217
Episode 2800	Average Score: 0.372
Episode 3000	Average Score: 0.208
Episode 3200	Average Score: 0.367
Episode 3221	Average Score: 0.525
Environment solved in 3221 episodes!	Average Score: 0.525
```


## Future Works

1. Get my machine running !! I still don't like coding at Notebook. I like vi.
2. Different hyperparameters (LR, different optimziers, epsilon)
3. Different NN configurations - current NN is not deep at all
