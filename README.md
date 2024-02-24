### Description

This project is an implementation of a deep learning model for brain tumor segmentation using the UNet architecture. The goal is to accurately identify and delineate brain tumors in MRI images. The UNet architecture is chosen for its ability to capture fine-grained details while maintaining spatial context, which is crucial for accurate segmentation.

### Background
MRI images are widely used for diagnosing brain tumors. However, manually segmenting these tumors is a time-consuming and challenging task. Deep learning models, particularly the UNet architecture, have shown promising results in automating this process.

## UNet Architecture

The UNet architecture was proposed by Olaf Ronneberger, Philipp Fischer, and Thomas Brox in their paper U-Net: Convolutional Networks for Biomedical Image Segmentation. It consists of a contracting path (encoder) and an expansive path (decoder), which are connected by a bottleneck layer.

### Contracting Path (Encoder)
The contracting path is similar to a traditional convolutional neural network (CNN) and is designed to capture context. It consists of a series of convolutional and pooling layers that gradually reduce the spatial dimensions of the input image while increasing the number of feature channels.

### Bottleneck Layer
The bottleneck layer is the deepest layer of the network and serves as a bridge between the contracting and expansive paths. It contains a series of convolutional layers that further capture context and spatial information.

![unet_architecture](https://github.com/YugantGotmare/UNet-Enhanced-Brain-tumor-Segmentation/assets/101650315/6b0911e7-45a8-4848-ad80-bb14464422c8)


Results:



![output2](https://github.com/YugantGotmare/UNet-Enhanced-Brain-tumor-Segmentation/assets/101650315/72000151-ce5a-4244-bb0e-38d3e13eff63)




![output3](https://github.com/YugantGotmare/UNet-Enhanced-Brain-tumor-Segmentation/assets/101650315/b540e77f-54c4-42f7-99e8-8cc67e8ddcc2)
### Expansive Path (Decoder)
The expansive path is designed to localize details and generate the final segmentation mask. It consists of a series of upsampling and convolutional layers that gradually increase the spatial dimensions of the input while reducing the number of feature channels. Skip connections from the contracting path are used to preserve spatial information and aid in the reconstruction of the segmentation mask.


