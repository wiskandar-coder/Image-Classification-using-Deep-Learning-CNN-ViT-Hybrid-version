# Image Classification using Deep-Learning CNN-ViT Hybrid version
This project is an extent of a previous projet https://github.com/wiskandar-coder/Image-Classification-using-Deep-Learning-CNN-version, and consists of classifying images of dogs using hybrid Convolutional Neural Network (CNN) and Vision Transformer (ViT). I will compare between a pure CNN architecture and a hybrid architecture CNN+ViT. For that, I will use Stanford Dogs Dataset http://vision.stanford.edu/aditya86/ImageNetDogs/ containing 20580 images of dogs distributed on 120 dog breeds.

![image](https://github.com/wiskandar-coder/Image-Classification-using-Deep-Learning-CNN-version/assets/64427335/e7d01161-4122-45e3-b300-19bdaa9fde2a)

- Finding an hybrid model that is optimum in predicting time and accuracy score for the image resolution used in the project
- Pre-treatment and preparation for the modelisation in 'code':
    - Put all images at the same resolution
    - Transforming all images to RGB
    - Image augmentation using random horizontal flip , random rotation in +-30 degrees, random luminosity in +-25%, and random contrast in +-25%
    - Normalization of the color values in each pixel
    - Dividing the images into 490 batches (42 images/batch)
    - Dividing the batches into 80% train, 10% validation, and 10% test
  
- Modelisation in 'code'
    - I did use pretrained ResNet-50 as the pure CNN and pretrained MaxxViT-v2-Base as the hybrid CNN-ViT for the comparaison
    - First, training the final layer to adapt to the 120 dog breeds
    - Second, trying to optimize the models by training more layers at the end of the models architecture and using augmented images
    - Check the performance of the model using the train and validation accuracy and loss on each step, and finally the prediction time, test loss and test accuracy on the model that give the best validation accuracy and loss

A powerpoint presentation of the project can be shared under request.
