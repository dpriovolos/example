# Face to Sketch and Sketch to Face using Deep Autoencoders

This project involves the development of a deep autoencoder using Python Keras and Tensorflow libraries, with the purpose to accurately convert face images with specific backround to sketches and the opposite. There are 3 models displayed. One fully Dense layers autoencoder, one autoencoder created with convolutional layers (CNN) and one original model created by combining those two types of layers. In between those layers some other layers are used like Pooling layers and Dropout layers for regularization. The project uses the publicly available data set CUHK Sketch Database (CUFS) that can be found in Kaggle. 

The expected results for the Face 2 Sketch project for each models are:
<img width="550" alt="Face 2 sketch" src="https://user-images.githubusercontent.com/108266112/191847566-b4cc8082-9dc3-4fa7-bb02-275f918cd6e2.png">

The expected results for the Sketch 2 Face project for each models are:
<img width="540" alt="Sketch 2 face" src="https://user-images.githubusercontent.com/108266112/191848981-89795636-9b59-49c6-8f4c-b4e2e2a327e1.png">

The models' performance was judged by the following metrics.

| Similarity   Measures | Dense AE | Convolutional AE | Self-Implemented   AE |
|:---------------------:|:--------:|:----------------:|:---------------------:|
|      Average MAE      |   0.162  |       0.171      |          0.15         |
|      Average RMSE     |   0.266  |       0.274      |         0.269         |
|      Average SSIM     |   0.642  |       0.739      |         0.727         |

Table: FACE TO SKETCH SIMILARITY MEASURES FOR EACH MODEL

| Similarity   Measures | Dense AE | Convolutional AE | Self-Implemented   AE |
|:---------------------:|:--------:|:----------------:|:---------------------:|
|      Average MAE      |   0.064  |       0.051      |         0.055         |
|      Average RMSE     |   0.136  |       0.121      |          0.13         |
|      Average SSIM     |   0.735  |       0.824      |         0.801         |

Table: SKETCH TO FACE SIMILARITY MEASURES FOR EACH MODEL
