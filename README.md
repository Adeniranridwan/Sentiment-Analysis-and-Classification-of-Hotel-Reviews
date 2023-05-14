# Sentiment-Analysis-and-Classification-of-Hotel-Reviews

**Problem Statement**
Travelers depend heavily on hotels, and as information became more widely available, new methods of choosing the finest ones appeared. The feedback from past visitors are one of the crucial factors in determining whether a future client would choose the hotel or not.

The analysis and classification of trip Advisor evaluations was the main focus of this project. The hotel management will be informed of what previous guests thought based on their experiences, and this will enable the management to make improvements that will best serve their guests.

**Data Sourcing:**
Due to my curiosity on how this problem can be best solved and improvement the performance of the hotel , i went ahead to search for data on kaggle. I found the Trip Advisor Hotel Reviews dataset and
downloaded the csv file. The dataset consists of about nearly 20,000 hotel reviews with ratings.

This is the link https://www.kaggle.com/datasets/andrewmvd/trip-advisor-hotel-reviews

**Data information:**


**Data Check and Transformation:**
missing values, duplicates, data type, number of unique values for each column, statistics of the data set were checked and jusified where neccessary.
Special characters, hyperlinks, tags, numerals, whitespaces, and punctuation were removed from the data to reduce noise. Articles, pronouns, conjunctions, and prepositions were among the stop words that were also eliminated.
Lemmatization was done as well.

After cleaning i get:
- The total word before cleaning: 14853861
- The total word before cleaning: 13667822 

**Analysis and Visualizations**
During Analysis, The sentiments were labeled (positive, neutral, or negative) in order to make hidden opinions in a review clear. Rating scores of above 3 were labelled as postive, Rating scores of 3 were labelled as neutral while Rating scores of below 3 were labelled as negative.

Wordcloud visualizations make it easier to see which words are most frequently used in customer evaluations.
  
wordcloud representative of Positive reviews
![](positive review.png)

wordcloud representative of negative reviews
![](negative review.png)

**Modelling and Evaluation**
sklearn library TfidfVectorizer was used convert a collection of text documents to a matrix of TF-IDF features which was then trained  using Multinomial Naive Bayes algorithm

The model’s performance was evaluated by using the accuracy_score evaluation metric. 


**Deployment** Fast API and heruko

**Conclusion and Recommedation**



**Conclusion:**
Sentiment analysis of hotel reviews have helped to provide insightful information about customer satisfaction and this will assist the hotel in making the necessary changes to improve the guest experience.


**Recommendation:**

Rectify negative feedbacks: some of the areas where visitors are dissatisfied, as we can see in the negative reviews wordcloud visualization, such as room condition or customer service, are very important to resolve. This can entail enhancing the facilities or giving the employees more training.

Appreciate the positive feedback: Always appreciate the positive feedback of your visitor such as serene resort, beach, good time, room condition as shown in the positive wordcloud visualisation and emphasize this point on your website and during advertisement. This may aid in drawing more visitors to your establishment.

Review responses: Whether they are favorable or unfavorable, responses to guest evaluations should be prompt and polished. This demonstrates your appreciation for client input and dedication to delivering top-notch customer service.

Utilize criticism to improve: Use comments from reviews to tweak your hotel. This may entail putting new rules or procedures into place as a result of ideas from visitors or improving the place in response to frequent complaints.

Track the mood over time: As time passes, keep an eye on sentiment analysis of your hotel reviews to monitor shifts in visitor perception. This might assist you in seeing patterns so you can alter as needed to please your visitors.
