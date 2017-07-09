# A Hitting Time Analysis of Stochastic Gradient Langevin Dynamics

### Two main results in this paper

-   if the empirical risk is pointwise close to the (smooth) population risk, then the algorithm finds an approximate local minimum of the population risk in polynomial time, escaping suboptimal local minima that only exist in the empirical risk
-   SGLD improves on one of the best known learnability results for learning linear classifiers under the zero-one loss.

How to escape "approximately shallow" local minima

-   inject random noise to the gradient

$$x<- x- \eta (\nabla f(x)+\omega)$$

-   Langevin Monte Carlo (LMC)


$$x<- x -\eta(\nabla f(x)+\sqrt{\frac{2}{\eta\xi}} w), w\sim \mathbb N(0,I)$$

It converges to stationary distribution (Gibbs distribution). It takes some times (related to h) to escape the depth-h basin of attraction.

### Contribution

Not bounding the mixing time, but the paper bounds the hitting time instead. And two results are that SGLD hits the local minima of f, with a hitting time is polynomial in dimension d and the other result is that the time complexity bound is stable. Two properties together gives the result of hitting an approximate local minima in polynomial time. And the technique here is mainly restricted Cheeger constant.

-   hitting time is polynomial in the inverse of the restricted Cheeger constant
-   Give the SGLD, mixing the metropolis together
-   give the stability of restricted Cheeger constant by lower bounding the restricted Cheeger constant

### Conclusion

Here I omit the detail in this paper

-   The approach here is different from the existing analysis which is continuous analysis. 
-   Establish the polynomial-time guarantees for achieving certain optimality sets.
-   empirical risk can be optimized far below the population risk
-   avoid poor population local minima.


### Reference

-   [Gradient Descent Can Take Exponential Time to Escape Saddle Points](https://uk.arxiv.org/pdf/1705.10412.pdf) add some perturbance to the GD in order to escape the saddle point


