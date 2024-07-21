Sentiment Analysis of YouTube Comments for iPhone 15 Pro
========================================================

Overview
--------

This project involves performing sentiment analysis on YouTube comments related to the iPhone 15 Pro. The goal is to gauge public opinion and sentiment towards the new iPhone model. We aim to identify key trends, sentiments, and common themes expressed by users in their comments.

Objectives
----------

*   **Understand public perception**: Analyze the sentiments in comments to determine whether users are positive, negative, or neutral about the iPhone 15 Pro.
    
*   **Identify common themes**: Discover frequent topics and keywords associated with the sentiments expressed in the comments.
    

Methodology
-----------

### Data Collection

The dataset was collected by scraping comments from YouTube videos using Python libraries such as BeautifulSoup, requests, and pandas. The comments were extracted from videos specifically discussing the iPhone 15 Pro.

### Data Cleaning

The following steps were taken to clean and preprocess the text data:

*   **Remove HTML tags**: Extracted text content by removing HTML tags using BeautifulSoup.
    
*   **Remove URLs**: Eliminated URLs from comments using regular expressions.
    
*   **Handle Emojis**: Converted emojis to their textual representation using the emoji library.
    
*   **Lowercase Conversion**: Converted text to lowercase to standardize the data.
    
*   **Remove Punctuation and Numbers**: Removed punctuation and numeric characters from the text.
    
*   **Remove Stop Words**: Removed common English stop words to focus on meaningful words.
    

### Sentiment Analysis

We utilized the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment analysis tool from the nltk library. The sentiment scores were computed, and each comment was categorized into one of the following sentiments:

*   **Positive**: Sentiment score >= 0.05
    
*   **Negative**: Sentiment score <= -0.05
    
*   **Neutral**: -0.05 < Sentiment score < 0.05
    

### Visualization

Visualizations were created to present the sentiment distribution and common themes:

*   **Sentiment Distribution Pie Chart**: Displayed the proportion of positive, negative, and neutral comments.
    
*   **Word Clouds**: Generated word clouds for positive, negative, and neutral comments to visualize common words.
    
*   **Sentiment Trend Over Time**: Analyzed how sentiment changed over time, if timestamps were available.
    

Results
-------

### Sentiment Distribution

The sentiment analysis revealed the following distribution of sentiments:

*   **Positive Comments**: X%
    
*   **Negative Comments**: Y%
    
*   **Neutral Comments**: Z%
    

### Common Themes

Word clouds highlighted the most frequent words in each sentiment category:

*   **Positive Comments**: Keywords like "love", "great", "best", and "awesome" were common.
    
*   **Negative Comments**: Keywords like "hate", "worst", "bad", and "disappointed" were prevalent.
    
*   **Neutral Comments**: Keywords such as "features", "phone", "price", and "review" appeared frequently.
    

### Sentiment Over Time

The sentiment trend over time showed fluctuations, with notable peaks and troughs corresponding to specific events or announcements related to the iPhone 15 Pro.

Conclusion
----------

The sentiment analysis of YouTube comments provided valuable insights into public opinion on the iPhone 15 Pro. The project successfully identified the general sentiment trend and highlighted key topics of discussion among users. Future work could include expanding the dataset, exploring more sophisticated NLP techniques, or integrating additional data sources for a more comprehensive analysis.

Future Work
-----------

*   **Expand Dataset**: Gather more comments from additional videos for a broader analysis.
    
*   **Enhance NLP Techniques**: Explore advanced NLP models such as BERT or GPT for deeper sentiment analysis.
    
*   **Incorporate Additional Data**: Include user demographics or video metadata to enrich the analysis.
    

References
----------

*   VADER Sentiment Analysis
    
*   BeautifulSoup Documentation
    
*   [Emoji Library Documentation](https://pypi.org/project/emoji/)
