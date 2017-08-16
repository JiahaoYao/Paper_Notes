# A Multi-Batch L-BFGS Method for Machine Learning

The paper wants to improve SGD, and it wants to employ second-order information. It is a multi-batch approach where batch changes at each iteration. The difficulty is that LBFGS wants to update Hessian approximation, and the gradients from different data causes the process to be unstable. The paper shows how  to perform stable quasi-Newton updating in the multi-batch setting.

The paper is first to implement batch L-BFGS (Robust). It achieves a good balance between computation and communication costs. It is something like fault-tolerant variant of LBFGS, that is you can be slow since I am a paralleled one or a distributed one. The challenge of LBFGS is the entire training set is not used, but a subset of data is used. It is divided into a number of batches. The algorithm operates on larger datasete for the small variance. Consecutive datasets have overlap then I employ this overlapped dataset. If teh overlap is not too small, it is very effective.

The paper wants to achieve the minimal restrictions in sample changes. The algorithm is slightly different, which  is based on the overlap dataset.

The result is convincing and achieve some kind of robustness. There is also a extended paper[^extend] 

[^extend]: https://arxiv.org/pdf/1707.08552.pdf	"A Robust Multi-Batch L-BFGS Method for Machine"

