# Generating Long-term Trajectories Using Deep Hierarchical Networks

First imitate ,then explore

### Introduction

conventional approaches are shallow model, but in this paper it learns something short-term and long-term. The paper puts forward *hierarchical policy models*, using the attention mechanism.

### Approach

Their approach learns to imitate demonstrated behaviour. And the result is macro goals can improve the performance. Their work learns sementically meaningful latent variables and gives reasons about the long-behaviour. 

And AIm is to design the policy class gives expert trajectories.

### Long-Term Trajectory Planning

Their model gives two timescale: short-term and long-term. macro-goals can be variable. There is an attention mechanism on action space, it is just a hadamard product.

Because of the intractibility of continuous, they use some kind of approximation. Multi-stage learning is just decompose the loss function into two parts. The trick may be train some raw micro-policy and macro-policy when freezing other parts.

### Imitating the players' movements

-   it is patiotemporal planning setting
-   hierrchical policy network

### Visualization

-   do not memorize tracks
-   generate rollouts wiith a high dynamic range
-   Human perference study is just what Stephen shows us

### The difference of attention and Micro-planner

-   Attention: favors a wider range of velocities and larger magnitudes
-   micro-planner favors smaller velocities

### The use of weak labels

-   do not know exactly what weak labels' definition is 
-   ​lower the accuracy on short-term prediction
-   increases the quality of the on-policy rollouts

### Summary

-   hierarchical memory network for generating long-term spatio-temporal trajectories.



### Policy structure:

-   long-term short-term defactorziation
-   Micro-policy( low-level) macro-policy(high-term)
-   goals are dynamic

### Future work

-   Robust long-term forecasting
-   Model-based RL
-   Adversarial RL
-   consider all aspects of players
-   model defensive players
-   acquire approximate weak labels to initialize the macro-planner training
-   attention mechnism can be good for other structure

The data is in the website [2017 MIT Sloan Sports](https://www.stats.com/data-science/)