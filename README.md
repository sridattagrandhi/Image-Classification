# Image-Classification

Model: 
The model used for this project is a Vision Transformer (ViT) with dropout and partial freezing. Specifically, it is based on the vit_b_16 architecture from torchvision.models. The classification head has been modified with a dropout layer (p=0.5) before the final linear layer.
Some encoder layers (8-11) and the classification head remain trainable while other parameters are frozen.
MixUp data augmentation is applied to improve generalization.

Environment: 
The following Python libraries are required for this project:
torch
torchvision
numpy
pandas
PIL (Pillow)
tqdm
Sklearn

Usage: 
To run the model, follow these steps:
Set up the environment:
  1. Run this command in terminal to install the required libraries:
        pip install torch torchvision timm numpy pandas pillow
  2. Prepare the dataset: Ensure the training images are in the train/train directory.
  3. Run the script: Execute the model training and evaluation.
