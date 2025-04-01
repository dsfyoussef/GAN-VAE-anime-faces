Variational Autoencoder with GAN Discriminator


This project implements a Variational Autoencoder (VAE) with a Generative Adversarial Network (GAN) discriminator to generate realistic anime-style face images. The model combines the advantages of VAEs for structured latent space learning and GANs for improved image generation quality.

Project Structure

Encoder: Extracts features from input images and outputs a latent representation (mean and variance).

Sampling Layer: Generates latent vectors using the reparameterization trick.

Decoder: Reconstructs images from the latent space.

Discriminator: A CNN-based classifier that distinguishes between real and generated images.



Dataset: The model is trained on an anime face dataset extracted from a ZIP file stored in Google Drive. The dataset is preprocessed by resizing images to 64x64 pixels and normalizing pixel values to [-1, 1].


Load Dataset: Extract and preprocess images.

Train Discriminator: Classifies real vs. generated images.

Train Generator (VAE): Optimized with adversarial and reconstruction losses.

Iterate for Multiple Epochs: The model gradually improves image quality.

Requirements:

-TensorFlow & Keras

-NumPy

-Matplotlib

-Google Drive access (for dataset)

-OpenCV


Expected Output

After sufficient training, the model should generate anime-style faces that resemble the training data, improving over time through adversarial training.
