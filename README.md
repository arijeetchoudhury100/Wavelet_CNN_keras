# Wavelet_CNN_keras
This repo contains the implementation of wavelet based CNN in keras, translated from pytorch.
The original pytorch implementation can be found in https://github.com/LiQiufu/WaveCNet

paper link:
https://openaccess.thecvf.com/content_CVPR_2020/papers/Li_Wavelet_Integrated_CNNs_for_Noise-Robust_Image_Classification_CVPR_2020_paper.pdf

## The DWT_Pooling layer can be used inplace of MaxPooling for noise robust image classification

# Example usage
#### model = Sequential([
####  Conv2D(16,(3,3),padding='same',activation='relu'),
####  DWT_Pooling(),
####  Conv2D(32,(3,3),padding='same',activation='relu'),
####  DWT_Pooling(),
####  Flatten(),
####  Dense(2,activation='softmax')
#### ])

### The notebook also contains MNIST digit classification as an example.
