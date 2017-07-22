# REINFORCEMENT LEARNING WITH UNSUPERVISED AUXILIARY TASKS

### Introduction

-   an agent that also maximises many other pseudo-reward functions simultaneously by reinforcement learning
-   focusing this representation upon extrinsic rewards
-   approximate both the optimal policy and optimal value function for many different pseudo-rewards
    -    long-term goal of predicting cumulative extrinsic reward as well as short-term predictions of extrinsic reward
-   use an experience replay mechanism to provide additional updates to the critics (this sentence is not fully understand, and also his words 'the further research is needed')
-   Experience replay improves both data efficiency and stability of algorithms

The rewards of the reinforcement learning is very sparse, and that is just the facts of life. Therefore, the paper gives the ideas of the auxiliary prediction and control tasks to help the lack of rewards. I also do not understand why the pixel control can contribute so much to the architecture. The result is so amazing that I am overwhelmed with the enginering.