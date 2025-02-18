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

- The dataset used in this analysis is composed of three files: train.json, test.json, and val.json.
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

## Key Findings





--------------
## Project Overview:

Dataset: train.json, test.json, and val.json

Restaurant dataset that comprises 8,879 reviews of a single restaurant. These reviews are categorized into eight distinct aspects: food, service, staff, price, ambience, menu, place, and miscellaneous.

Sentiment analysis is a technique in natural language processing (NLP) and text mining that involves analyzing and determining the emotional tone or sentiment expressed in a piece of text. The goal is to understand the feelings, opinions, or attitudes conveyed by the text, whether it's positive, negative, neutral, or even more specific emotions like anger, joy, or sadness.

## Objectives:

Sentiment analysis in this restaurant review dataset involves analyzing customer reviews to determine whether the sentiment is positive, negative, or neutral. By examining key aspects like food, service, staff, ambiance, and price, the project aims to uncover customer experiences and identify areas for improvement. The goal is to provide actionable insights that help optimize restaurant operations, enhance customer satisfaction, and improve overall performance. With these insights, the restaurant can refine its strategies, improve service quality, and ultimately boost customer loyalty.

## Project Structure:

1. Text Preprocessing & Data Preparation:
- Clean the review data by removing noise such as special characters, stop words, and any irrelevant information to prepare the text for analysis.
- Using Word2Vec Skipgram embeddings as discover in Optimizing Sentiment Analysis Models for Accurate Predictions Project

2. Exploratory Data Analysis (EDA):
- Perform some basic analysis and visualizations to get an overall understanding of the data, looking at trends and patterns.

3. Train the Model (LSTM with Attention -  best model in Optimizing Sentiment Analysis Models for Accurate Predictions Project):
- Train the LSTM model with an attention mechanism to highlight the important words related to the review's aspects and sentiment.

4. Apply the Model & Generate Insights:
- Use the trained model on the dataset to make predictions. Then, analyze the new dataset by visualizing the results to gain insights and understand the overall sentiment.

---

## Outcome: 

![image](https://github.com/user-attachments/assets/ca2aa8e4-e93a-4fb4-b948-79f9b7ade192)
Figure 1: Top Aspects in Terms of Frequency

![image](https://github.com/user-attachments/assets/202f43df-9ba2-4d26-95d2-57e73c245581)
Figure 2: Sentiment Distribution Across Aspects

![image](https://github.com/user-attachments/assets/45beeec4-aa6a-4425-a787-2e378a73e6c3)
Figure 3: Food Aspect with Each Polarity Wordcloud 

Overview on Food Aspect:

- Positive Sentiment: Words like "good", "great", "menu", "price", "service", "waiter", "worth", "best", "better", and "delicious" dominate.
- Neutral Sentiment: Common words include "service", "food", "table", "drink", "waiter", "order", "waitress", "time", "place", and "dinner"
- Negative Sentiment: The word "food", "service", "menu", "bland", "price", "expensive", "cold", "waiting", "overprice", and "average"

![image](https://github.com/user-attachments/assets/e37c8d58-3610-406b-a832-7ccd57dabc63)
Figure 4: Staff Aspect with Each Polarity Wordcloud

Overview on Staff Aspect:

- Positive Sentiment: Words like "table", "staff", "waiter", "friendly", "nice", "attentive", "helpful", "promtly", "server", and "appetizer" dominate.
- Neutral Sentiment: Common words include "waiter", "food", "chef", "table", "menu", "time", "staff", "manager", "waitress", and "service"
- Negative Sentiment: The word "order", "table", "time", "waiter", "rude", "attitude", "manager", "waiting", "seated", and "minute"

![image](https://github.com/user-attachments/assets/682093f6-e583-483c-b133-15f33673f2a5)
Figure 5: Miscellaneous Aspect with Each Polarity Wordcloud

Overview on Miscellaneous Aspect:

- Positive Sentiment: Words like "portion", "entree", "menu", "place", "great", "price", "big", "time", "good", and "quality" dominate.
- Neutral Sentiment: Common words include "reservation", "table", "wait", "waiter", "hostess", "seated", "drink", "dessert", "waiting", and "time"
- Negative Sentiment: The word "small", "portion", "table", "food", "price", "seat", "long", "line", "tiny", and "crowd"

![image](https://github.com/user-attachments/assets/6724f1e4-da2d-41c7-8d2f-d2092036ed95)
Figure 6: Service Aspect with Each Polarity Wordcloud

Overview on Service Aspect:

- Positive Sentiment: Words like "good", "friendly", "great", "attentive", "service", "attentive", "excellent", "best", "quickly", and "better" dominate.
- Neutral Sentiment: Common words include "food", "waiting", "service", "table", "average", "drink", "seated", "reservation", "good", and "quick"
- Negative Sentiment: The word "service", "wait long", "crowded", "hour", "slow", "rude", "bad", "poor", "price", and "reservation"

## INSIGHTS & RECOMMENDATIONS:

Based on the information of Sentiment Distribution Across Aspects plot, Top Aspects in Term of Frequency, and wordclouds of some aspects, we have some observe and recommendations:

1. Food - most discussed aspect 

Finding:
- Food is the most frequently mentioned aspect
- Positive Sentiments: Words like "delicious," "best," "worth," "great," "good" indicate satisfaction.
- Neutral Words: "service," "waiter," "menu," "table," "order" suggest that food discussions often involve service experiences.
- Negative Words: "bland," "cold," "overpriced," "waiting," "average" highlight concerns about food quality, temperature, and price.

Recommendations:
- Improve Consistency: Ensure food temperature and taste remain consistent across different visits.
- Menu Adjustments: Address concerns about food blandness—consider introducing bolder flavors or customizable spice levels.
- Value Perception: Offer combo deals or portion size options to balance pricing concerns.
- Speed Up Food Preparation: Since "waiting" appears frequently, reducing food preparation time is essential.

2. Staff - second most discussed, and most negative aspect

Finding:
- Staff is the second most frequently mentioned topic.
- Positive Sentiments: Words like "friendly," "attentive," "helpful," "promptly" indicate some customers appreciate good service.
- Negative Words: "rude," "attitude," "waiting," "seated," "order," "manager" show dissatisfaction with staff behavior and long wait times.

Recommendations: Since this aspect has most negative review, consider:
- Customer Service Training: Reinforce polite and professional communication to reduce complaints about rudeness.
- Handling Peak Hours: Implement better queue management and proactive updates to customers about wait times.
- Improve Staff Motivation: Employee incentives for good service could improve engagement and attitude.
- Clearer Seating Process: Address complaints about "seated" and "waiting" by streamlining table assignments.

3. Miscellaneous - third most concerned, and high neutral review

Finding:
- Miscellaneous aspects often involve elements like portion size, seating, reservations, and general dining experience.
- Neutral Words: "reservation," "table," "wait," "hostess," "dessert," "drink"
Negative Words: "small," "portion," "long," "line," "tiny," "crowd"
- The majority of these reviews are neutral, which means they are not particularly satisfied or dissatisfied—an opportunity for improvement.

Recommendations:
- Enhance Reservation & Seating Experience: Digital waitlist systems or pre-booking options can reduce complaints about "table," "long," and "line."
- Portion Size Adjustments: If "small" portions are a common complaint, either adjust portion sizes or clearly communicate portion expectations in the menu.
- Improve Waiting Area Comfort: Since "crowd" and "tiny" appear in complaints, consider expanding seating space or managing reservations better.

4. Service - highly negative review aspect

Finding:
- Service has a high proportion of negative sentiment, which affects overall customer satisfaction.
- Positive Sentiments: "attentive," "excellent," "quickly"
- Negative Words: "wait long," "slow," "rude," "bad," "poor," "hour"

Recommendations:

- Reduce Waiting Times: Optimize kitchen workflow and improve order management to address complaints about slow service.
- Empower Staff to Handle Issues Proactively: Provide training on diffusing customer frustration and resolving complaints efficiently.
- Monitor Peak Hour Performance: Use customer feedback to determine when service issues arise most and allocate resources accordingly.
