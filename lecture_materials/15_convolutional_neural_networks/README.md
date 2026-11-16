# Convolutional Neural Networks

Live teaching materials from the CNN classes taught on 31 October, 1 November, 14 November, and 15 November 2026.

## Lecture Materials

### Lecture 23 - CNN Theory - 31 October 2026

- `notes/23_convolutional_neural_networks_theory_live_notes.pdf`
- Why image structure motivates convolutional neural networks.
- Local connectivity, parameter sharing, translation equivariance, kernels, feature maps, padding, stride, channels, pooling, receptive fields, and complete CNN architecture.

### Lecture 24 - CNN Coding - 1 November 2026

- `notebooks/24_convolutional_neural_networks_coding_live.ipynb`
- A spelled-out implementation that starts with images as tensors and calculates convolution directly.
- Applies Sobel, blur, and sharpening kernels, then trains a convolutional layer to learn a Sobel-style feature detector.
- Builds and trains a small PyTorch CNN on CIFAR-10 and inspects its learning curves, confusion matrix, and confident mistakes.

### Lecture 25 - CNN Training and Generalization - 14 November 2026

- `notebooks/25_cnn_training_and_generalization_live.ipynb`
- Establishes a small CIFAR-10 CNN as a baseline and verifies the initial multiclass loss.
- Adds normalization, data augmentation, Batch Normalization, dropout, a learning-rate scheduler, early stopping, and best-checkpoint restoration.
- Compares baseline and improved training through loss, accuracy, and learning-rate curves.

### Lecture 26 - Modern CNN Architectures (Theory) - 15 November 2026

- `notes/26_modern_cnn_architectures_theory_live_notes.pdf`
- Connects early CNNs to the design ideas behind modern architectures.
- Covers ImageNet context, influential architecture families, residual learning, efficient building blocks, $1\times1$ convolution, and depthwise separable convolution.

> **Coverage status:** Transfer learning was not covered in Lecture 26. It will be added after it is taught in a future class.

## Topics Covered

- Images as structured tensors and why flattening loses spatial relationships.
- Cross-correlation and convolution calculated with sliding local windows.
- Hand-designed Sobel, blur, and sharpening filters.
- Learning convolutional filters through backpropagation.
- Padding, stride, channels, feature maps, pooling, receptive fields, and parameter counts.
- Building and evaluating a compact PyTorch CNN on CIFAR-10.
- Improving CNN training with normalization, augmentation, Batch Normalization, dropout, scheduling, early stopping, and checkpointing.
- ImageNet and the progression of influential CNN architectures.
- Residual learning and efficient CNN operations, including $1\times1$ and depthwise separable convolutions.

## Dataset Note

The coding notebooks use CIFAR-10. Follow their dataset setup cells before creating the PyTorch data loaders; the newer training notebook can obtain CIFAR-10 through the Hugging Face `datasets` library.
