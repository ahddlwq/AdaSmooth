# Demos

Here we provide some demos of using AdaSmooth on several benchmark tasks.
The purpose of these demos is to give an example of how to use it your research, and also
illustrate the robust performance of AdaSmooth.

In short, AdaSmooth can be regarded as an optimizer that dynamically transforms from Adam to SGD as
the training step becomes larger.
In this way, it can ** combine the advantages of ADABOUND and AdaMod algorithms, viz. achieve a smooth transition 
from adaptive methods in the early stage of training to SGD at the end**.

In most examples, you can observe that AdaSmooth has a much faster training speed than SGD
in the early stage, and the learning curve is much smoother than that of SGD.
As for the final performance on unseen data, AdaSmooth can achieve better or similar performance
compared with SGD, and has a considerable improvement over the adaptive methods.

## Demo List
- CIFAR-10 \[[notebook](./cifar10/visualization.ipynb)\] \[[code](./cifar10)\]
- MNIST \[[notebook](./MNIST/visualization.ipynb)\] \[[code](./MNIST)\]
- PennTreebank \[[notebook](./PennTreebank/visualization.ipynb)\] \[[code](./PennTreebank)\]

## Future Work

We will keep updating the demos in the near future to include more popular benchmarks.
Feel free to leave an issue or send an email to the first author ([Wuqi Liang](mailto:liangwuqi@ahtvu.ah.cn))
if you want to see a specific task which has not been included yet. :D
