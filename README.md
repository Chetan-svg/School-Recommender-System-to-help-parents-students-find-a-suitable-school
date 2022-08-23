# School Recommender System to help parents/students find a suitable school


## Background & Objectives of Project:
For student hoping for higher studies in other countries, university selection process is a challenging task as lot of different criteria needs to considered during application process based on individual’s requirement.We built a recommender system for this problem, based on various classification algorithms.Based on the student dataset and user profile, a list of 10 best universities will be suggested such that the chances of a student getting admission into those universities is maximum.

## DataSet:
Choosing the data set is one of the most important part for building a recommender system.www.thegradcafe.com was the source of graduate student data of this project and the Undergraduate student data for this project was scraped from https://collegescorecard.ed.gov/data/.

## Analysis & Methodology:
Here I have used Knowledge based recommendation System where User inputs are taken into account and compare with the training data.

For Graduate University Recommendation I have used Case based knowledge recommendation as it will take the User inputs and compare with trained data.

For Undergraduate Recommendation System, I have used Constraint based Knowledge recommendation system where user inputs taken into account as constraints and based on the constraints we will compare with trained data.

## Models:
I used two different models like K-Nearest Neighbors and Feature weighted algorithms.

## K Nearest Neighbor: 
In KNN, the trained data is compared with test data and distances are calculated using Euclidean distance. It then classifies an instance by finding its nearest neighbors and recommend the top n nearest neighbor universities. Algorithm is stated as below.

1. Initialize the value of k
2. For getting recommendation, iterate from 1 to number of trained data
1. Calculate distance between test data and each row
2. Sort the distances in ascending order
3. Get top k rows and recommend to the user

# Feature weighted algorithm: 
The weightage of all the features are taken and find the similarity score. Based on the similarity score, the universities with highest similarities will be recommended to student. Suppose w1, w2 are weights and f1 and f2 are features the similarity is calculated by formula
Similarity score = w1* f1+w2*(1-f2)

## Web Application:

The Web aplication is created using python Flask and Bootstrap framework

Once the application is running, The home page will appear as below.


## Under graduate Recommendations

![Home Page](/images/home.png?raw=true "Optional Title")
2. click on the Undergraduate University button , you will be redirected to Under Graduate recommendations page as below.
![Undergraduate Page](/images/ug.png?raw=true "Optional Title")

3. Provide the SAT Score ,Maximum tution fees and submit, then you will be redirected to recommendations page.
![Under Graduate Recommendations Page](/images/ug_recommendations.png?raw=true "Optional Title")

## Graduate Recommendations:

1. Click on the graduate Universities from the top Nav bar, then you will be redirected to graduate page
![Graduate Page](/images/grad.png?raw=true "Optional Title")

2. We need to provide Gre scores and cgpa of Under graduation , then click on Submit
![Graduate Recommendations Page](/images/graduate_recommendations.png?raw=true "Optional Title")

