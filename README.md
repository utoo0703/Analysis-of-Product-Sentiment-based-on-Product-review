# Analysis-of-Product-Sentiment-based-on-Product-review

![architecture](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/3e145086-4841-49c9-b14d-c5b9174217b6)


## Description

This sentiment analysis project is designed to analyze product reviews and determine sentiment labels (positive, neutral, negative) based on the content of the reviews. The project uses natural language processing (NLP) techniques and machine learning algorithms to process text data and extract sentiment-related insights.

## Code Explanation

The project consists of several Python scripts and functions:

- **Main Script (`main.py`):**
  - Contains the main logic for interacting with the user and coordinating the sentiment analysis tasks.
  - Provides a menu-based interface for users to choose options such as analyzing product reviews, comparing products, inputting random user reviews, or exiting the program.

- **Sentiment Analysis Functions (`sentiment_analysis.py`):**
  - `calculate_sentiment_score`: Calculates the sentiment score of a sentence based on positive and negative words.
    - Tokenizes the sentence and filters out stop words.
    - Assigns a sentiment score of +1 for positive words, -1 for negative words, and 0 for neutral words.
  - `analyze_product_reviews`: Analyzes product reviews for a given product type, calculates sentiment labels, and displays sentiment distribution.
    - Filters the dataset for the selected product type.
    - Calculates sentiment labels based on sentiment scores.
    - Visualizes sentiment distribution using matplotlib.
  - `compare_products`: Compares sentiment percentages between two product types.
    - Calls `analyze_product_reviews` for each product type and calculates positive review percentages.
  - `random_user_reviews`: Allows inputting random user reviews and analyzes their sentiment.
    - Takes user input for random reviews and calls `analyze_random_user_reviews` for sentiment analysis.
  - `analyze_random_user_reviews`: Analyzes sentiment for random user reviews.
    - Calculates sentiment scores and labels for each random review.

- **Data Handling (`data_handling.py`):**
  - Loads the necessary data files (e.g., positive and negative word lists, product reviews dataset) using pandas.

- **Dependencies (`requirements.txt`):**
  - Lists the required Python libraries and their versions for running the project (e.g., pandas, matplotlib, nltk).

