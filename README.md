This repository serves as a platform where I may discuss projects I have worked on, demonstrate skills I have picked up as well as track my progress in the field of Data Science & Analytics. Thanks for stopping by!

- **[Tableau Visualizations](https://public.tableau.com/app/profile/lim.yi.han)**
- **[Github Page](https://github.com/Yihan2407/Yihan2407.github.io)**



## About

Hey there, I'm Yi Han!  I'm currently an undergraduate at the National University of Singapore pursuing a degree in Economics with a Second Major in Business Analytics. My passion for utilizing big data and analytics to drive informed decision-making and shape consumer behavior has been a driving force in my academic pursuits. My goal is to continue growing my knowledge and skills to leverage the abundance of online data to drive positive outcomes for businesses and society as a whole.

## Table of Contents
- [About](#about)
- [Table of Contents](#table-of-contents)
- [Stand-alone Projects](#stand-alone-projects)
- [Machine Learning Case Studies](#machine-learning-case-studies)
  * [Classification](#classification)
  * [Regression](#regression)
  * [Natural Language Processing](#natural-language-processing)
- [Econometrics Case Studies](#econometrics-case-studies)
- [Courses & Certifications](#courses--certifications)
- [Contacts](#contacts)

To view the projects, clicking on the project titles will direct you to either the Github Repository or the file/notebook.

## Stand-alone Projects

**[FairPrice Protein Sources: A Cost- & Caloric-Efficiency Analysis](https://github.com/Yihan2407/fairprice_cost_efficiency_analysis)**

The average serving of whey protein contains about 25g of protein. To build muscle, it is commonly recommended to consume a wide range of protein sources instead of only whey protein alone to ensure a well-balanced and nutritious diet. However, how cost- and calorie-efficient (let's abbreviate this as C&C efficiency) is whey protein compared to common protein sources that we may consume within a week? To examine this, I performed a simple study that compares the C&C efficiency of popular Fairprice protein sources to a single serving of whey protein. As a point of reference, I used the Optimum Nutrition Gold Standard Whey Protein, that has 25g of protein and 121kcal per serving. To obtain the data, I scraped the prices and nutritional information of products falling under popular protein sources such as protein bars, dairy and nuts from the FairPrice site, then cleaned and normalized the data with Pandas. Finally, I produced an [interactive dashboard](https://public.tableau.com/app/profile/lim.yi.han/viz/Cost-andCalorieEfficiencyofFairPriceProteinSources/Dashboard1) with Tableau to visualize my findings.

**[Spotify Insights and Recommendations Generator](https://github.com/Yihan2407/Spotify_Insights_and_Recommendations/blob/main/spotipy_recommendations.ipynb)**

After discovering [Spotipy](https://spotipy.readthedocs.io/en/2.22.1/), a well-documented Python library for the Spotify Web API, I knew I had to tinker around with it. One area of focus I wanted to learn more about at the time was recommender systems, and so I delved right in. I learnt that Spotify has data on tracks such as acousticness, danceability, instrumentalness and speechiness, which can be used to generate recommendations based on past listening history. Here, I first generated insights using my top songs of 2022, a playlist that is automatically generated by Spotify annually, such as visualizing the data of my top genres and artists. Next, I created a recommender system using cosine similarity, which measures the similarity between two vectors. By inputting a user's playlist and another target playlist, music recommendations can be generated from the target playlist based on cosine similarity matching the initial playlist.


**[Pokémon Data Exploration: Web Scraping and Machine Learning](https://github.com/Yihan2407/pokemon_analytics)**

Here, I wanted to work on a data analytics project that was related to something of personal interest to me. Looking back to my childhood self, fond memories of Pokémon would arise. It is an extremely popular franchise that is well-known by many around the world, and is accessible regardless of age. In fact, even in 2023, Pokémon remains one of the highest-grossing media franchises of all time. To start off, I web scraped the data of 809 individual Pokémon from the [serebii.net](https://serebii.net/) database, transformed it and stored it as a Pandas dataframe for analysis. Then, I explored the data, performing univariate and bivariate data visualization to showcase the distribution of stats across 18 types. Lastly, I developed and evaluated multiple binary classifiers to predict the legendary status of a given Pokémon.


**[Hospital Management Database: Analytics with SQL](https://github.com/Yihan2407/healthcare-data-analytics)**

At the time, I was really curious about the various types of healthcare data stored, which led me to the course 'Data Analytics: Intro to SQL using Healthcare Data', which culminated in this final project. Using the healthcare data provided, I developed a database that centralized healthcare data including patient IDs and diagnoses, utilizing Microsoft SQL Server Management Studio. Then, I queried various data using subqueries, CTEs, joins and window functions. An example query would be querying the average age of patients by gender with a diagnosis that included Type 2 diabetes.

**[120 Years of Olympic History: Data Exploration with SQL](https://github.com/Yihan2407/olympic_games_analytics/blob/main/olympic_games_analysis.sql)**

The Olympic Games possess a rich history; the first recorded, modern Olympic Games held actually dated back to 1896. Now, the Olympic Games serve as a platform where the best athletes globally may showcase their prowess at a certain sport, thereby promoting peaceful global interactions. Here, I used SQL to explore the [1896 - 2016 Olympic Games dataset](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results) by first importing the csv file into PostgreSQL. Then, I queried various data such as the M:F Gender Ratio of each Olympic Games, incorporating methods such as subqueries, CTEs, aggregation, joins, window functions, rolling sums, CASE expressions, COALESCE, string subsetting and concatenation in my queries.

## Machine Learning Case Studies

### Classification
**[Credit Card Default Classification](https://github.com/Yihan2407/credit-default-analytics)**

Predictive analytics in finance is extremely important as it allows for the prediction of risk in lending (i.e. credit default rates) by using the existing data of clients to identify prominent trends, and thereafter make predictions that generate valuable insights. Given a [dataset](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset) of 30,000 clients, we attempt to create several binary classifiers that would predict whether clients would default on their payment next month, using various factors such as demographic data, credit data and history of payment. A range of machine learning alogrithms have been implemented, including Logistic Regression, K-nearest Neighbors, Support Vector Machines, Random Forests, Neural Network and XGBoost. We have also applied the Synthetic Minority Oversampling Technique to address imbalances in the dataset and improve accuracy of predictions.

**[Cardiovascular Disease Classification](https://github.com/Yihan2407/cardiovascular_diseases_ml_project)**

Cardiovascular diseases (CVD) have been on the rise; in fact, according to the National Heart, Lung and Blood Institute (NHLBI), CVDs alone accounted for one-third of all deaths worldwide, and even posed as a risk factor for severe COVID-19 that would result in hospitalization and death. The [dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset) that I have used contains data on 70,000 patients, with information such as their age, height, weight and cholesterol levels, of which may be correlated to the probability of contracting cardiovascular diseases.  Here, using my prior knowledge on the risk factors of CVDs, I attempt to create several binary classifiers that would predict whether a given patient would contract cardiovascular diseases. A non-exhaustive list of risk factors include smoking, drinking, being overweight, as well as being physically inactive.

### Regression
**[Predicting Property Prices with Regression Techniques](https://github.com/Yihan2407/house_prices_ml_project)**

What determines the value of a property? Given 79 explanatory variables describing almost every aspect of residential homes in Ames, Iowa, I attempt to predict each property's sale price using regression techniques. Examples of explanatory variables include the neighborhood the property resides in, size of the garage, year it was sold, the general shape of the property as well as the above grade living area square feet. I first conducted exploratory data analysis, before proceeding onto data processing & cleaning, imputation of missing values, feature transformation as well as feature engineering to try and maximize the predictive capability of my models. Then, I experimented with several regression models such as Ridge Regression, ElasticNet Regression and Random Forest Regression. Overall, it was a really fun dataset to play around with, and the abundance of predictor variables made for some interesting ways to approach feature transformation and feature engineering.

### Natural Language Processing
**[Twitter Sentiment Analysis](https://github.com/Yihan2407/twitter_sentiment_analysis)**

Sentiment Analysis refers to the process of using Natural Language Processing (NLP) techniques to extract subjective information from text, thereby allowing us to analyze the opinions and emotions of individuals towards a certain topic or event. This can be really useful, especially in the sector of research and policy-making. For example, sentiment analysis can provide valuable data for academic research in fields such as psychology and sociology, or provide insights into public opinion on social and political issues thereby informing policy decisions. As part of a group project, we used a labelled dataset consisting of 100,000 tweets and their respective sentiment labels, with '1' denoting a positive sentiment and '0' denoting a negative sentiment'. Then, we cleaned the data using techniques such as removing Emojis, stopwords (e.g. "the", "is"), punctuations, then proceeded with the expansion of contractions, lemmatization of words to their root form (e.g. "rocks" -> "rock") and tokenization. Finally, we fitted several models such as SVM, Random Forest, Stochastic Gradient Descent. Finally, we attempted to use [GloVe word vectorization](https://github.com/stanfordnlp/GloVe) and trained an LSTM model on the vectorized data, which yielded us the highest accuracy of 80% after tuning. Overall, working with the dataset was rather challenging as it required extensive data pre-processing given the unstructured nature of textual data. Still, it was an eye-opening experience that exposed me to new machine learning techniques.

## Econometrics Case Studies
- Here's another interest of mine -- Econometric analysis helps us understand the causes and effects of economic phenomena and make informed decisions based on empirical evidence via the use of statistical techniques. This allows us to try and find or confirm the relationship between ideas or objects that may not seem immediately apparent at first, for example how meteorological factors may influence the amount of bikes rented on a particular day or how healthcare spending influences health outcomes.

**[Spotify Track Popularity Regression Analysis](https://github.com/Yihan2407/spotify_regression_analysis)**

The Spotify API allows us to view the various characteristics of each track streamed on Spotify, for example audio features such as danceability, tempo and energy, to non-audio features such as the duration of the track and whether the track contains explicit content. Using these features, we can find the one that influences a track's popularity the most?

## Courses & Certifications

While I believe projects are the best way to improve and showcase one's technical skills, courses can also prove to be useful in providing a gentle nudge in the right direction to get started. Here are some of the courses I have completed and certificates I have picked up along the way!

- [SQL (Advanced) Certificate](https://www.hackerrank.com/certificates/fc15f91976e6) (HackerRank)
- [Data Analytics: Introduction to SQL using Healthcare Data](https://www.udemy.com/certificate/UC-b1e7b876-fa42-4d75-95a7-944bc8dc923a/) (Udemy)
- [Machine Learning, Data Science and Deep Learning with Python](https://www.udemy.com/certificate/UC-3e943c34-bde9-4b28-8e11-0116271a7f60/) (Udemy)
- [Tableau 2022 A-Z: Hands-On Tableau Training for Data Science](https://www.udemy.com/certificate/UC-85120abd-34b2-48ff-87c0-f0ec1782ea7c/) (Udemy)
- [Tableau 2022 Advanced: Master Tableau in Data Science](https://www.udemy.com/certificate/UC-2828ed7d-431f-48e1-8545-6ebd87e72cf5/) (Udemy)
- [Data Warehouse: The Ultimate Guide](https://www.udemy.com/certificate/UC-d3a1c4af-eba5-4925-a10e-738e2d0b06e1/) (Udemy)

## Contacts

- **[Linkedin Profile](https://www.linkedin.com/in/lim-yi-han/)**
- **Email: yihanlim24@gmail.com** 

[Return to Top](#about)
