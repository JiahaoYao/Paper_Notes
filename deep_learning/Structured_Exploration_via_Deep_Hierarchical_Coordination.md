# Structured Exploration via Deep Hierarchical Coordination

-   exploitation: apply gradients using rewards observed from rollout

-   exploration: entropy regualarztion of policy -> force policy to sample enough

There is a exploration-exploitation trade-off: agents must sample rollouts from an exponentially large state-action space, but discovering good coordinated policies when each agent samples independently becomes combinatorially intractable, e.g. as N grows or the problem requires long-term coordination.

RL hard:

-   creadit assignment problm

    -   weak feedback
    -   sparse
    -   delayed

-   exploration under the curse of dimensionality


variation inference

predator-Prey model

### contribution

-   a novel hierarchical stochastic multi-agent policy class
-   a AC using variational methods

### Breakthrough

-   learn more efficiently optimal policies
-   meaningful( can be explained) coordinated agent behavior

### Introduction

This predator and prey model can be useful in many areas.It is Also formulated as dynamic multi-agent-task problems. the task here is spatiotemporal task assignment. In order to avoid the intractable methods, here the paper uses structured learning. The two approaches are to utilize a shared stochastic latent variable model and employ the principled variational method to learn the distribution.

### Cooperative Multi-agent Reinforcement Learning

The advantage function is just reduce the bias.In the experiment part, he gives some detail of the experiment. Also, some quantitative analysis is given out. Again, there are some explanation of the parameter $\lambda$: relevant, strong correlation,semantic meaningful behavior.Also, many applications in other fields: game theory, RL, Communication models, variational models, multi-task learning.