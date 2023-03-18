## _**Predicting Loan Default in Banks : Mitigating the Risk of Non-Payment**_


### **Project Summary**

Banks earn a major share of their revenue from the interest on loans, but this is often associated with a high level of risk. One of the most significant challenges that banks face is loan defaults. Banks are using forecasting techniques to analyze patterns that are more likely to be present in loan defaulters in order to mitigate this problem. Our dataset is made up of borrowers' past data collected by banks. Our aim is to identify a classification model that could be used to classify borrowers as likely to default or not.

The dataset we chose for our analysis comprises of 148,670 rows with 34 attributes. The attributes describe the nature of the loan and of the borrower. As our first step in the analysis, we excluded missing values, searched for outliers, and even excluded columns that did not contribute to our class of interest. The multivariate analysis using scatterplot matrix also showed some interesting correlations between the predictor variables. Borrowers with a higher property value, for example, are able to claim a larger loan amount. In addition, a higher loan to value ratio (LTV) increases the likelihood of loan defaults. Similarly, a higher debt-to-income (DTIR) ratio suggests a greater risk of default on a loan.

We then tried the classification models on our dataset to determine which model performed the best for our analysis. We compared important metrics for model selection, such as AUC, Accuracy of 1s prediction, Lift, and so on. There are 21 categorical variables and 7 continuous variables in our input variables. Ensemble Model 1 performed well under ROC, with area under the curve being 0.8094, a misclassification rate of less than 13%, and the best accuracy of 1s prediction (83.55%). The Ensemble model was developed by averaging logistic regression, boosted trees, neural networks, boosted forests, & the Naive Bayes Model, resulting in a robust model in nature. Importantly, since each model used is unique, Ensemble model reduces the variance in the predictions, resulting in improved predictive performance.

Finally, we concluded from our data analysis that the loan defaults occurring for business accounts were more as compared to non-commercial loans. Higher LTV values corresponded to high default chances and thus a threshold can be set in order to process future loans. The banks could utilize this analysis to restructure their loan lending process which can be further expanded to other financial systems.

Default in financial systems indirectly impacts the country’s economy as banks function on a large scale. Hence,  it is essential to identify loan defaults to optimize the bank’s profits which could eventually benefit the economy as a whole.


### **Results**

#### _**Best Model : Ensemble Model 1**_

![image](https://user-images.githubusercontent.com/70052374/226123745-6fd00b26-24fc-44ba-824a-ae18b52a35ab.png)


![image](https://user-images.githubusercontent.com/70052374/226123800-04171255-866d-4861-8bb9-e1c6f81c6931.png)


![image](https://user-images.githubusercontent.com/70052374/226123804-b1b16d5e-751f-49c6-9583-6d22ea78b1f0.png)


* Overall, our Ensemble Model 1 has performed well under the ROC with an AUC of **0.8094**, a misclassification rate of about **13%**, and the best accuracy of 1s prediction of **83.55%**. The Ensemble model was created by averaging logistic regression, boosted trees, boosted forest, and Naive Bayes Model making it robust in nature. Significantly, as each model used differs from each other, Ensemble reduces the variance in the predictions leading to improved predictive performance.


### **Conclusions**

**a) LTV vs Loan Default Status**


<img width="266" alt="image" src="https://user-images.githubusercontent.com/70052374/226123214-1ec3c19b-f2e4-4427-88a1-3f045a001c9b.png">


* Loan-to-Value (LTV) ratio is the relation between the amount of loan granted to the customer and the value of property pledged as collateral. A higher LTV ratio indicates that the borrower is more likely to lack sufficient collateral. As can be observed from the picture, borrowers who made loan defaults had a higher median value for LTV than borrowers who did not make loan defaults.



**b) DTIR vs Loan Default Status**

<img width="266" alt="image" src="https://user-images.githubusercontent.com/70052374/226123239-3668a497-7e4b-401f-9de7-be038e38b8c8.png">


* Debt-to-Income ratio (DTIR) compares the borrower's monthly debt payments to their monthly income. A higher Debt-to-Income ratio indicates lower income for the borrower, and in unforeseen circumstances, borrowers with lower incomes are more likely to default on the loan. As shown in the picture, borrowers with a higher median DTIR have defaulted on their loans.




**c) Loan Type vs Loan Default Status**

<img width="314" alt="image" src="https://user-images.githubusercontent.com/70052374/226123357-07d0a8b4-fe90-4f63-9f64-390bc7747e97.png">


* The loans have been classified into two types, namely commercial/business loans and non-commercial loans. It is observed that the ratio of defaults to non-defaults for commercial/business loans is **0.396**, whereas for non-commercial loans it is **0.171**. This indicates that a higher percentage of business loans are defaulted on when compared to non-commercial loans.


### **Recommendations**


* **For existing customers :**

**a)** Borrowers could be asked by banks to restructure their loan repayment model in order to reduce defaults while extending the loan term. This could result in fewer loan defaults and increased revenue for the bank in the form of higher interest paid by the borrower due to the term being extended, leading to higher overall profitability for the banks.



* **For new loan applications :**

**a)** The LTV ratio threshold above which loan applications would not be processed could be lowered by banks. If the LTV ratio exceeds the threshold, there is a greater risk of loan default, which can have an impact on the bank's profitability.


**b)** Banks must ensure that all of the borrower's debts have been included in the credit history, in addition to the DTIR ratio which evaluates the individual's income. If certain debts are not included in the credit history but are still owed, the DTIR ratio will remain low despite a higher risk of loan default. Hence, a comprehensive profile evaluation should be part of the approval process.


**c)** When approving the loan, the borrower's age should be considered. If the borrower is over the age of 50, for example, the loan term should be set so that the borrower can repay the loan before retiring. Lump-sum repayments could be incorporated into the loan structure. Furthermore, the maximum borrowing limit set for such borrowers should be lower than that of a typical borrower.