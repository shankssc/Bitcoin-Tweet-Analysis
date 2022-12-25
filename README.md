# Bitcoin Tweets Analysis

This project is created as part of the Data Mining course at IU. As part of this project, our goal is to analyze tweets related to Bitcoin. The presentation related to the project can be found on [YouTube](https://youtu.be/sZwj2wcSRPA).  

The slides for the presentation are included in this repository as [`PresentationSlides.pdf`](./PresentationSlides.pdf). Also, the report for the project containing all the information is also available in this repository as [`Report.pdf`](./Report.pdf).

## Data

We have used [Kaggle dataset](https://www.kaggle.com/datasets/alaix14/bitcoin-tweets-20160101-to-20190329) for Bitcoin tweets. You can find the dataset and all the intermediate files (processed files) on [this OneDrive folder](https://indiana-my.sharepoint.com/:f:/g/personal/ashuhath_iu_edu/EpwKwI_dx7pIjIvdSt6WTFkBvxT0qGiXjOPemI4pT5tjWA?e=dGxWDE). If you are looking at the OneDrive folder, then the original dataset file is [`tweets.csv`](https://indiana-my.sharepoint.com/:x:/g/personal/ashuhath_iu_edu/EWvr87f5QulFnsjvMHWHvyUBu7aHdNgto-sms0y83nwIqw?e=1NMiH0).

Due to the size of the dataset files, we haven't included it in the repository but if you want to run the project, then you can create `data` dir in the root of the project repo and add `tweets.csv` file to it. Also, please make sure to create virtual environment and install all dependencies mentioned in `requirements.txt` file. Now, you are good to run all the notebooks in the project.

## Notebooks

All of our codebase is created as jupyter notebooks. Below are the sequential order of notebooks we created which you can follow to understand the flow of analysis in the project.

- Language Detection: [`language_detect.ipynb`](./notebooks/language_detect.ipynb) is created to detect language of tweet text and to filter English language tweets.
- Exploratory Data Analysis: [`EDA.ipynb`](./notebooks/EDA.ipynb) contains code for initial distribution analysis, histogram, different types of aggregation, preprocessing data for prediction modelling etc. 
- Sentiment Analysis: [`DM_project_Sentiment_analysis.ipynb`](./notebooks/DM_project_Sentiment_analysis.ipynb) contains code corresponding to extracting sentiments out of the tweet text and statistical analysis of the sentiment analysis.
- Clustering Analysis: [`DM_Proj_Clustering.ipynb`](./notebooks/DM_Proj_Clustering.ipynb) contains code corresponding to user level clustering analysis using different methods like K-means, Heirarchial and Density based clustering.
- Regression Analysis: [`regression.ipynb`](./notebooks/regression.ipynb) contains code for predicting bitcoin price based on tweets and previous day bitcoin price. It contains code for multiple regression models and comparison between them. It also contains code for parameter tuning using K-Fold cross validation.
- Classification Analysis: [`BTC_price_prediction_classification.ipynb`](./notebooks/BTC_price_prediction_classification.ipynb) contains code for predicting whether the bitcoin price would go up or down the next day. It contains code for multiple models and comparison between them.

## Group Members

Below are the group member information and their respective contribution in the project. Note that these group members are also responsible for creating slides and writing report for the corresponding topics they worked on.

- Ashutosh Hathidara ([ashuhath@iu.edu](ashuhath@iu.edu)): Language Detection, Exploratory Data Analysis, Regression Analysis
- Gaurav Atavale ([gatavale@iu.edu](gatavale@iu.edu)): Sentiment Analysis, Classification Analysis
- Suyash Chaudhary ([suschaud@iu.edu](suschaud@iu.edu)): Clustering Analysis