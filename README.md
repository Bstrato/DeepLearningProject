# CIFAR-10 Classification with ResNet-14

This project implements and trains a ResNet-14 architecture on the CIFAR-10 dataset using PyTorch, with extensive visualization and performance tracking via TensorBoard.

**Highlights**
- Model Architecture: A custom ResNet-14 built from scratch, based on He et al. (2015) https://arxiv.org/pdf/1512.03385, comprising 3 stages of residual blocks with batch normalization and ReLU activation.

**Dataset:**
- CIFAR-10, with standard data augmentation (random cropping, horizontal flipping) and normalization.

**Training Setup:**
- Optimizer: Adam
- Loss: Cross-Entropy
- Epochs: 30
- Device: CUDA/CPU

**Visualization:**
- Real-time logging of training/test accuracy, loss curves, PR curves, parameter histograms, and embedding projections using TensorBoard.

**Performance:**
- Achieved up to 87.8% test accuracy after tuning with adaptive learning rate scheduling using ReduceLROnPlateau.

**Tuning:**
- Integrated a dynamic LR scheduler to improve convergence without manual intervention.
