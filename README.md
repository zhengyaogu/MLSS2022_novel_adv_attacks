# Novel Adversarial Attacks (Final Project for the Machine Learning Safety Scholar program, 2022)

## Overview

In this final project for MLSS, we proposed LocalBlur, a localized masking method that blurs important parts of an image in order to fool the classifier; Pullback, a new `L_p` attack that computes the gradient on an image before it is transformed by common image distortion techniques; and finally `mu-delta`, which shifts the center and variance of the data distribution to fool the network.

## Instructions

The deliverable content is in `novel_adversarial_attack.ipynb`, whose successful running depends on the `save` and `data` folder.
To download those two folders, first install `gdown`

```
pip install gdown
```
Then, run `setup.sh`.

***\*CAUTION\****: one should modify the next block to accommodate their own Google Drive directory structure. This Colab Notebook would only work if the accompanying data are positioned in the right place. The structure of your project folder should be

\```

<project folder>

---> <this notebook>

---> <data> # where CIFAR10 and CIFAR100 as well as adversarial data are stored

---> ---> <adv10.pt> # adversarial training set for CIFAR10

---> ---> <adv100.pt> # adversarial training set for CIFAR100

---> <save> # where the trained models are stored

---> ---> <cifar10.pt> # trained CIFAR10 model

---> ---> <cifar100.pt> # trained CIFAR100 model

---> ---> <adv10.pt> adversarially fine-tuned CIFAR10 model

---> ---> <adv10.pt> adversarially fine-tuned CIFAR10 model

\```



The Colab Notebook is written under a subscription to Colab Pro+. If you encounter GPU RAM shortage, I reccomend subscribing first.