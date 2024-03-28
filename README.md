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

## Usage Examples

### Case 1: Analyzing Sentiment for a Single Product

- **Explanation:**
  - User provides a product type for sentiment analysis.
  - The script filters the dataset for the specified product type.
  - Sentiment analysis is performed on each review to calculate positive, neutral, and negative sentiment.
  - The sentiment distribution and a bar chart visualizing the distribution are displayed.
  
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/9cf602b5-7c15-4c4f-af8f-0b7a481cce94)
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/e8b71de1-7bfb-4f0c-9f73-32221d475f2c)

- Explanation of Case 1 and its functionality.
- Sample output for Case 1.

### Case 2: Comparing Sentiments Between Two Products

- **Explanation:**
  - User enters two product types for comparison.
  - Sentiment analysis is performed for each product individually to calculate positive review percentages.
  - The positive review percentages for both products are compared, and a bar chart visualizes the comparison.
  
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/3bc0321e-4a57-4013-b43a-a4bd31136119)
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/415376c5-667d-43ff-8904-d4d55c212add)
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/1e27653d-fa77-4d83-aea8-870353c3bedb)
![image](https://github.com/utoo0703/Analysis-of-Product-Sentiment-based-on-Product-review/assets/78578594/9014255d-c510-483e-9e0c-e34cd3384a75)

- Explanation of Case 2 and its functionality.
- Sample output for Case 2.

### Case 3: Inputting Random User Reviews
- **Explanation:**
  - User provides a product type for sentiment analysis.
  - The script filters the dataset for the specified product type.
  - Sentiment analysis is performed on each review to calculate positive, neutral, and negative sentiment.
  - The sentiment distribution and a bar chart visualizing the distribution are displayed.

- Explanation of Case 3 and its functionality.
- Sample output for Case 3.
