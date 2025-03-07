---
layout: post
author: Hazizul Humaayun
title: "Applied Data Science Project Documentation"
categories: ITD214
---
## Project Background
The purpose of this report is to conduct a comprehensive text analysis of hotel customer reviews to identify top customer concerns, highlight key strengths, and recommend areas for improvement. By leveraging sentiment analysis and topic modelling, the insights gained will help prioritize service enhancements to improve customer satisfaction and overall experience.

## Work Accomplished
To accomplish the outcome of identifying top customer concerns, highlighting key strengths, and recommending areas for improvement, the following steps were carried out:

Data Preprocessing and Cleaning: Removed special characters, numbers, punctuation, stopwords, and converted text to lowercase. Performed lemmatization to convert words into their base forms.

Tokenization: Split text data into individual tokens to facilitate further analysis.

Exploratory Data Analysis (EDA): Conducted initial word frequency analysis, revealing that most common words were general and the majority of reviews carried positive sentiment.

Sentiment Analysis: Classified reviews into positive, negative, and neutral sentiments. Added a review length column to investigate the relationship between review length and sentiment.

Topic Modeling with LDA: Performed initial LDA modeling with 5 topics, later increased to 10 topics for more granular insights.

Visualization with PyLDAvis: Created interactive visualizations to explore topic distributions and keyword associations.

Sentiment-Based Topic Modeling: Segmented reviews by sentiment and performed topic modeling separately to gain targeted insights.

Custom Stopwords Removal: Imported custom stopwords to remove common but uninformative words like "hotel" and "room."

### Data Preparation
1. Data Preprocessing and Cleaning
The dataset Datafiniti_Hotel_Reviews_Jun19.csv was loaded using the pandas library.
Duplicate reviews were identified and removed to ensure data integrity.

The raw hotel review data underwent several preprocessing steps to ensure consistency and quality of the analysis. The following steps were performed:
•	Removal of special characters, numbers, and punctuation.
•	Conversion of text to lowercase.
•	Removal of stopwords using NLTK's stop words list and custom stop words (e.g., "hotel", "room")
•	Lemmatization to convert words into their base forms using WordNetLemmatizer.

2. Tokenization
The text data was tokenized into individual words to facilitate further analysis. This process helped in breaking down the reviews into smaller components, making it easier to identify patterns and trends.

4. Exploratory Data Analysis (EDA)
•	Review Length Distribution: A histogram was created to visualize the distribution of review lengths, providing insights into the typical length of customer feedback.
•	Word Frequencies: The most frequent words in the reviews were identified and visualized using a bar chart.
•	Word Cloud: A word cloud was generated to highlight the most prominent words, offering a visual representation of key themes.
•	N-gram Analysis: Bigrams (two-word sequences) were analyzed to understand common phrases and word combinations used in the reviews.

Initial exploratory data analysis revealed that the majority of the reviews carried positive sentiment. The most common words in the dataset were fairly general, such as "good," "stay," and "service," which highlighted the need for more refined topic modelling.

6. Sentiment Analysis
Sentiment analysis was conducted to classify reviews into positive, negative, and neutral categories. Additionally, a new column was added to the dataset to calculate review length and investigate whether review length played a role in sentiment distribution. The analysis indicated that longer reviews tended to express more detailed experiences, often associated with either very positive or very negative sentiments.

•	Sentiment Distribution: A histogram was created to visualize the distribution of sentiment scores.
•	Sentiment by Rating: Box plots were used to compare sentiment scores across different hotel ratings, revealing potential relationships between customer satisfaction and sentiment.
•	Sentiment vs. Review Length: A scatter plot was used to explore the correlation between sentiment score and review length.

### Topic Modelling with LDA
Latent Dirichlet Allocation (LDA) was used to uncover hidden topics within the reviews. The initial model with 5 topics produced overly general themes. To enhance the granularity of insights, the number of topics was increased to 10. This adjustment allowed for better identification of customer concerns and key strengths.

### Visual Analysis
Visualization of topic distributions using PyLDAvis provided an interactive way to explore the relationship between topics and keywords. This helped to better understand the dominant themes within the reviews and how they were associated with sentiment categories.

• The pyLDAvis library was used to visualize the topics and their associated words, allowing for interactive exploration.
• Initial topic modeling results were too general. Further analysis involved segregating the reviews based on sentiment (positive and negative) and then performing topic modeling separately. This segregation allowed for a more focused identification of topics     
  relevant to positive and negative feedback, revealing more specific themes driving customer satisfaction or dissatisfaction.

### Things done to further improve the Analysis

#### Segregated Sentiment-Based Topic Modelling
• To further improve the analysis, the dataset was segmented by sentiment categories before performing topic modelling. This approach yielded more targeted insights into the concerns expressed in negative reviews and the strengths highlighted in positive reviews.

#### Custom Stopwords Removal
To avoid skewed results, custom stopwords such as "hotel," "room," and other frequently occurring but non-informative words were removed. This step enhanced the clarity of the extracted topics.
  
### Evaluation: Identifying the key strengths in Topics

#### Key Strengths Identified from Positive Reviews
1. Topic #1: Friendly and Helpful Staff
Top Words: staff, great, clean, friendly, helpful, historic
Insight: Customers consistently praised the friendly and helpful attitude of the staff, especially in historic and high-traffic areas like the French Quarter.

3. Topic #3: Scenic Views and Pool Facilities
Top Words: great, view, nice, pool, location, perfect
Insight: Guests enjoyed beautiful views and clean pool facilities, indicating these amenities positively impact customer satisfaction.

4. Topic #7: Breakfast Quality and Free Parking
Top Words: good, great, breakfast, parking, restaurant, free
Insight: Complimentary breakfast and free parking were appreciated by customers, especially in budget-friendly hotels.

6. Topic #9: Prime Location and Restaurant Options
Top Words: great, location, restaurant, beach, enjoyed
Insight: Hotels located near beaches, restaurants, and city attractions received positive feedback, especially in destinations like San Francisco and Waikiki.

#### Key Strengths Identified from Negative Reviews
1. Topic #4: Dirty Rooms and Smell Issues
Top Words: dirty, smell, bed, floor, water, old
Insight: The most common complaint was dirty rooms and unpleasant smells, particularly in older hotels.

2. Topic #6: Shower and Luggage Issues
Top Words: shower, luggage, fix, microwave, dirty
Insight: Guests frequently reported broken showers and dirty amenities like microwaves, which negatively impacted their stay.

3. Topic #8: Poor Front Desk Service
Top Words: desk, bad, bathroom, booked, bed
Insight: Poor front desk service and issues with room bookings were recurring concerns across various hotels.

4. Topic #10: Gym Facilities and Cleanliness
Top Words: gym, cleanliness, food, decor, size
Insight: The cleanliness of gym facilities and food quality were identified as areas needing improvement.

### Recommendation and Analysis
Based on the analysis, the following recommendations are proposed to enhance customer satisfaction:
•	Improve Cleanliness Standards: Implement stricter cleaning protocols for rooms, bathrooms, and gym facilities.
•	Upgrade Maintenance Services: Address frequent issues with showers, microwaves, and other room amenities promptly.
•	Enhance Front Desk Training: Provide customer service training to improve front desk efficiency and communication.
•	Expand Breakfast Options: Upgrade breakfast selections to offer more variety and better quality.
•	Leverage Strengths in Marketing: Highlight friendly staff, prime locations, and free amenities in promotional materials.

### Conclusion
This report identifies both positive and negative aspects of customer experiences in hotels. By focusing on cleanliness, customer service, and maintenance, hotels can significantly improve guest satisfaction. Leveraging existing strengths in marketing campaigns will further enhance the hotel's reputation and customer loyalty.

Further analysis could involve exploring the relationship between specific topics and customer ratings or demographics.
The identified themes and sentiment insights can be used to inform hotel management about areas for improvement and strategies to enhance customer experience.

### AI Ethics
1. Privacy Concerns:
•	Sensitive Information: Reviews might reveal sensitive information about individuals' preferences, habits, or experiences. Be mindful of potential privacy risks when analyzing and interpreting such data. Avoid making inferences or drawing conclusions that could   violate user privacy.
2. Bias and Fairness:
• Review Bias: Online reviews can be subject to various biases, including self-selection bias, where individuals with strong opinions are more likely to leave reviews. This can skew the analysis and lead to inaccurate conclusions about overall customer sentiment.
• Algorithmic Bias: The sentiment analysis and topic modeling techniques used in my code rely on algorithms that can be susceptible to bias.

3. Data Security:
• Data Storage: Hotel review data should be stored securely to prevent unauthorized access or breaches. Follow best practices for data security, including encryption and access control measures.
• Data Sharing: Be cautious when sharing or publishing your findings, ensuring that any data shared is anonymized and does not violate privacy regulations or agreements.

4. Transparency and Explainability:
• Model Transparency: The algorithms used in my analysis, LDA, should be well-documented and understandable. Transparency about the models' limitations and potential biases is crucial for building trust in the results.

7. Misuse of Insights:
• Manipulative Marketing: The insights gained from my analysis could be misused for manipulative marketing practices, such as targeting specific customer segments with tailored messages that exploit their preferences or vulnerabilities. It's important to use the   insights responsibly and ethically.
• Unfair Competition: Analyzing competitor reviews could potentially be used for unfair competitive advantage.

#### Recommendations:
• Prioritize Privacy: Anonymizing the data and ensuring compliance with privacy regulations.
• Mitigate Bias: using Diverse datasets and evaluating algorithms for potential bias.
• Ensure Security: Securely storing and sharing data.
• Be Transparent: when Documenting methods, acknowledging limitations, and interpreting results.
• Using Insights Ethically: Avoid manipulative marketing or unfair competition.

## Source Codes and Datasets
[Upload your model files and dataset into a GitHub repo and add the link here. ](https://github.com/Hazizul10/ITD214_ProjectFiles.git)
