# Image-Segmentation
Trying this Kaggle competition : https://www.kaggle.com/c/tgs-salt-identification-challenge/overview

# U-Net
U-Net is a type of convolutional neural network (CNN) that is specifically designed for image segmentation tasks. It was developed by Olaf Ronneberger, Philipp Fischer, and Thomas Brox in 2015 at the University of Freiburg, primarily for biomedical image segmentation. The network's architecture and performance have made it a popular choice for various image segmentation problems beyond the biomedical field.

The U-Net architecture consists of two main parts :

1. Contracting Path (Encoder):
    - This part of the network is similar to a traditional CNN.
    - It consists of a series of convolutional layers, each followed by a rectified linear unit (ReLU) and a max pooling operation.
    - As the data flows through the contracting path, the spatial dimensions of the feature maps are reduced while the depth (number of feature channels) increases.
    - This path is responsible for capturing the context and features of the input image.

2. Expanding Path (Decoder):
    - This part of the network is designed to upsample the feature maps back to the original image size.
    - It consists of upsampling operations (usually transposed convolutions) followed by convolutional layers and ReLU activations.
    - Skip connections from the contracting path are introduced at each level, allowing the network to utilize fine-grained information that was captured during the downsampling process.
    - These skip connections help the network to better reconstruct the details of the segmented image.

https://www.youtube.com/watch?v=NhdzGfB1q74&t=514s
https://towardsdatascience.com/understanding-semantic-segmentation-with-unet-6be4f42d4b47

All credits go to hlamba28 and Birinder1469.
