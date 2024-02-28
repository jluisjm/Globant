# Globant
Topic Modeling and Clustering of Abstracts from XML Files
This repository contains code for extracting, analyzing, and clustering abstracts from XML files.

Key Steps
1. Data Extraction:
- Reads XML files from a specified directory.
- Extracts the "AbstractNarration" field from each file.
- Cleans the extracted abstracts by removing special characters.

2. Exploratory Data Analysis (EDA):
- Calculates descriptive statistics about abstract lengths.
- Visualizes the distribution of abstract lengths using a histogram.
- Generates a word cloud to visualize the most frequent words.

3. Text Preprocessing:
- Tokenizes the text into words.
- Normalizes text by converting words to lowercase.
- Removes common stop words.

4. Vectorization and Topic Modeling:
- Converts text to numerical TF-IDF vectors.
- Applies Latent Dirichlet Allocation (LDA) to discover underlying topics.
- Visualizes topics interactively using PyLDAvis.

5. Clustering:
- Groups abstracts based on their semantic similarity using K-Means clustering.
- Uses PCA to visualize clusters in a 2D space.

Requirements
- Python 3.x
- Libraries: pandas, NumPy, seaborn, nltk, wordcloud, sklearn, pyLDAvis, gensim

Usage
1. Clone this repository.
2. Install required libraries: pip install -r requirements.txt
3. Modify the file path in the code to point to your XML files.
4. Run the Python script (main.py or similar).

Output
- The script generates various visualizations and prints results to the console, including:
 - Descriptive statistics about abstract lengths.
 - A histogram of abstract lengths.
 - A word cloud of frequent words.
 - Interactive topic visualization using PyLDAvis.
 - Printed topics with their top words.
 - Grouped abstracts based on their similarity.
 - A scatter plot visualization of clusters using PCA.
