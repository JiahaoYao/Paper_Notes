# Improved Training of Wasserstein GANs

>   penalize the norm of gradient of the critic with respect to its input

## Wasserstein GANs

The formula of WGAN is $$\min_G\max_{D \in \mathcal D} \mathbb E_{x\sim \mathbb P_r} D(x) -\mathbb E_{\tilde x \sim \mathbb P_g} D(\tilde x)$$ and the techinique is to clip the weight $$[-c,c]$$

The paper is discuss the weight clipping of WGAN, which leads to optimization difficulties. The difficulty is WGAN lies in the bad regime and fail to learn.

With the gradient penalty, the objective becomes $$L=\mathbb E_{\tilde x \sim \mathbb P_g} D(\tilde x) -\mathbb E_{x \sim \mathbb P_r} D(x)+ \lambda\mathbb E_{\hat x\sim \mathbb P_{\hat x}} (\Vert \nabla_{\hat x}D(\hat x)\Vert_2-1)^2$$. This penalty is two-sided penalty, force the gradient to be one.

