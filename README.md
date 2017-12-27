# Adversarial Attacks

Adversarial attacks are types of malicious attacks that are aimed at making machine learning classifiers misclassify. The phenomenon was discovered by [Szegedy et al.](https://arxiv.org/abs/1312.6199) in 2014, and it continued to attract the interest of researchers ever since. 

In the context of image classification, these attacks are in the form of adding non-random noise to the images to be classified.

This repository explores the attacks and applies JPEG and JPEG2000 compression techniques as a defensive tool. Further defenses will be added in the future and this repository will be updated accordingly. Initial choice of JPEG and JPEG2000 compression is based on [this work](https://arxiv.org/abs/1608.00853)

To generate the attacks, [Cleverhans](https://github.com/tensorflow/cleverhans) library is used.
Most of the code in this repository is modified from NIPS Adversarial Attacks Tutorial in the Cleverhans library.

The code in this repository mainly uses the following libraries:

- [Tensorflow](https://github.com/tensorflow)
- [Scikit Image Library](http://scikit-image.org/)
- [Python Image Library (PIL)](https://pillow.readthedocs.io/en/4.3.x/)
- [Celeverhans](https://github.com/tensorflow/cleverhans)

Note that for some of the code in this repository to work, PIL must be built from source with JPEG2000 support. In order to do this, OpenJPEG library version 2.1+ is needed. The instructions to build these libraries for Linux systems is given in the PIL and OpenJPEG documentations respectively. If you don't want to use JPEG2000 compression you need to comment out or remove JPEG2000 compression in the code. If you don't want to use JPEG2000, you can use PIL out-of-the-box.

The code in this repository uses Tensorflow as the deep learning framework. The code explicitly specifies the use of an Nvidia GPU. However, it could also be made to use a CPU as described in [Tensorflow documentation](https://www.tensorflow.org/tutorials/using_gpu).

For any questions or comments, please send an [e-mail](aelvanaydemir@gmail.com) or send a [tweet](https://twitter.com/L1_norn).



