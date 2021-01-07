# Uber and Lyft Price Modeling Analyses
## Team Yellow Leopard
## Fall 2020

This repository provides explanations of the data analysis process for the DataRes article "Uber VS Lyft: How do they decide their price?", published [INSERT DATE]. Please check out our article, which contains visualizations and insights about Uber and Lyft price modeling analyses.

Contributors: Yupeng Chen, Sylvia Ma, Hana Yerin Lim, Lu Cheng, Anish Dulla

# Introduction
Our team’s analysis focused on comparing Uber and Lyft rides in Boston, MA for a sample set of 750,000 rideshares. In our analysis, we predicted and compared the price of Uber and Lyft rideshares based on a variety of predictors such as distance, hour of the day, surge multiplier (demand-based pricing), etc. We collected our data from Kaggle and used this rich dataset to build a price prediction model.

# Data Source
The data used to develop our Medium article came from: [Kaggle dataset](https://www.kaggle.com/brllrb/uber-and-lyft-dataset-boston-ma). The contributors of the dataset queried both Lyft and Uber prices in the Boston Area. The queries were done on the apps every 5 minutes for 22 days from late November through mid-December in 2018. The weather data were queried from the Dark Sky API every hour.


# Data Processing
We cleaned up some of the variables of our interests. The time stamp data was in Unix format, so we converted them to fit in the local time zone so that it could be more applicable when assessing how time influences price. We also noticed that there were no prices associated with rows with “cab_type” taxi. After removing unusable or irrelevant data, we are left with 637,976 observations. 
