# Building-Gray-Area-Interval-for-Lung-Cancer-Detection
This is not an open source project, and hence the data will not be provided. The data are collected in the laboratory where they apply a new biotech product on
artificial mutated cells. These cells are thought to be related to Lung Cancer. Hence, by assuring the quality control of the product and acquiring the mutation
index measured by such product, we can then observe some of the interesting insights throuhg exploratory data analysis and construct models for predicting lung cancer from medical data. Lastly, several methods are propose to estimate the gray-area
of the reaction of such product. If the index fall in this range, it means that the diagnosis is ambiguous and other inspections should be taken.

Problem:
1.Test whether the quality of the product is stable.
2.Construct interval estimation for 50 different mutated cells.

Conclusion:
1.The product is proved stable under both parametric and nonparametric statistical tests.
2.The variance of the performance between the cells and within the cells are extremely large. Though obvious pattern shown in most data, it is still risky to 
allow any False-Positive prediction in medical data.
3.The lower bound of the gray-area is rather easy to estimate throughout the whole project.
4.However, the upper bound is controversial. Instead of opting for max(x) (Wide gray area, low False-Positive) or machine learning and statistical modeling (accurate but strict),
we proposed methods with logistic regression and bootstrapping embodied to simulate a sampling distribution of 50/50 lung cancer. In such case, the methoud is robust
throughout different cells and time.
5.Given the fact that the product can be produced cost-efficient in the future, the gray-area can be somehow relaxed to allow larger ambiguity but lower False-Positive conclustion.
If the index fall in this robust gray-area, the patient will be then asked to take the test again or other medical action would be taken to investigate such case.
