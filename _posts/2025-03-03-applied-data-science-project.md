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
The raw hotel review data underwent several preprocessing steps to ensure consistency and quality of the analysis. The following steps were performed:
•	Removal of special characters, numbers, and punctuation.
•	Conversion of text to lowercase.
•	Removal of stopwords.
•	Lemmatization to convert words into their base forms.

2. Tokenization
The text data was tokenized into individual words to facilitate further analysis. This process helped in breaking down the reviews into smaller components, making it easier to identify patterns and trends.

3. Exploratory Data Analysis (EDA)
Initial exploratory data analysis revealed that the majority of the reviews carried positive sentiment. The most common words in the dataset were fairly general, such as "good," "stay," and "service," which highlighted the need for more refined topic modelling.

4. Sentiment Analysis
Sentiment analysis was conducted to classify reviews into positive, negative, and neutral categories. Additionally, a new column was added to the dataset to calculate review length and investigate whether review length played a role in sentiment distribution. The analysis indicated that longer reviews tended to express more detailed experiences, often associated with either very positive or very negative sentiments.

### Topic Modelling with LDA
Latent Dirichlet Allocation (LDA) was used to uncover hidden topics within the reviews. The initial model with 5 topics produced overly general themes. To enhance the granularity of insights, the number of topics was increased to 10. This adjustment allowed for better identification of customer concerns and key strengths.

### Evaluation
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce bibendum neque eget nunc mattis eu sollicitudin enim tincidunt. Vestibulum lacus tortor, ultricies id dignissim ac, bibendum in velit. Proin convallis mi ac felis pharetra aliquam. Curabitur dignissim accumsan rutrum. In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris. Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc. Praesent varius interdum vehicula. Aenean risus libero, placerat at vestibulum eget, ultricies eu enim. Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

## Recommendation and Analysis
Explain the analysis and recommendations

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce bibendum neque eget nunc mattis eu sollicitudin enim tincidunt. Vestibulum lacus tortor, ultricies id dignissim ac, bibendum in velit. Proin convallis mi ac felis pharetra aliquam. Curabitur dignissim accumsan rutrum. In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris. Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc. Praesent varius interdum vehicula. Aenean risus libero, placerat at vestibulum eget, ultricies eu enim. Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

## AI Ethics
Discuss the potential data science ethics issues (privacy, fairness, accuracy, accountability, transparency) in your project. 

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce bibendum neque eget nunc mattis eu sollicitudin enim tincidunt. Vestibulum lacus tortor, ultricies id dignissim ac, bibendum in velit. Proin convallis mi ac felis pharetra aliquam. Curabitur dignissim accumsan rutrum. In arcu magna, aliquet vel pretium et, molestie et arcu. Mauris lobortis nulla et felis ullamcorper bibendum. Phasellus et hendrerit mauris. Proin eget nibh a massa vestibulum pretium. Suspendisse eu nisl a ante aliquet bibendum quis a nunc. Praesent varius interdum vehicula. Aenean risus libero, placerat at vestibulum eget, ultricies eu enim. Praesent nulla tortor, malesuada adipiscing adipiscing sollicitudin, adipiscing eget est.

## Source Codes and Datasets
[Upload your model files and dataset into a GitHub repo and add the link here. ](https://github.com/Hazizul10/ITD214_ProjectFiles.git)
