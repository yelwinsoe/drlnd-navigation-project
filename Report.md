# Report
The agent is being trained by valued-based reinforcement learning methods using deep neural network mothod called Deep-Q Network.

The neural network contains 3 layers
1. First fully connected hidden layer with ReLU activation function and has 64 nodes
2. Second fully connected hidden layer with ReLU activation fuction and has 64 nodes
3. Third fully connected linear output layer that produce action values

The agent is being trained based on the following learning parameters.
- Replay buffer size for experience replay: 1e5
- Batch size of: 64
- Discount factor Gamma as: 0.99
- Soft update value of: 1e-3
- Learning rate as: 5e-4
- The network is updated on every: 4 time steps

## Reward plot
The agent is being trained with 2000 episode but only take 600 episodes to get 13+ rewards on average of 100 plays. I observe that training more than 1000 episodes doesn't produce better result significantly for this model.
![Reward](reward_plot.png)

## Future ideas
The agent sometimes stuck between Walking forward and backward action which the agent will stop collecting the yellow banana. Implementing Double DQN, Prioritized Experience Replay or Dueling DQN might solve the problem.