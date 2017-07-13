### _Tanalysis_

#### A simple python package for utilising basic tensor network decompositions in a data-science context

Over the last two-decades, tensor network decompositions have played a huge role in the many-body physics and quantum information communities, where they have proven themselves as an essential tool in the process of both understanding and exploiting the correlation structure of many-body quantum states. For great introductions to such decompositions -  primarily aimed at the physics community - see [here](https://arxiv.org/abs/1603.03039), [here](https://arxiv.org/abs/1008.3477) and [here](https://arxiv.org/abs/1306.2164).

However, more recently, tensor network decompositions have started to attract the attention of the machine learning and data science communities. From the learning algorithms perspective tensor networks have recently begun to be utilized, amongst other applications, as a tool for investigating and understanding the [properties of deep neural networks](https://arxiv.org/abs/1704.01552), [compressing neural network layers](https://arxiv.org/abs/1611.03214) and designing [new learning algorithms](https://arxiv.org/abs/1605.05775). From a more data science perspective, it has been recognized how various tensor network decompositions can be utilised for [feature extraction and dimensionality reduction](https://arxiv.org/abs/1403.2048), particularly within the context of [multi-dimensional datasets](https://arxiv.org/abs/1503.00516), represented by [higher order tensors](https://arxiv.org/abs/1503.00516v2), such as video and colour images.

Tanalysis is a package aimed at facilitating the use of various Matrix Product State decompositions for feature extraction and dimensionality reduction. In particular the goal is to allow flexibility and ease of use, with the hope of both spurring research in this domain, while simultaneously allowing quick and easy comparisons with existing methods on real world datasets and problems.

<center><img src="https://user-images.githubusercontent.com/6330346/28163528-d0e38428-67cb-11e7-8fe0-eabd012907bd.jpeg"></center>

#### Example usage:

In what follows we illustrate the functionality provided for in the current version of tanalysis, by looking at the [MNIST](http://yann.lecun.com/exdb/mnist/) dataset.


We begin by importing the packages we are going to use for this demonstration. In particular, in addition to tanalysis and its dependency tncontract, we will use both tensorflow and Keras, in order to illustrate a full typical use-case scenario. We also import the MNIST dataset, which is provided via tensorflow.