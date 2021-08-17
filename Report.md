# Report
The agent is being trained by valued-based reinforcement learning methods using deep neural network mothod called Deep-Q Network.

The neural network contains 3 layers
1. First fully connected convolutional neural layer that take state space as input
2. Second fully connected convolutional neural layer that take the output from the first layer
3. Third fully connected linear layer that take the output from the second layer and finally return the action

The agent is being trained based on the following learning parameters.
- Replay buffer size for experience replay: 1e5
- Batch size of: 64
- Discount factor Gamma as: 0.99
- Soft update value of: 1e-3
- Learning rate as: 5e-4
- The network is updated on every: 4 time steps

## Reward plot of 100 episodes of 14.09 rewards
![Reward](reward_plot.png)

It only take 600 episodes of training to get +13 rewards on average of 100 plays.

## Future ideas
The agent sometimes stuck between Walking forward and backward action which the agent will stop collecting the yellow banana. Implementing Double DQN, Prioritized Experience Replay or Dueling DQN might solve the problem.