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

Steps to run the restoration Code:
Running restoration is divided into two steps. Train and test. 
Steps to run test for restoration:
1. Download SwinIR code from https://github.com/JingyunLiang/SwinIR  
2. Change to directory you have stored SwinIR project in
3. Download model_weights.pth
4. Move model_weights.pth to Desktop/new_model/ 
5. Save the images you want to test on in Desktop/test/
6. Create desktop/result folder
7. Open https://github.com/AditiAgrawal95/CAECompressionSWinIRRestoration/blob/main/ImageRestoration/SwinIR_SR_Transfer_Learning.ipynb in colab
8. Connect colab to your local
9. Run JUST the last step
10. Check result in result folder

Steps to run train code:
1. Download SwinIR code from https://github.com/JingyunLiang/SwinIR 
2. Change to directory you have stored SwinIR project in
3. Save the images you want to train on in Desktop/train/
4. Save the images you want to validate on in Desktop/validation/
5. Create Desktop/new_model/
6. Open https://github.com/AditiAgrawal95/CAECompressionSWinIRRestoration/blob/main/ImageRestoration/SwinIR_SR_Transfer_Learning.ipynb in colab
7. Connect colab to your local
8. Run all the steps in colab sequentially other than lat step (Last step is for testing the model new model)
