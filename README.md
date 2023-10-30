# TextPatternAnalysis-ML
## Analysis of Amazon Food Reviews
### Overview

This project conducts a comprehensive analysis on Amazon food reviews utilizing text analysis methodologies, aiming to uncover insights on the sentiment and patterns in the reviews.

### Data Source

Dataset: Obtained from the Stanford Network Analysis Project.
Size: Over 500,000 food reviews from Oct 1999 to Oct 2012.
Details: Over 260 users with more than 50 reviews. 256,059 users reviewing 74,000+ products.
Format: Reviews are stored in a csv file (Reviews.csv) pulled from the SQLite table named Reviews in database.sqlite.
Columns: The dataset houses various columns, with a focus on 'Score' for ratings and 'Text' for the actual review content.

### Text Analysis

Subset Selection: From the vast dataset, a subset of 50,000 reviews is chosen for the analysis.
Tokenization: Using NLTK, reviews are broken into words or 'tokens'.
Stopword Removal: Commonly used words with minimal significance (like 'and', 'the', 'is') are removed.
Stemming and Lemmatization: Words are transformed to their root or base form.
POS Tagging: Identifies part-of-speech for each token.
Entity Recognition: Recognizing named entities using NLTK.

### Sentiment Analysis

Methodology: Uses the SentimentIntensityAnalyzer from NLTK, utilizing a bag-of-words approach.
Scoring: For each review, sentiment scores (positivity, negativity, neutrality, and compound) are computed and stored.

### Evaluation and Visualization

Relationship between review scores and sentiment scores are visualized using bar plots.
Analysis indicates higher sentiment scores for reviews with higher ratings.

### Project Code Steps

Setup: Import necessary libraries and tools.
Data Loading: Read data into a Pandas dataframe.
Exploratory Analysis: Visualize the data, understand score distributions.
Text Preprocessing: Tokenization, stemming, lemmatization, etc.
Sentiment Computation: Calculate sentiment scores for each review.
Visualization: Understand trends and patterns in the sentiment data.

### Key Insights

Higher-rated reviews manifest more positive sentiments while the reverse holds true for lower-rated reviews. This sentiment analysis effectively captures the mood of the reviews, granting businesses and consumers deeper insights.

### Bibliography

Stanford Network Analysis Project (2013). Amazon Fine Food Reviews
McAuley, J., & Leskovec, J. (2013). From Amateurs to Connoisseurs: Modeling the Evolution of User Expertise through Online Reviews.

### How to Run

Ensure you have Python installed along with the libraries mentioned in the project (like pandas, NLTK, etc.). Run the code provided to analyze the data and view visualizations.
