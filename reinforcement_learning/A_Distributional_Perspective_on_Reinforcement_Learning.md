# A Distributional Perspective on Reinforcement Learning

First, DeepMind's Blog [^Blog] is interesting, which impresses me a lot about their affection for the paper and research. The topic is mainly about the rare event, which wil severely affects the life. Since the RL calculates the average, it is not that good for the rare event, and therefore value distribution is put forward. RL uses the Bellman equation and makes the prediction sequentially and updates these predictions on the basis of new information. Instead, the paper states that the distributional perspective leads to better and stable reinforcement learning. This paper gives a variant of Bellman's equation that predicts all possible outcomes, without averaging them. With this algorithm, we can do these things like disentangling the cause of randomness, telling safe and risky choices apart and natural auxiliary predictions.  It is implemented by the Deep Q-network. There is a transition from Bellman's Equation to its distributional counterpart. The agent tries to understand the intrinsic randomness. It seems that finally deep learning tries to find the distribution.



In the paper, *value distribution* dispicts the distribution form of the Bellman equation. Here it define the transition Bellman operator. 

Learning distributions matters in the presence of approximation.

One question is that the Wasserstein Metric is exactly the p-norm.

[^Blog]: https://deepmind.com/blog/going-beyond-average-reinforcement-learning/	"Going beyond average for reinforcement learning"