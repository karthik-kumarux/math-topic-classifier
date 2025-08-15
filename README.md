Math Problem Topic Classifier
This project demonstrates training a math problem topic classifier using the MATH dataset and a DistilBERT model.

Project Goal
The goal of this project was to build a model that can automatically classify the topic or subject of a given mathematical problem.

Dataset
The dataset used for training and evaluation is the MATH Dataset (Hendrycks et al.). This dataset contains a collection of challenging math problems categorized by subject and difficulty level.

Model
A pre-trained DistilBERT model was fine-tuned for sequence classification on the collected math problems and their corresponding topics.

Process
Dataset Download and Loading: The MATH dataset was downloaded from Kaggle using kagglehub.
Data Collection and Preparation: Math problems and their topics were extracted from the JSON files in the downloaded dataset and organized into pandas DataFrames.
Data Preprocessing: The problem text was tokenized using the DistilBERT tokenizer, and topic labels were converted into numerical IDs.
Model Training: A DistilBERT model configured for sequence classification was fine-tuned on the preprocessed dataset using the Hugging Face Trainer API.
Evaluation: The model's performance was evaluated on a test set, achieving an accuracy of approximately 77.14% in our training run.
Model Saving: The trained model and tokenizer were saved for future use.
Prediction Interface: A simple function was created to load the saved model and predict the topic of new math problems.
Results
The trained model is capable of predicting the topic of a math problem based on its text. The validation accuracy achieved during training was approximately 77.14%.

Citation  :

@article{hendrycksmath2021,
  title={Measuring Mathematical Problem Solving With the MATH Dataset},
  author={Dan Hendrycks and Collin Burns and Saurav Kadavath and Akul Arora and Steven Basart and Eric Tang and Dawn Song and Jacob Steinhardt},
  journal={NeurIPS},
  year={2021}
}
