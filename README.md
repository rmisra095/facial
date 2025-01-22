# CAIS++ Winter Project

Nutshell: Machine learning model to classify facial expressions into seven emotions—Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral—using the FER-2013 dataset of 48x48 grayscale images. 

Dataset: I chose the FER-2013 dataset because it provides a large number of labeled images and is well-suited for this task. Before training, I resized the images to 48x48 pixels, normalized the pixel values to improve training, and applied data augmentation like flipping and rotating the images. These steps made the dataset more diverse and helped the model generalize better.

Model Development and Training: I designed a convolutional neural network (CNN) with three convolutional layers, followed by pooling, batch normalization, and fully connected layers. I trained the model for 10 epochs using the Adam optimizer and a cross-entropy loss function. I chose these settings because they are effective for image classification tasks like this.

Model Evaluation/Results: To evaluate the model, I used accuracy and a confusion matrix to see how well it classified the emotions. The model achieved an accuracy of about 65% on the test set, when intially run. However, now it performs with an accuracy of 100%. This is definitely a problem, but intially the loss steadily decreased across the 10 epochs. It performed well on clearer emotions like Happy and Surprise but struggled with more difficult ones like Disgust. 

Discussion: I think the dataset and model worked well together for this project, but there were some challenges. The dataset had fewer images for some emotions, like Disgust, and the small image size made it harder for the model to capture details. This project can definitely be extended to wider applications including national security measures and determining weather or not certain emotions are more associated with certain crimes. 
