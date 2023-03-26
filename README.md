# Sentiment-Analysis-and-Classification-of-Hotel-Reviews

Problem Statement
Travelers depend heavily on hotels, and as information became more widely available, new methods of choosing the finest ones appeared. The feedback from past visitors are one of the crucial factors in determining whether a future client would choose the hotel or not.

The analysis and classification of trip Advisor evaluations was the main focus of this project. The hotel management will be informed of what previous guests thought based on their experiences, and this will enable the management to make improvements that will best serve their guests.

Data Sourcing:
Due to my curiosity on how this problem can be best solved and improvement the performance of the hotel , i went ahead to search for data on kaggle. I found the Trip Advisor Hotel Reviews dataset and
downloaded the csv file. The dataset consists of about nearly 20,000 hotel reviews with ratings.

This is the link https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews


Data Transformation:
Special characters, hyperlinks, tags, numerals, whitespaces, and punctuation were removed from the data to reduce noise. Articles, pronouns, conjunctions, and prepositions were among the stop words that were also eliminated.
Lemmatization was done as well.

After cleaning i get:
- The total word before cleaning: 14853861
- The total word before cleaning: 13667822 

Analysis and Visualizations
During Analysis, The sentiments were labeled (positive, neutral, or negative) in order to make hidden opinions in a review clear. Rating scores of above 3 were labelled as postive, Rating scores of 3 were labelled as neutral while Rating scores of below 3 were labelled as negative.

Wordcloud visualizations make it easier to see which words are most frequently used in customer evaluations.
  
wordcloud representative of Positive reviews

wordcloud representative of negative reviews


Modelling and Evaluation
sklearn library TfidfVectorizer was used convert a collection of text documents to a matrix of TF-IDF features which was then trained  using Multinomial Naive Bayes algorithm

The model’s performance was evaluated by using the accuracy_score evaluation metric. 


Deployment: Fast API and heruko

Conclusion and Recommedation
