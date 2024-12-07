# CYSE635-Group7-DataBusters
**Authors: Macky Castro and Kurt Karpin**

## Introduction

This repo consists of the CYSE 635 AI Security and Privacy course project covering the topic of Data Poisoning on datasets like phishing email. This process is split up into three parts:

1.  Email Dataset Setup and Preprocessing
2.  Initial Model Training and Analysis
3.  Data Poisoning Attacks
4.  Comparitive Analyis of two models being used: Random Forest Classifier and Support Vector Machine

![Group9-Model](img/Group9-Diagram-Workflow.png)


## Data Poisoning Attacks
Two approaches were conducted on attacking an email dataset.

- Approach 1: Conventional Data Poison method - inserting data poisoned row. This inserts duplicate rows of the dataset and flipping the labels. Up to twice the amount of training data were duplicated with flipped labels. Because the dataset contains more than $18k rows of email content, this process would take a collective of 1 1/2 hours to train both models with as much as twice the original training data being added.
- Approach 2: Keyword changing - this is more of a precise data poisoning attack method, where keywords of the email was taken and manipulated by swapping them over to the oppsite of the gender. For example, the word 'money' is the most common used word amongst phishing emails. We would apply this to critical spots in the safe email dataset for the desired goal of having the model misclassify the emails. 
