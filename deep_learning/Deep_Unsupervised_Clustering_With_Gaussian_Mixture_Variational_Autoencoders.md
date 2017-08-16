# DEEP UNSUPERVISED CLUSTERING WITH GAUSSIAN MIXTURE VARIATIONAL AUTOENCODERS

This is the first paper that I find the use of deep learning in clustering. The idea is to produce clustering using the deep generative models. The porblem of using VAE is cluster degeneracy. In order to mitigate such an effect, a heuristic method of minimum information constraint is a good method. I think this is the probability graph, which is traditional, and it uses the novel way of nenural network, which approximate some function by means of NN. The log-evidence lower bound [^ ELBO] used here is very famous and widely used methods. For getting the sample of the probability, here the author uses the monte carlo method. In clustering, the regularization term and reconstruction term are in tension wit each other. To attack the over-regularization problem, they uses two method. Perhaps, it is the latten code that does count and say for the specific class. I find this blog [^Ruishu] and there are also codes about it.





[^ELBO]: https://benmoran.wordpress.com/2015/02/21/variational-bayes-and-the-evidence-lower-bound/	"log-evidence lower bound can be understood by some simple mathematical analysis."
[^Ruishu]: http://ruishu.io/2016/12/25/gmvae/	"This is a blog about such a paper"