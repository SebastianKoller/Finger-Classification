# CP468 Fingers Classification
7/17/2022
## Description
AI project for CP468 at Wilfrid Laurier University with Professor Sukhjit Sehra.
### Objective
Train a Convolutional Neural Network to be able to classify images in the fingers dataset into their respective classes, with high accuracy.
### Results
Our model, trained to stop at 0.002 validation loss, reported the following accuracies:
99.48% training
99.97% validation
99.92% testing
### Conclusion
The Convolutional Neural Network was extremely effective in classifying each image into its respective class.
## Dataset
We used the [Fingers](https://www.kaggle.com/datasets/koryakinp/fingers) dataset by Pavel Koryakin.
This dataset was very attractive to us for our first Convolutional Neural Network project as it offered a large balanced dataset, with a good amount of preprocessing already applied to the images to assure effective model training.
## Installation and Execution
### Testing our pre-trained model
1. Open *FingersClassification.ipynb* on Google Colab. 
2. Upload *fingers_dataset_modified.zip* and *FingersModel* into the session storage. (This can be done by selecting the "Files" icon in the left toolbar, followed by the "Upload Session Strorage" icon.)
3. Navigate to the **Setup Section** in the notebook and run all cells. (This can be done easily by collapsing the section and clicking the play button)
4. Ignore the Training Section and navigate to the **Testing Section** and run the code block inside. The output of this block displays the testing results using our pre-trained model.
### Create and test model from scratch
1. Open *FingersClassification.ipynb* on Google Colab. 
2. Upload *fingers_dataset_modified.zip* into the session storage. (This can be done by selecting the "Files" icon in the left toolbar, followed by the "Upload Session Strorage" icon.)
3. Navigate to the top Menu, Select **Runtime > Run All**. This will run the Setup, Training and Testing sections in succession and print the testing results at the end. (Please note its takes approximatley 5-10 mins to train the model)
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
## Developers
Sebastian Koller - Senior Computer Science Student at Wilfrid Laurier University
Nadia Eghnaim - Senior Computer Science Student at Wilfrid Laurier University
## License
MIT License
