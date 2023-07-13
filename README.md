# Assignment 1

To compare the effects of different activation functions using the Fashion MNIST dataset, we built a simple neural network model using TensorFlow and
Keras. We investigated the learning and generalization behavior of the model using
the following activation functions: ReLU (Rectified Linear Unit), SELU (Scaled Exponential Linear Unit), and Tanh (Hyperbolic Tangent). For model architecture, we
used 2 Convolutional layers with max pooling on the first two layers and ReLU, SELU
and tanh as activation function. Also, in the ouput layer, we used softmax activation.

# Assignment 2

Part 1: We trained a VAE on the Fashion MNIST dataset, we performed
latent space interpolation between pairs of data points, both within a class and between different
classes (row 2nd and 4rd of fig). This experiment revealed the smooth transitions between data points
in the latent space, highlighting the VAE’s ability to capture the underlying structure and generate
meaningful interpolations between data points.  

Part 2: We now generated GAN on same dataset. The images demonstrated the ability of the GAN to create
realistic representations of the Fashion MNIST dataset. The adversarial training process resulted in
a generator capable of producing images that resemble the original dataset.


# Assignment 3

We trained CNN on MNIST data set and performed 3 different attacks as following.

1.Fast Gradient Sign Method(FGSM)

2.Deep Fool

3.Adversarial Examples via Transformation-Based Error Feedback(ABBA).

# Assignment 4

We trained CNN on fashion MNIST dataset and used Explanation methods such as LIME, DeepLIFT anf Saliency map to find out how the Deep model makes a perticular decision.
