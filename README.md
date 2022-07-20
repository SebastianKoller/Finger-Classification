# CP468 Fingers Classification
7/17/2022
## Description
AI project for CP468 at Wilfrid Laurier University with Professor Sukhjit Sehra.
### Objective
Train a Convolutional Neural Network to be able to classify images in the fingers dataset into their respective classes, with high accuracy.
### Results
Our model, trained to stop at 0.002 validation loss, reported the following accuracies:
- 99.85% training
- 99.97% validation
- 99.92% testing
### Conclusion
The Convolutional Neural Network was extremely effective in classifying each image into its respective class.
## Dataset
We used the [Fingers](https://www.kaggle.com/datasets/koryakinp/fingers) dataset by Pavel Koryakin.

This dataset was very attractive to us for our first Convolutional Neural Network project as it offered a large balanced dataset, with a good amount of preprocessing already applied to the images to assure effective model training.

**NOTE** We have modified the file structure of our dataset so each image is contained within a parent folder denoting its class. This is done in order to properly make use of the Keras ImageDataGenerator class when preapring our data for training and testing. This modified dataset is required if you wish to use the code. (See example of modified structure below)

![image](https://user-images.githubusercontent.com/90881660/179855081-24058c39-6c8a-4dca-a17e-5e935ed6820f.png)
## Installation and Execution
### Create and test model from scratch
1. Open *FingersClassification.ipynb* on Google Colab. 
2. Upload *fingers_dataset_modified.zip* into the session storage. (This can be done by selecting the "Files" icon in the left toolbar, followed by the "Upload Session Strorage" icon.)
3. Navigate to the top Menu, Select **Runtime > Run All**. This will run the Setup, Training and Testing sections in succession and print the testing results at the end. (Please note its takes approximatley 10-15 mins to train the model)
## Performance Parameters
### Performace Evaluation
In the training process, performace of the model is evaluated by: 
- **Accuracy**: the goal is to maximize training accuracy (without overfitting)
- **Validation Loss**: the goal minimize validation loss
- **Validation Accuracy**: the goal is to maximize the validation accuracy

Analyzing these metrics allow us to identify if the model is behaving correctly.

When evaluating performance of the complete model, we use prediction accuracy to determine the model's efficacy.
### Hyperparameters
The model's hyperparameters (sizes of Conv2D and Dense layers) have been hard-coded in after our model omptimization evaluation.

Others parameters such as layer choice, count and order were selected in a trial and error process beginning with the simplest model we could create and progressively making it more complex.
## Developers
Sebastian Koller - Senior Computer Science Student at Wilfrid Laurier University

Nadia Eghnaim - Senior Computer Science Student at Wilfrid Laurier University
## License
MIT License (See LICENSE.md)
