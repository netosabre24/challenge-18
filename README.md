# Cryptocurrencies

# Overview

The purpose of this project is to create a analysis of cryptocurrency data for clients who are wwanting to invest into the crypto market. The data will be grouped together and visualized to help classify and understand the different types of cryptocurrencies on the market. For this analysis, unsupervised machine learning and its different algorithms will help guide us through this analysis.

# Analysis and Results

**Deliverable 1**

First step is to load the data and clean it up, then we filter the data by getting only the cryptocurrencies that are currently being traded, get working algorithms and some mined coins. Then remove any unecessary columns and any rows that have null values.
*Dataframe shown below*


![Pic1](https://user-images.githubusercontent.com/82550431/136467788-cd9c2fbc-2843-483e-afe5-2b673f83974d.PNG)


**Deliverable 2 & Deliverable 3****

Using the pd.get_dummies() command will create integer values and replace the two string columns, because the ML algorithms we'll be using can't process strings. Then reduce the different features from 4 decreasing to 3 principal components using PCA (Principal Component Analysis). Now we can run the K-Means algorithm that will help us identify and pick how many clusters our day will fit into.

![pic2](https://user-images.githubusercontent.com/82550431/136468432-2bf14917-7f23-4ea5-960a-831150f0e679.PNG)

In the line graph above, we can see small slant at both k = 4 and 5.
After running the algorithm with our clusters set to 4, then we put it it all into a dataframe. *Shown below*

![pic3](https://user-images.githubusercontent.com/82550431/136468443-f840eb95-f512-47ed-9131-27116ef74e68.PNG)

**Deliverable 4**

Using the data frame above, we can use plotly library to plot a 3d scatter plot.

![pic4 (2)](https://user-images.githubusercontent.com/82550431/136493010-5e71f367-3ed9-4529-8175-6a7c06ac7b49.png)

To help visualize our different types of cryptocurrencies, the data is scaled using the MinMaxScaler() method, then plot it on the regular scatter plot using hvplot. *shown below*

![pic5](https://user-images.githubusercontent.com/82550431/136468481-51f61be2-0281-4e06-842d-c78e6001c238.PNG)

# Summary 
Using unsupervised machine learning, we can cluster our data in
