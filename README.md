# Task-3-SVM:
Implementing a Support Vector Machine (SVM) to classify images of cats and dogs involves several steps, including data preprocessing, feature extraction, and model training. Here’s a detailed guide to implement this using Python, along with the necessary libraries such as opencv-python, scikit-learn, and tensorflow for loading and processing images.

Dataset :- https://www.kaggle.com/c/dogs-vs-cats/data

Step-by-Step Implementation:
1)Data Preparation

Load the dataset from Kaggle.
Preprocess the images to ensure they are in a consistent format and size.

2)Extract features from the images to use as input for the SVM model.
Feature Extraction

3)Use a pre-trained CNN model (e.g., VGG16) to extract features from the images.
Train the SVM Model
Train the SVM classifier using the extracted features.

4)Evaluate the Model
Evaluate the performance of the SVM classifier on the test dataset.

Explanation
Data Preparation:

Define the directories for the dataset.
Specify the target image size for the VGG16 model.
Feature Extraction:

Load and preprocess the images using the img_to_array and preprocess_input functions.
Use the pre-trained VGG16 model to extract features from each image.
Flatten the extracted features to create a 1D array for each image.
Train the SVM Model:

Combine the features and labels for cats and dogs.
Split the data into training and testing sets.
Train an SVM classifier with a linear kernel on the training data.
Evaluate the Model:

Make predictions on the test set.
Calculate and print the accuracy of the model.
Save the Model (Optional):

Save the trained SVM model using joblib for future use
