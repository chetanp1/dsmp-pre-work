### Project Overview

 For this project, we will be exploring the publicly available data from LendingClub.com. Lending Club connects people who need money (borrowers) with people who have money (investors). As an investor one would want to invest in people who showed a profile of having a high probability of paying the amount back.

Problem Statement
What is the probability that the borrower paid back their loan in full?

About the Dataset
The snapshot of the data you will be working on:


### Learnings from the project

 Why solve this project?
After completing this project, you will have a better understanding of probability. In this project, you will apply the following concepts.

Independency check
Bayes theorem
Visualizing discrete variable
Visualizing continuous variable


### Approach taken to solve the problem

 Independence check !
To calculate the joint probability it's very important that conditions are idependent from each other. Les's check whether the condition fico credit score is greater than 700 and purpose == 'debt_consolidation' are independent from each other.

Instructions:
The path for the dataset file has been store in variable path
Load dataset using pandas read_csv api in variable df
Calculate the probability p(A)for the event that fico credit score is greater than 700. and store it in variable 'p_a'.
Calculate the probabilityp(B) for the event that purpose == 'debt_consolation' and store it in variable 'p_b'.
Calculate the purpose == 'debt_consolidation' and store it in dataframe df1.
Calculate the probablityp(B|A) for the event purpose == 'debt_consolidation' given 'fico' credit score is greater than 700 and store it in variable p_a_b.
formula to check the independency P(A|B) == P(A)
check the independency store it in variable result.
Print result

-------------------------------------------------------------------------------------------------------------------------------------------------------------

Bayes theorem
Calculating conditional probabilty is the very important step. Let's calculate the bayes theorem for the probability of credit policy is yes and the person is given the loan.

Instructions:
Calculate the probability p(A) for the event that paid.back.loan == Yes and store it in variable called prob_lp.

Calculate the probability p(B) for the event that credit.policy == Yes and store it in variable prob_cs.

Calculate ['paid.back.loan'] == 'Yes' and store it in variable new_df

Calculate the probablityp(B|A) for the event paid.back.loan == 'Yes' given credit.policy == 'Yes' and store it in variable prob_pd_cs

Calculate the conditional probability where the formala is given below:
P(A|B)=\frac{P(B|A).P(A)}{P(B)}
P(A∣B)= 
P(B)
P(B∣A).P(A)
​	
 
Store the result of the event P(A|B) it in variable bayes

Print the bayes

------------------------------------------------

Purpose vs paid back loan
Let's visualize the bar plot for the purpose and again using condition where

Instructions:
Visualize the bar plot for the feature purpose.
Calculate the paid.back.loan == No and the store the result in dataframe df1
Visualize the bar plot for the feature purpose where paid.back.loan == No

------------------------------------
visualization of continuous variable
Let's plot the histogram for visualization of the continuous variable. So that you will get the basic idea about how the distribution of continuous variables looks like.

Instructions:
Calculte the median for installment and store it in variable inst_median.
Calculate the mean for installmentand store it in variable inst_mean.
plot the histogram for installment
plot the histogram for log anual income


