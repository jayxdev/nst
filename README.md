# NST (Neural Style Transfer)

This project implements Neural Style Transfer using TensorFlow and the VGG19 model.

## Overview

Neural Style Transfer is a technique that combines the content of one image with the style of another image using deep neural networks. This implementation uses the VGG19 model pretrained on ImageNet as the feature extractor.

## Features

- Utilizes the VGG19 model for feature extraction
- Allows selection of specific VGG19 layers for style and content representation
- Implements a custom model that outputs intermediate layer activations

## Requirements

- TensorFlow
- Python 3.x

## Usage

The main functionality is implemented in the `vgg_layers` function, which creates a modified VGG19 model that returns intermediate layer outputs.

```python
from main import vgg_layers

# Specify the layers you want to extract features from
layer_names = ['block1_conv1', 'block2_conv1', 'block3_conv1', 'block4_conv1', 'block5_conv1']

# Create the model
model = vgg_layers(layer_names)```

## Contributing
Contributions to improve the project are welcome. Please feel free to submit a Pull Request.

## License
[Add your chosen license here]


