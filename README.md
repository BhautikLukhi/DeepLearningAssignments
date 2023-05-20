Assignment 1

To compare the effects of different activation functions using the Fashion MNIST dataset, we built a simple neural network model using TensorFlow and
Keras. We investigated the learning and generalization behavior of the model using
the following activation functions: ReLU (Rectified Linear Unit), SELU (Scaled Exponential Linear Unit), and Tanh (Hyperbolic Tangent). For model architecture, we
used 2 Convolutional layers with max pooling on the first two layers and ReLU, SELU
and tanh as activation function. Also, in the ouput layer, we used softmax activation.
For optimizer, we went for Adam instead of SGD(), because Adam tends to converge
faster. For the comparison of accuracy for different activation functions (refer to 2nd
figure on next page). ReLU is computationally efficient and helps mitigate the vanishing gradient problem but may suffer from dying neurons. SELU has self-normalizing properties and can improve training performance but may be sensitive to initialization
and architecture choices. Tanh is fully differentiable and doesn’t suffer from the dying problem but can be prone to vanishing gradients in deep networks. The choice of activation function depends on the specific problem and architecture being used.


Assignment 2

Part 1: We trained a VAE on the Fashion MNIST dataset.To accomplish this task, we first
preprocessed the data by normalizing and reshaping the images. Next, we built a VAE model consisting
of an encoder and a decoder. The encoder maps the input images into a lower-dimensional latent space,
while the decoder reconstructs the images from the latent space representation. After training the
model, we assessed the reconstruction error (last row of figure), which gives an indication of how well
the VAE can recreate the input images. We also displayed typical results of generated images (first
row of fig) by sampling from latent space and decoding samples using trained VAE. These images
demonstrated the quality of the representations learned by the VAE. Furthermore, we performed
latent space interpolation between pairs of data points, both within a class and between different
classes (row 2nd and 4rd of fig). This experiment revealed the smooth transitions between data points
in the latent space, highlighting the VAE’s ability to capture the underlying structure and generate
meaningful interpolations between data points.
Part 2: We now generated GAN on same dataset. We normalised and reshaped the images.
Then, we built a GAN model consisting of a generator and a discriminator. The generator creates
fake images from random noise, while the discriminator tries to differentiate between real and fake
images. We assessed the quality of the generated images by visually examining the samples generated
by the GAN after training (see fig 4). The images demonstrated the ability of the GAN to create
realistic representations of the Fashion MNIST dataset. The adversarial training process resulted in
a generator capable of producing images that resemble the original dataset.
