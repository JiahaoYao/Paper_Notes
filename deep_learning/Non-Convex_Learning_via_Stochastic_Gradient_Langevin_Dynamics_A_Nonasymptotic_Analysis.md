# Non-Convex Learning via Stochastic Gradient Langevin Dynamics: A Nonasymptotic Analysis

[DIFFUSION FOR GLOBAL OPTIMIZATION IN $\mathbb R^n$](http://epubs.siam.org/doi/pdf/10.1137/0325042) gives the theorem that the diffusion process gives the weak limit of Gibbs densities. 

SGLD is very popular. And the nonasymptotic means that it is finite here. Relate the discrete-time SGLD to continuous-time diffusion process, and also use the Euclidean 2-Wasserstein distance.

$$W_{k+1}=W_k-\eta g_k+\sqrt{2\eta \beta^{-1}\xi_k}\to dW(t)=-\nabla F_z(W(t))dt+\sqrt{2\beta^{-1}}dB(t)$$ 

decompose the difference into three parts, each of which is bounded.