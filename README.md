**Conditional GAN Implementation for MNIST Dataset**

This repository contains a PyTorch implementation of a conditional generative adversarial network (cGAN) designed to generate images of handwritten digits from the MNIST dataset, conditioned on class labels.

**Key Features:**

- **Conditional GAN architecture:** The model employs a discriminator and a generator, both conditioned on class labels, to enable control over the generated images.
- **Gradient penalty:** Implements a gradient penalty to improve training stability and prevent model collapse.
- **TensorBoard integration:** Uses TensorBoard to visualize training progress and generated images.
- **Clear code structure:** The code is well-organized into separate modules for model definitions, utility functions, and training.

**Files:**

- **model_conditional_GAN.ipynb:** Contains definitions for the discriminator and generator models.
- **utils_2.py:** Houses the gradient penalty function.
- **train_conditional_GAN.ipynb:** Performs the training process, including data loading, model setup, optimization, and logging.

**Running the Code:**

1. Ensure you have Python and required libraries installed (`torch`, `torchvision`, `tensorboard`).
2. Run the `train_conditional_GAN.ipynb` notebook to initiate training.
3. Monitor progress and generated images using TensorBoard:
   - Open a terminal and navigate to the repository directory.
   - Run `tensorboard --logdir logs`.
   - Access TensorBoard at `http://localhost:6006` in your browser.

**Research Paper:**

- This implementation is based on the research paper "Conditional Generative Adversarial Nets": [https://arxiv.org/pdf/1411.1784](https://arxiv.org/pdf/1411.1784)

**Additional Notes:**

- Hyperparameters can be adjusted in the `train_conditional_GAN.ipynb` notebook to experiment with different settings.
- The code can be adapted to work with other datasets and conditional settings.
