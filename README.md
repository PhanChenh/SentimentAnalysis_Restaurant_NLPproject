# Project Title: Sentiment Analysis of Restaurant Reviews to Enhance Customer Experience and Optimize Operations

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Objective](#objective)
- [Analysis Approach](#analysis-approach)
- [Key Findings](#key-findings)
- [How to run code](#how-to-run-code)
- [Technologies Used](#technologies-used)
- [Results & Visualizations](#results--visualizations)
- [Recommendation](#recommendation)
- [Contact](#contact)

## Overview

This project aims to perform sentiment analysis on restaurant reviews to uncover customer experiences and identify areas for improvement. The dataset consists of 8,879 reviews for a single restaurant, covering eight key aspects: food, service, staff, price, ambience, menu, place, and miscellaneous. By analyzing the sentiment expressed in these reviews, this project provides actionable insights that can help optimize operations, enhance customer satisfaction, and ultimately improve overall restaurant performance.

## Dataset

- The dataset used in this analysis is composed of three files: [train.json](data/train.json), [test.json](data/test.json), and [val.json](data/val.json).
- These files contain a total of 8,879 reviews for a single restaurant.
- Each review is categorized into one of the following eight aspects: food, service, staff, price, ambience, menu, place, and miscellaneous. The sentiment associated with each review is classified as positive, negative, or neutral.

## Objective

Sentiment analysis in this restaurant review dataset involves analyzing customer reviews to determine whether the sentiment is positive, negative, or neutral. By examining key aspects like food, service, staff, ambiance, and price, the project aims to uncover customer experiences and identify areas for improvement. The goal is to provide actionable insights that help optimize restaurant operations, enhance customer satisfaction, and improve overall performance. With these insights, the restaurant can refine its strategies, improve service quality, and ultimately boost customer loyalty.

## Analysis Approach
1. Text Preprocessing & Data Preparation:
  - The first step involves cleaning the review data by removing noise such as special characters, stop words, and irrelevant information. This ensures the text is ready for analysis. Additionally, Word2Vec Skipgram embeddings are applied as discovered in the "Optimizing Sentiment Analysis Models for Accurate Predictions" project.
2. Exploratory Data Analysis (EDA):
  - Basic visualizations and analysis are performed to understand the trends and patterns in the data.
3. Model Training (LSTM with Attention):
  - The Long Short-Term Memory (LSTM) model with an attention mechanism is trained. This model helps highlight the important words related to each review’s aspects and sentiment, enhancing prediction accuracy.
4. Apply the Model & Generate Insights:
  - The trained model is applied to predict sentiment in the reviews. Insights are then drawn by visualizing sentiment distribution and identifying key sentiment drivers in the restaurant experience.
5. Recommendation:
- Based on the insights generated, actionable recommendations are provided to improve the restaurant's customer experience and business strategies.

## Key Findings
- Food: Positive feedback on quality, but concerns over price and temperature. Word clouds help identify areas for improvement, like consistency.
- Staff: 67% negative reviews, mainly about rudeness and wait times. Word clouds can guide staff training and service improvements.
- Miscellaneous: Neutral reviews with some complaints about seating and portion sizes. Word clouds can help optimize these aspects.
- Service: 51% negative reviews, focusing on slow service and poor behavior. Word clouds highlight areas to improve service speed and staff training.

## How to run code
1. Install Required Libraries: Ensure all necessary libraries such as pandas, matplotlib, seaborn, tensorflow, and gensim are installed like in the [file](SentimentAnalysis_RestaurantReview.ipynb)
2. Load the Dataset: Import the dataset by loading the train.json, test.json, and val.json files.
3. Run the Analysis Notebooks: Execute the analysis notebooks in Jupyter to process the data, build and train the model, and visualize the results.

Run this process in Google Colab for easy execution and visualization.

## Technologies Used
- Python Code: Data processing and analysis were done in Python using libraries like pandas and numpy for data manipulation, gensim for Word2Vec and FastText embeddings, and nltk for text preprocessing tasks such as tokenization, stopwords removal, and stemming. Model evaluation was carried out with scikit-learn, and deep learning models were built and trained using torch.

- Visualization: For visualizing the results, matplotlib and seaborn were used for plotting, while wordcloud was utilized to generate word clouds to illustrate sentiment and aspect-wise insights.

## Results & Visualizations

![image](https://github.com/user-attachments/assets/ca2aa8e4-e93a-4fb4-b948-79f9b7ade192)
Figure 1: Top Aspects in Terms of Frequency

Finding: Observe that food, staff, and miscellaneous got mentioned the most

![image](https://github.com/user-attachments/assets/202f43df-9ba2-4d26-95d2-57e73c245581)
Figure 2: Sentiment Distribution Across Aspects

Finding: Food got pretty good review, since there are only around 11% for negative reviews, the rest are neutral and positive. However, the most noticable aspects are staff and service aspects since these two have high negative reviews (67% and 51% respectively)

![image](https://github.com/user-attachments/assets/45beeec4-aa6a-4425-a787-2e378a73e6c3)
Figure 3: Food Aspect with Each Polarity Wordcloud 

Finding on Food Aspect:

- Positive Sentiment: Words like "good", "great", "menu", "price", "service", "waiter", "worth", "best", "better", and "delicious" dominate.
- Neutral Sentiment: Common words include "service", "food", "table", "drink", "waiter", "order", "waitress", "time", "place", and "dinner"
- Negative Sentiment: The word "food", "service", "menu", "bland", "price", "expensive", "cold", "waiting", "overprice", and "average"

![image](https://github.com/user-attachments/assets/e37c8d58-3610-406b-a832-7ccd57dabc63)
Figure 4: Staff Aspect with Each Polarity Wordcloud

Finding on Staff Aspect:

- Positive Sentiment: Words like "table", "staff", "waiter", "friendly", "nice", "attentive", "helpful", "promtly", "server", and "appetizer" dominate.
- Neutral Sentiment: Common words include "waiter", "food", "chef", "table", "menu", "time", "staff", "manager", "waitress", and "service"
- Negative Sentiment: The word "order", "table", "time", "waiter", "rude", "attitude", "manager", "waiting", "seated", and "minute"

![image](https://github.com/user-attachments/assets/682093f6-e583-483c-b133-15f33673f2a5)
Figure 5: Miscellaneous Aspect with Each Polarity Wordcloud

Finding on Miscellaneous Aspect:

- Positive Sentiment: Words like "portion", "entree", "menu", "place", "great", "price", "big", "time", "good", and "quality" dominate.
- Neutral Sentiment: Common words include "reservation", "table", "wait", "waiter", "hostess", "seated", "drink", "dessert", "waiting", and "time"
- Negative Sentiment: The word "small", "portion", "table", "food", "price", "seat", "long", "line", "tiny", and "crowd"

![image](https://github.com/user-attachments/assets/6724f1e4-da2d-41c7-8d2f-d2092036ed95)
Figure 6: Service Aspect with Each Polarity Wordcloud

Finding on Service Aspect:

- Positive Sentiment: Words like "good", "friendly", "great", "attentive", "service", "attentive", "excellent", "best", "quickly", and "better" dominate.
- Neutral Sentiment: Common words include "food", "waiting", "service", "table", "average", "drink", "seated", "reservation", "good", and "quick"
- Negative Sentiment: The word "service", "wait long", "crowded", "hour", "slow", "rude", "bad", "poor", "price", and "reservation"

## Recommendation

Based on the sentiment analysis and insights derived from the reviews, the following recommendations are made:

1. Food:
- Ensure food consistency, especially regarding temperature and taste.
- Consider enhancing the menu with more bold flavors or customizable spice levels to address concerns about bland food.
- Offer combo deals or larger portion options to improve value perception.
2. Staff:
- Reinforce customer service training to address issues with rude behavior and poor attitudes.
- Implement better queue management to handle peak hours and reduce complaints about waiting times.
- Improve staff motivation through incentives and recognition.
3. Miscellaneous:
- Enhance the reservation system by offering digital waitlists or pre-booking options to reduce waiting times.
- Adjust portion sizes or clarify expectations on the menu to address complaints about small portions.
- Improve the waiting area by expanding space or better managing reservations.
4. Service:
- Optimize kitchen and order management workflows to reduce service delays.
- Provide proactive customer service training to handle complaints and frustration efficiently.
- Monitor peak hours to allocate resources effectively and address service issues promptly.

## Contact

📧 Email: phanchenh99@gmail.com

🔗 [LinkedIn](https://www.linkedin.com/in/phan-chenh-6a7ba127a/) | Portfolio
