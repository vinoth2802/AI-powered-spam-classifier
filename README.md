# AI_powered_spam_classifier
## Problem Definition:-
The primary goal of this project is to build an AI-powered spam classifier 
capable of accurately distinguishing between spam and non-spam messages in emails or 
text messages. The key objectives include reducing the number of false positives 
(legitimate messages incorrectly classified as spam) and false negatives (genuine spam 
messages missed), while maintaining a high level of overall accuracy. This project 
addresses a common and vital challenge in natural language processing and machine 
learning. 
## Code Overview:-
This codebase is organized into several sections, each focusing on a specific aspect of the 
project. Below is a summary of the major sections:
### 1) Importing the Dataset:
In this section, we import the necessary libraries to support data analysis, natural 
language processing, and machine learning. These libraries include Pandas, NumPy, 
Matplotlib, NLTK, Seaborn, Scikit-Learn (for LabelEncoder), and others. We also load the 
dataset from a CSV file named "spam.csv" into a Pandas DataFrame. 
### 2) Data Cleaning:
Data cleaning is a crucial step to ensure data quality and consistency. In this section, the 
following tasks are performed: <br>
--> Gathering Information about the Dataset using df.info().<br>
--> Removing Unnecessary Columns: Columns "Unnamed: 2," "Unnamed: 3," and 
"Unnamed: 4" are dropped from the dataset to simplify the structure. <br>
3) Renaming Columns: The columns 'v1' and 'v2' are renamed to 'Type' and 'Message' 
for clarity. <br>
--> Encoding the 'Type' Column: The 'Type' column, likely containing 'spam' and 'ham' 
labels, is encoded into numerical values using LabelEncoder. <br>
--> Checking for Missing Values: We verify if any missing values exist in the dataset. 
--> Checking for Duplicate Values: Duplicates in the dataset are idenƟfied and removed 
to ensure data integrity. <br>
--> Rechecking for Duplicates: After removing duplicates, we confirm that the dataset 
contains no duplicate rows. <br>
### 3) Data Analysis:
Data analysis is a critical step to gain insights into the dataset. This section includes the 
following tasks: <br>
--> Counting the values of the 'Type' column to understand the distribution of spam 
and non-spam messages. <br>
--> Ploting a pie chart to visually represent the distribution of 'ham' and 'spam' 
messages. <br>
--> Analyzing the number of characters, words, and sentences in each message. <br>
--> Calculating descriptive statistics for the entire dataset, as well as separately for 
'ham' and 'spam' messages. <br>
--> Visualizing the distribution of message lengths (characters and words) using 
histograms. <br>
--> Creating pair plots and a heatmap to explore relationships between variables in the 
dataset. <br>
### 4) Data Preprocessing: 
Data preprocessing involves preparing the text data for machine learning. In this section, 
the following steps are taken: <br>
--> Text Transformation: A function, transform_text, is defined to preprocess text. This 
function converts text to lowercase, tokenizes it, removes special characters, stop 
words, and punctuation, and applies stemming.<br>
--> Applying the transform_text function to create a new column 'transformed_text' in 
the dataset. <br>
--> Saving the preprocessed dataset to a CSV file, "processed_dataset.csv." <br>
--> Generating Word Clouds to visualize the most common words in 'spam' and 'ham' 
messages. <br>
--> Analyzing and ploting the top 30 most common words in 'spam' and 'ham' 
messages. <br>
### 5) Data Visualization:
Data visualization is essential for understanding and presenting insights. This section 
includes visualizations such as:<br>
--> Histograms to show the distribution of 'ham' and 'spam' messages using different 
colors. <br>
--> A pie chart to display the distribution of 'ham' and 'spam' messages.<br>
--> Word clouds for both 'spam' and 'ham' messages. <br>
--> Word frequency analysis to identify and visualize the most common words in the 
text data. <br>
--> Message length analysis to explore the distribution of message lengths in 
characters and words. <br>
### 6) Feature Extraction:
Feature extraction is a critical step for preparing the dataset for machine learning. This 
section covers:<br>
--> Importung the necessary dependencies for feature extraction.<br>
--> Using the TF-IDF (Term Frequency-Inverse Document Frequency) vectorization 
technique to convert the text data into numerical features. <br>
--> Spliting the dataset into input features (x) and output features (y).<br>
--> Displaying the dimensions of the input and output features. <br>
### 7) Model Building:
Model building involves creating and training a machine learning model for spam 
classifiction. This section outlines the steps:<br>
--> Importing dependencies for spliting the dataset into train and test sets.<br>
--> Spliting the dataset into training and testing data.<br>
--> Importing TensorFlow for creating a neural network.<br>
--> Building a neural network model with input and hidden layers. <br>
--> Compiling the model with binary cross-entropy loss and the Adam optimizer.<br>
--> Training the model on the training dataset. <br>
--> Evaluating the model's accuracy on the test dataset.<br>
