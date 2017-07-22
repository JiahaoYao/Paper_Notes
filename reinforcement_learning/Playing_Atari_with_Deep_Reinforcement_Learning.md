# Playing Atari with Deep Reinforcement Learning

I think that this paper gives the DQN Algorithm, and so I review the paper again with more focus on the algorithm.

### Algorithm

The terms in the reinforcement learning are actions, environment, rewards and observations. One thing to note here is that the agent can only observe the screen image. The goal of the agent is maximize the future reward. A standard assumption is that future reward is discounted by a factor of $\gamma$ every timestep. Also, we can write discounted return, action-value and state-value function. The optimal action-value function can be gotten by solving the Bellman equation. The intuition idea behind is just one step look ahead. Using iteration method, more specifically value iteration method, is the key to solve such a Bellman equation and thus giving an good approximation of the value function. The idea is great to approximate nonlinear function by using neural network. Since the idea is to approximate, the loss function can be simply discribed as the mean square  error. Taking the gradient and using the SGD method.

### Special

-   model-free: use the sample of environment, without approxiamting the environment.
-   off-policy: learn about the greedy policy. In practice, it is often $\epsilon$－greedy.

