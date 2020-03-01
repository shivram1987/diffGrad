# diffGrad: An Optimization Method for Convolutional Neural Networks 

<strong><span class="color-blue"></span><sup><img style="display:inline"
                      src="https://josaa.nic.in/webinfocms/Images/newicon.gif" alt="" /></sup> <span class="newNews">It is recommended to use diffGrad_v2.py which fixes a bug in diffGrad.py.

arXiv version: https://arxiv.org/abs/1909.11015

IEEE TNNLS version: https://ieeexplore.ieee.org/document/8939562

<b>Abstract—</b>Stochastic Gradient Decent (SGD) is one of the core techniques behind the success of deep neural networks. The gradient provides information on the direction in which function has the steepest rate of change. The main problem with basic SGD is to change by equal sized steps for all parameters, irrespective of gradient behavior. Hence, an efficient way of deep network optimization is to make adaptive step sizes for each parameter. Recently, several attempts have been made to improve gradient descent methods such as AdaGrad, AdaDelta, RMSProp and Adam. These methods rely on the square roots of exponential moving averages of squared past gradients. Thus, these methods do not take the advantage of local change in gradients. In this paper, a novel optimizer is proposed based on the difference between the present and the immediate past gradient (i.e., diffGrad). In the proposed diffGrad optimization technique, the step size is adjusted for each parameter in such a way that it should have a larger step size for faster gradient changing parameters and lower step size for lower gradient changing parameters. The convergence analysis is done using the regret bound approach of online learning framework. Rigorous analysis is made in this paper over three synthetic complex non-convex functions. The image categorization experiments are also conducted over the CIFAR10 and CIFAR100 datasets to observe the performance of diffGrad with respect to the state-of-the-art optimizers such as SGDM, AdaGrad, AdaDelta, RMSProp, AMSGrad, and Adam. The residual unit (ResNet) based Convolutional Neural Networks (CNN) architecture is used in the experiments. The experiments show that diffGrad outperforms the other optimizers. Also, we showed that diffGrad performs uniformly well on network using different activation functions.

## Citation

If you use this code in your research, we would appreciate a citation to the original

      @article{dubey2019diffgrad,
      title={diffGrad: An Optimization Method for Convolutional Neural Networks},
      author={Dubey, Shiv Ram and Chakraborty, Soumendu and Roy, Swalpa Kumar and Mukherjee, Snehasis and Singh, Satish Kumar and Chaudhuri, Bidyut Baran},
      journal={IEEE Transactions on Neural Networks and Learning Systems},
      year={2019},
      publisher={IEEE}
      }

## Acknowledgement

All experiments are perfomed using following framework: https://github.com/kuangliu/pytorch-cifar


## License

Copyright (©2019): Shiv Ram Dubey, Indian Institute of Information Technology, Sri City, Chittoor, A.P., India. Released under the MIT License. See [LICENSE](LICENSE) for details.
