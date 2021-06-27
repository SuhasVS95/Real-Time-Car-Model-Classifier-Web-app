# CLASSIFICATION OF CAR MODELS USING COVOLUTIONAL NEURAL NETWORK (TRANSFERLEARNING|DEPLOYMENT)

This is an end to end image classification deep learning project from data collection to deployment as a web app.

# Problem Statement:

According to the study conducted by "Mordor Intelligence" on the Indian used car market was valued at USD 27 billion in 2020, and it is expected to reach USD 50 Billion by 2026. Link to the article: https://www.mordorintelligence.com/industry-reports/india-used-car-market

Sometimes when people see any car on the road and like it but not sure of the model to further enquire about it, then they can take a snap of it and use our app link to know about the car model. They can consult the used cars dealership.

Classification of images of the cars to their respective labels using Deep Learning Techniques.

# Class Labels:

Creta
Innova
Nano
Scorpio
Range Rover

# Project Pipeline/Work Flow:

1. Data Collection(Web Scraped)
2. Image Visualization with their class labels
3. Model Building
 3.1 Base Model(CNN Based)<br>
 3.2 Model 1(CNN + Image Augmentation)<br>
 3.3 Model 2(CNN +Image Augmentation + Batch Normalization)<br>
 3.4 Model 3(CNN + Image Augmentation + Drop Out)<br>
 3.5 Final Model(Transfer Learning + callbacks)<br>
4. Visualize the predictions
5. Analysis of the accuracy and loss of all the models built
6. Deployment

**Steps to handle overfitting:**

1. Use of Image Augmentation to make the model learn of the different versions of the training data.
2. Use of L1/L2 regularization, Drop out, Batch Normalization.
3. Use of callbacks such as Early Stopping.
4. Varying the learning rate of the optimizer.

**Steps taken to arrive at the best and final model:**

1. Use of pre-trained weights from MobileNet for the 70 convolutional layers.
2. Open up covolutional layers from 71st layer to train with a dense hidden layer of 512 neurons.
3. These layers account for optimization of weights through backpropagation.
4. Use of GlobalAveragePooling2D.
5. Use of "adam" optimizer.
6. Use of callbacks(EarlyStopping, ModelCheckpoint, CSVLogger).

# Comparison of all the models

![image](https://user-images.githubusercontent.com/70081663/123543802-e945b980-d76d-11eb-86f9-6abd934d6ac4.png)

# Visualize the predictions

![image](https://user-images.githubusercontent.com/70081663/123543824-09757880-d76e-11eb-9a8e-705410e8a7e0.png)


