# Toy autoencoder

The definition of an autoencoder from [Wikipedia](https://en.wikipedia.org/wiki/Autoencoder):

> An autoencoder is a type of artificial neural network used to learn efficient codings of unlabeled data (unsupervised learning). An autoencoder learns two functions: an encoding function that transforms the input data, and a decoding function that recreates the input data from the encoded representation. 

This notebook implements, in some sense, the simplest possible autoencoder: one that tries to reconstruct an arbitrary high-dimensional vector from a lower-dimensional internal representation. Specifically, it converts a 100-dimensional input vector to a 10-dimensional encoding, then attempts to reconstruct the original 100-dimensional vector from the 10-dimensional encoding.

We train and test on random data, so we get absolutely awful test accuracy (~8%). But if we used more structured data, such as [MNIST images](https://en.wikipedia.org/wiki/MNIST_database), we would get much better performance &mdash; the model would have actual features to represent as directions in a lower-dimensional space, as opposed to just high-entropy random noise.

![image](https://github.com/user-attachments/assets/786e0dc8-7290-418c-9ec7-60f95cc5534a)
