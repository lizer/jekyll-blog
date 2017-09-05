---
layout: post
title: SGD论文列表
date: '2017-09-04 17:05:13 +0000'
categories: jekyll update
published: true
--- 

### 降方差梯度下降相关论文：
* **Stochastic Averaged Gradient**:
	* **[roux2012stochastic]** Roux, Nicolas L., Mark Schmidt, and Francis R. Bach. "*A stochastic gradient method with an exponential convergence rate for finite training sets.*" Advances in Neural Information Processing Systems. 2012.

* **Stochastic Dual Coordinate Ascent**:
	* **[shalev2013stochastic]** Shalev-Shwartz, Shai, and Tong Zhang. "*Stochastic dual coordinate ascent methods for regularized loss minimization.*" Journal of Machine Learning Research 14.Feb (2013): 567-599.
	* **[zhao2015stochastic]** Zhao, Peilin, and Tong Zhang. "*Stochastic optimization with importance sampling for regularized loss minimization.*" Proceedings of the 32nd International Conference on Machine Learning (ICML-15). 2015.
	* **[csiba2015stochastic]** Csiba, Dominik, Zheng Qu, and Peter Richtárik. "*Stochastic dual coordinate ascent with adaptive probabilities.*" Proceedings of the 32nd International Conference on Machine Learning (ICML-15). 2015.

* **Stochastic Variance Reduced Gradient** descent:
	* **[johnson2013accelerating]** Johnson, Rie, and Tong Zhang. "*Accelerating stochastic gradient descent using predictive variance reduction.*" Advances in neural information processing systems. 2013.
	* **[xiao2014proximal]** Xiao, Lin, and Tong Zhang. "*A proximal stochastic gradient method with progressive variance reduction.*" SIAM Journal on Optimization 24.4 (2014): 2057-2075.

* **Mixed Optimization**:
	* **[mahdavi2013mixed]** Mahdavi, Mehrdad, Lijun Zhang, and Rong Jin. "*Mixed optimization for smooth functions.*" Advances in Neural Information Processing Systems. 2013.

* **SAGA**:
	* **[defazio2014saga]** Defazio, Aaron, Francis Bach, and Simon Lacoste-Julien. "*Saga: A fast incremental gradient method with support for non-strongly convex composite objectives.*" Advances in Neural Information Processing Systems. 2014.

* **Accelerated Algorithm**:
	* **[frostig2015regularizing]** Frostig, Roy, et al. "*Un-regularizing: approximate proximal point and faster stochastic algorithms for empirical risk minimization.*" International Conference on Machine Learning. 2015.
	* **[lin2015universal]** Lin, Hongzhou, Julien Mairal, and Zaid Harchaoui. "*A universal catalyst for first-order optimization.*" Advances in Neural Information Processing Systems. 2015.
	* **[allen2016katyusha]** Allen-Zhu, Zeyuan. "*Katyusha: Accelerated Variance Reduction for Faster SGD.*" arXiv preprint arXiv:1603.05953 (2016).

### 深度学习优化相关论文：

* **Natural gradient algorithm**:
	* **[roux2008topmoumoute]** Roux, Nicolas L., Pierre-Antoine Manzagol, and Yoshua Bengio. "*Topmoumoute online natural gradient algorithm.*" Advances in neural information processing systems. 2008.
	* **[pascanu2013revisiting]** Pascanu, Razvan, and Yoshua Bengio. "*Revisiting natural gradient for deep networks.*" arXiv preprint arXiv:1301.3584 (2013).

* **Training deep feedforward neural networks**:
	* **[glorot2010understanding]** Glorot, Xavier, and Yoshua Bengio. "*Understanding the difficulty of training deep feedforward neural networks.*" Proceedings of the Thirteenth International Conference on Artificial Intelligence and Statistics. 2010.

* **Hyper-parameter**:
	* **[bergstra2012random]** Bergstra, James, and Yoshua Bengio. "*Random search for hyper-parameter optimization.*" Journal of Machine Learning Research 13.Feb (2012): 281-305.

* **Neural Networks: Tricks of the trade**:
	* **[bengio2012practical]** Bengio, Yoshua. "*Practical recommendations for gradient-based training of deep architectures.*" Neural networks: Tricks of the trade. Springer Berlin Heidelberg, 2012. 437-478.
	* **[martens2012training]** Martens, James, and Ilya Sutskever. "*Training deep and recurrent networks with hessian-free optimization.*" Neural networks: Tricks of the trade. Springer Berlin Heidelberg, 2012. 479-535.

* **Learning rate**:
	* **[schaul2013no]** Schaul, Tom, Sixin Zhang, and Yann LeCun. "*No more pesky learning rates.*" International Conference on Machine Learning. 2013.

* **Momentum optimization**:
	* **[sutskever2013importance]** Sutskever, Ilya, et al. "*On the importance of initialization and momentum in deep learning.*" International conference on machine learning. 2013.

* **Saddle point problem in high-dimensional non-convex optimization**:
	* **[dauphin2014identifying]** Dauphin, Yann N., et al. "*Identifying and attacking the saddle point problem in high-dimensional non-convex optimization.*" Advances in neural information processing systems. 2014.

* **Adam**:
	* **[kingma2014adam]** Kingma, Diederik, and Jimmy Ba. "*Adam: A method for stochastic optimization.*" arXiv preprint arXiv:1412.6980 (2014).

* **Dropout**:
	* **[srivastava2014dropout]** Srivastava, Nitish, et al. "*Dropout: a simple way to prevent neural networks from overfitting.*" Journal of machine learning research 15.1 (2014): 1929-1958.

* **Very deep**:
	* **[srivastava2015training]** Srivastava, Rupesh K., Klaus Greff, and Jürgen Schmidhuber. "*Training very deep networks.*" Advances in neural information processing systems. 2015.

### Others
* **Flat minima**:
	* **[hochreiter1997flat]** Hochreiter, Sepp, and Jürgen Schmidhuber. "*Flat minima.*" Neural Computation 9.1 (1997): 1-42.

* **Quasi-newton**:
	* **[bordes2009sgd]** Bordes, Antoine, Léon Bottou, and Patrick Gallinari. "*Sgd-qn: Careful quasi-newton stochastic gradient descent.*" Journal of Machine Learning Research 10.Jul (2009): 1737-1754.