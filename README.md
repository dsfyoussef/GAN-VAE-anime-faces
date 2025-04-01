Variational Autoencoder with GAN Discriminator


This project implements a Variational Autoencoder (VAE) with a Generative Adversarial Network (GAN) discriminator to generate realistic anime-style face images. The model combines the advantages of VAEs for structured latent space learning and GANs for improved image generation quality.

Project Structure:

-Encoder: Extracts features from input images and outputs a latent representation (mean and variance).

-Sampling Layer: Generates latent vectors using the reparameterization trick.

-Decoder: Reconstructs images from the latent space.

-Discriminator: A CNN-based classifier that distinguishes between real and generated images.



Requirements:

-TensorFlow & Keras

-NumPy

-Matplotlib

-Google Drive access (for dataset)

-OpenCV


Expected Output

After sufficient training, the model should generate anime-style faces that resemble the training data, improving over time through adversarial training.
