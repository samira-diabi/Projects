# README
---
# Modeling the Madness
### Authors
* Samira Diabi, sdiabi@andrew.cmu.edu
* Amelia Janaskie, ajanaski@andrew.cmu.edu
* Genna Moellering, gmoeller@andrew.cmu.edu
---

### Project Description

March Madness is a 68-team single-elimination tournament of men’s Division I National Collegiate Athletic Association (NCAA) basketball teams. While popular to watch, predicting the tournament outcome has also become popular as many people submit their bracket predictions. The wide array of data and information about teams and games provides fertile ground for people to analyze and predict outcomes. Despite this richness of data, predicting the winner of March Madness is extremely challenging. In fact, the odds of predicting a perfect bracket are 1 in 9,223,372,036,854,775,808. 

Using this rich set of data, we use machine learning models to predict outcomes of the 2023 March Madness and gain insights about team performance. The project implements 12 different machine learning models from Gaussian Naive Bayes to Agglomerative Clustering to answer three questions (see below) about the March Madness tournament. The models found common characteristics that make teams successful as well as reached decent levels of accuracy when predicting what teams will be in the tournament and which teams will win when matched up. Overall, this project provides interesting insights on how to predict March Madness outcomes.

**Keywords:**
basketball, ncaa championship, march madness, brackets

**Questions:**
1. a.) Which teams will make it into the NCAA Men's Basketball Tournament in 2023? b.) Which teams will win each round of the tournament bracket? (Classification with a Target Variable of binary 'Win' column)

2. Have tournament outcomes become harder to predict in the Name Image & Likeness (NIL) Era where NCAA athletes can be paid by universities? We compare probability gaps in game outcomes from previous tournaments to see if prediction windows are becoming tighter and, consequently, game outcomes more uncertain. (Prediction with a Target Variable of win probability for a given team - TeamA)

3. What common characteristics What common characteristics in terms of their performance emerge when teams are grouped together? For example, do all the most successful teams have a certain shooting percentage or number of steals per game? (Unsupervised Learning)

---
### Data Collection

**Competition Description and Data Source:** 
Jeff Sonas, Maggie, Will Cukierski. (2023). March Machine Learning Mania 2023, Kaggle, https://kaggle.com/competitions/march-machine-learning-mania-2023


**Raw Data:**
https://drive.google.com/drive/folders/1QQdON5MN4fGMu_liM8uyWiOxpTmLDrPs?usp=share_link 


Other Data Files: There are multiple datasets that are created and read out at the end, which can be seen in the data folder.

---
### Merging Strategies

Question 1 involved using two different datasets. There were two different notebooks: one to answer question 1a and the other for question 1b. At the end, to merge the  two Jupyter notebooks, the Python library called nbmerge was used. 

To use nbmerge, it was installed in anaconda command prompt:

$ pip install nbmerge

After installing nbmerge, the two notebooks were merged by opening the command prompt, navigating to the directory where the notebooks were located, and running the following command:

!nbmerge "Final Project - Classification Part 1.ipynb" "Final Project - Classification Part 2.ipynb" -o Q1 – Classification_Modeling.ipynb

This command merged the two notebooks and saved them as a new notebook titled "Q1 – Classification_Modeling.ipynb"

Overall, however, merging strategies were limited due to the structure of the project. Each team member had their own notebook that they were working in with minimal overlap. The same rationale applies to branching.

---
### How to Run the Project
Our notebooks are separated by each question since the questions differ in terms of modeling, datasets used, and more. Each notebook will indicate which question it corresponds to (i.e. "Q1-Classification_Modeling.ipynb" indicates question 1). Please read each notebook in the following order:

* Q1-Classification_Modeling.ipynb
* Q2-Prediction_Modeling.ipynb
* Q3-Unsupervised_Learning.ipynb 
 
Note that some code might be #commented out# or indicate a warning if there are long processing times.

Other libraries used: Q1 uses a new library called itertools so this will need to be installed to run the code.
