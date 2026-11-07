# Convolutional Neural Networks

Live teaching materials from the CNN theory and coding classes taught on 31 October and 1 November 2026.

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

## Topics Covered

- Images as structured tensors and why flattening loses spatial relationships.
- Cross-correlation and convolution calculated with sliding local windows.
- Hand-designed Sobel, blur, and sharpening filters.
- Learning convolutional filters through backpropagation.
- Padding, stride, channels, feature maps, and parameter counts.
- Max pooling and spatial downsampling.
- Building a compact CNN using `nn.Conv2d`, ReLU, pooling, flattening, and a linear classifier.
- Train, validation, and test workflows for image classification.
- CIFAR-10 evaluation using accuracy and a confusion matrix.
- Error analysis through confidently misclassified images.

## Dataset Note

The coding notebook expects the CIFAR-10 dataset in the runtime environment. Follow its dataset setup cells before creating the PyTorch data loaders.
