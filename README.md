Subject: 2023W-T2 AML 2203 - Advanced Python AI and ML Tools 01 Group Number: Group 8 Group Members: Varun Sharma, Kelvin Simon, Muhammad Ibraheem, Sarathchandran Santhosh, Ankit Ambikaprasad

Project Name 1: Resume Screening using python: By natural language processing algorithms, we have developed a program capable of screening  resumes in few minute  to identify the best fit for a job opening based on specific criteria or scores.
These programs usually look for specific keywords; they sort resumes and rank them to determine the job applications that should be further reviewed by recruiters. While each company might have its own resume screening system, it is crucial for candidates to know how they work with the aim of improving their keywords selection based on the job opening they are applying to.
The match percentage is displayed on a bar chart, and the predicted job position for the resume is displayed.The application uses the pandas for creating dataframes, nltk for processing the content of resume and matplotlib to plot the chart.


Project Name 2: Fake News Predictor: In this project, we have used various natural language processing techniques and machine learning algorithms to classify fake news articles using sci-kit libraries from python.

Getting started<a name="TOP"></a>
===================

## pre-requisites ##

    You will also need to download and install below 3 packages after you install  python:
Sklearn (scikit-learn) - 
pandas - for creating the dataframes.
nltk - for natural language processing.
re - for searching text in document.

The dataset used for this project were in csv format named train.csv can be found in repo. Below is some description about the data files used for this project.
the dataset containes 5 variables/columns for train, test sets as follows:

Column 1: the unique id for a news article .
Column 2: the title of a news article.
Column 3: the author of the news.
Column 4: the text of the article; could be incomplete.
Column 5: label indicating whether news is fake or not.
       1: Fake news
       0: real News

### File descriptions ###
#### main.py ####

This is the main python file that predicts whether the news is fake or not. In this project the text file is converted into meaningful numbers so that the computer can understand. we are using the vectorize function[TFIDF] TFIDF works by proportionally increasing the number of times a word appears in the document but is counterbalanced by the number of documents in which it is present. Hence, words like ‘this’, ’are’ etc., that are commonly present in all the documents are not given a very high rank. However, a word that is present too many times in a few of the documents will be given a higher rank as it might be indicative of the context of the document.After changing the data into numerical mode, it is fed into machine learning model. The model we are using is logistic regression model. Logistic regression function gives a sigmoid curve and if the predicted value is greater than the threshold value, it will give label as one which means the news is fake and if it is less than the threshold value then it will give label as zero which means news is not fake.




