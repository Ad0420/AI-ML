# AI-ML

Advik Unni 
aunni@usc.edu

Project:
My project used transfer learning as well as computer vision classification to distinguish between muffins and chihuahuas.

Pre-Processing steps:
I took my dataset from kaggle. They had a good dataset on muffins and chihuahuas that were split between 2 folders. 
I downloaded the dataset and then uploaded it onto google co-labs.
I created labels for the dataset and then moved all the images into one folder.
I resized the images to a 224 x 224 frame when I moved them.
This was because 224 * 224 is the standard image size for the Transfer Learning model that I was using.
After that, I converted the images into a numpy array and split a 80/20 Train-Test split.

Model Training
I used the pre-trained MobileNetV2 model for this project.
I chose this model as it's used for image classification so I felt it would be a good place to start.
I used a standard optimizer ‘Adam’ in my model.
The total number of parameters were 2,260,546 out of which there were 2,562 trainable parameters.
I imported Tensorflow and tensorflow hubs and used it to help code the loss function.

Model Results
I trained the model on 5 epochs before testing.
The training data had a loss function of 0.655 and an accuracy score of 0.6099.
The testing data had a loss function of 0.781 and an accuracy score of 0.4723.

Discussion
The model did not have the best results. Since I am new to transfer learning, I may have not used the correct pre-trained model or not frozen proper layers.
If I were to continue this project, I would dive deeper into different models and learn how to and where to freeze layers.

