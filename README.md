# Image Generation using Autoencoder

PyTorch project for MNIST image reconstruction and generation using a convolutional autoencoder.

## What this project does

- Loads MNIST with `torchvision`
- Trains a CNN autoencoder with latent size 8
- Plots training loss
- Shows original vs reconstructed images
- Generates new images from random latent vectors

## Files

- `image_generation_AE_MNIST.ipynb`: full workflow (data, model, train, plots, generation)

## Quick start

```bash
python -m venv venv
source venv/bin/activate
pip install torch torchvision matplotlib numpy tqdm jupyter
jupyter notebook image_generation_AE_MNIST.ipynb
```

## Training setup

- Loss: MSE
- Optimizer: AdamW (`lr=1e-4`)
- Batch size: 64
- Epochs: 20
- Latent dimension: 8

