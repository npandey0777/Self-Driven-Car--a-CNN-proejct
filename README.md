# Self-Driven-Car--a-CNN-proejct
In this project, around 45000 frontal images taken while driving the car are provided, along with the appropriate steering rotation. Each image's width and height are 455 and 255 pixels, respectively. The analysis will be performed to train the model to suggest the correct steering rotation taken by the car.
## Motivation
• The increased use of automobiles has resulted in a significant increase in road accidents.
• Self-driving cars have become a myth of the past.
• Cars learn through images to drive safely, avoiding mistakes and wrong turns. Optimize fuel composition by predicting the accurate 
steering angle.
## Problem Statement 
• The main objective of the project is to predict the required steering wheel angle for safe navigation of a car without human intervention
based on the model trained with a series of images and their respective steering wheel angles.
• The images consist of road lanes, traffic signals, diverse weather conditions, etc.
## Research questions
• Automated steering control system to reduce human errors using Convoluted Neural Network (CNN) model.
• Selecting the model that can provide results with good accuracy and improve them for new cases is key
## Data
• The data consists of images of road lanes and signals and a text file
containing steering rotation information for each image.
• There are 45000 images with a resolution of 455 x 256 pixels in 
total.
• The image dataset has more than 80% of the images being of road
lanes, followed by signs and signal images.
• The steering wheel angle (degree) is the target variable, where
positive and negative values represent right and left steering,
respectively.
• Images in the dataset cover shadow, low light, and bright light
conditions.
## Approach
• A CNN model is used to predict the steering rotation.
• The model was developed using the TensorFlow framework.
• The CNN model architecture is as follows:
• A normalization layer.
• 5 convolution layers with weight values normally distributed.
• 3 fully connected layers.
• The model was trained on 80 percent of the 45000 images and tested
on 20 percent.
• The optimized model performance is compared with pre-trained
models (VGG, inception, ResNet).
# Final Results and Key Findings
• The goal of the model is to predict the appropriate steering angle based on the image. We used two approaches to design the model.
• First, we created our own CNN architecture (layers) and optimized it.
• Second, the transfer learning method is utilized for training the model. The state-of-the-art trained CNN models are used to classify the images in
this technique. Later on, fully connected layers are appended to predict the final output. The following pre-trained model is used for the project:
• VGG16
• RESTNET50
• INCEPTIONV3
## Final Results: The final results based on the two approaches are given below
Key Findings
• VGGNET16 gave the least Test and Train error, but the processing time was relatively high when compared to INCEPTIONV3.
• INCEPTIONV3 runs in the least time and has relatively good test and train accuracy error.
• Regularization helped reduce the test error in optimized model, but it wasn’t good enough compared to the pre-trained model.
• Based on the run time and errors, VGGNET16 comes out to be the best model for the project
