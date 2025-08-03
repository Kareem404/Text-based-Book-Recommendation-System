# Text-based-Book-Recommendation-System

📚 In this project, we present a book recommendation system that leverages textual user reviews. There are three main parts in the project. First, the users are presented with trending books created using a hybrid system of Bayesian scoring. Second, we utilize deep learning to to make a personalized recommendation system that unique books for users based on what they have read. Third, we use FP-growth to recommend frequently read together books. All these implementations have integrated togther using a Gradio project. 

# 1. Dataset Description
**TODO**

# 2. Trending-Now System

To create a successful trending-now system for our dataset, we use previous user rating and reviews for books. We implemented bayesian scoring for both the ratings and reviews. The Bayesian Scoring algorithm basically extracts a score that can be seen as a measure of trend.

Implementing Bayesian Scoring for the numerical ratings is deemed to be straightforward; however, implementing it for text (user reviews) is a bit tricky since text is not numeric. To fix this problem, we decided to extract numerical sentimental ratings from the text using an open-source sentiment analyzer named [VADER](https://github.com/cjhutto/vaderSentiment). The details for the implementation is shown in the `./sentiment_scoring.ipynb` notebook. 

After implementing Bayesian Scoring for reviews and ratings, we combine them in a hybrid system. To do so, we give a weight of 0.5 for both the ratings and reviews. In the `./sentiment_scoring.ipynb` notebook, you can clearly see why doing so is better than just using the sentiment scores or numerical ratings only.

# 3. Personalized Recommendations
**TODO**

# 4. Frequently Read Together
**TODO**

# 5. Demo
**TODO**
