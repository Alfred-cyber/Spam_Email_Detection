Project Title:

Detecting Spam Emails Using TensorFlow in Python

Objective:

To build a deep learning model using TensorFlow that classifies emails as Spam or Ham (Not Spam).

Key Steps and Methodology:

Import Libraries:
Used essential libraries like pandas, numpy, matplotlib, nltk, TensorFlow, etc., for data handling, preprocessing, visualization, and model building.

Load and Explore Dataset:

Dataset: 5171 emails with labels (spam or ham).

Initial exploration showed an imbalance between spam and ham emails.

Balance the Dataset:

Downsampled the majority class (Ham) to match the number of Spam emails.

Created a balanced dataset for fair training.

Text Cleaning and Preprocessing:

Removed stopwords and punctuations.

Performed basic text cleaning like removing "Subject" prefixes.

Word Cloud Visualization:

Generated separate word clouds for Spam and Ham emails to visualize common words.

Tokenization and Padding:

Text data was converted to numeric sequences.

Sequences were padded to ensure consistent input length for the model.

Model Architecture:

Embedding Layer for word vector representation.

LSTM Layer for sequence modeling.

Dense Layers for classification.

Final layer used sigmoid activation for binary classification.

Model Training:

Used EarlyStopping and ReduceLROnPlateau callbacks.

Trained for up to 20 epochs with validation split.

Evaluation and Results:

Achieved 97% accuracy on the test set.

Plotted training vs. validation accuracy over epochs.

Conclusion:

The project successfully implemented a deep learning-based spam detection system using LSTM in TensorFlow. The model demonstrated high accuracy and can be further fine-tuned for real-world applications.
