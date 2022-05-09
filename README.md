# CAECompressionSWinIRRestoration
This project improves the image compression and restoration when sent over internet.

Compression
It uses Convolutional Autoencoder with three convolutional layers each in encpder and decoder to compress and decompress the image.
It is compared with JPEG compression and evaluated using PSNR and SSIM.

Steps to run the Compression Code:
Run CAE.ipynb file

The CAE file will download CIFAR10 dataset and train the model on it and test it.
In order to test your own image, Upload the image from google drive and then mount the drive on google colab.
Load the image in the notebook. Convert the image in the format of fixed_input variable and run the file.

The images reconstructed from the CAE code will be saved and used in the SwinIR model.
Steps to run the Restoration code:

