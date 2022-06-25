# Super-Image-Resolution

#### BSDS500 Dataset for training and Set5 Dataset for the testing 
https://drive.google.com/drive/folders/13yWa0-mXJATPzgMrwad7y2CrlH73myJt?usp=sharing

Four different interpolation methods, to convert images into low resolutions and then rescontruct them,are implemented
Autoencoder model is used for training and validation purposes. We train our low-resolution images using the autoencoder model. Autoencoders like the denoising autoencoder can be used for performing efficient and highly accurate image denoising. Unlike traditional methods of denoising, autoencoders do not search for noise, they extract the image from the noisy data that has been fed to them via learning a representation of it. The representation is then decompressed to form a noise-free image.Denoising autoencoders thus can denoise complex images that cannot be denoised via traditional methods.

#### Encoder Architecture
5 Conv2D layers 
2 Max Pooling layers.
#### Decoding Architecture
2 Up sampling Layers.
5 Conv2D Layers
Other Parameters
Activation function: Relu
Kernel Initializer: Glorot Uniform

#### Training and Validation Losses


#### Comparasion Between output and Input 
![image](https://user-images.githubusercontent.com/104934568/175793013-adb6f9ec-6465-48bf-b861-298da531e737.png)

#### Deciding Factor PNSR
PNSR is increased between 2 to 7
#### Conclusion
Image super resolution is challenging but it is an interesting task. In this task, image super resolution by degrading the image with multiple interpolation methods and then reconstructing the image using our denoising autoencoder model is implemended . The results were quite significant as the shown in the comparison with increase in PNSR score of reconstructed images and decrease in their mean squared error.
![image](https://user-images.githubusercontent.com/104934568/175792891-af9ccf90-3c1d-4b54-bdc2-3dbfd6d78b5f.png)





















##### References
https://towardsdatascience.com/image-super-resolution-using-convolution-neural-networks-and-auto-encoders-28c9eceadf90
