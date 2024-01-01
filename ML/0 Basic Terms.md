---
status:: Published
summary: Summary of the post
tags: 
	- post 
	- ML
alias: 
	- intro
creation_date: Sunday, 4th December 2022, 15:15:40
Progress: 80
Target: 100
---
%%
Bar::  <progress max=100 value=100> </progress> 100%
%%

In these series of articles we will talk about ML algorithms and implement them in python and the main focus of these articles is to understand math and logic behind these algorithms. We will start by understanding basic terms of ML. 

#### 1. Classification Algorithms
As the name suggest these are classification algorithms that **categorizes the data into different category**. It is a Supervised Learning technique.

#### 2. Supervised Learning 
Supervised learning is associated with **learning with supervision or training**. In supervised learning, the algorithms are trained with data which is labeled or classified.

#### 3. Unsupervised learning 
Unsupervised learning is associated with **learning without supervision** or training. In unsupervised learning, the algorithms are trained with data which is neither labeled nor classified. In unsupervised learning, the agent needs to learn from patterns without corresponding output values. 

#### 4. Cross-Entropy Loss
Is **a metric used to measure how well a classification model in machine learning performs**. The loss (or error) is measured as a number between 0 and 1, with 0 being a perfect model.

#### 5. Condition positive (P)
The number of real positive cases in the data

#### 6. Condition negative (N)
The number of real negative cases in the data

#### 7. True positive (TP)
A test result that correctly indicates the presence of a condition or characteristic

#### 8. True negative (TN)
A test result that correctly indicates the absence of a condition or characteristic

#### 9. False positive (FP)
A test result which wrongly indicates that a particular condition or attribute is present

#### 10. False negative (FN)
A test result which wrongly indicates that a particular condition or attribute is absent

#### 11. Confusion Matrix
It provides us the result of our model in matrix form (as shown below). We use this to measure accuracy of the mode.

|                    | Actual positive | Actual Negative |
|:------------------ |:---------------:| ---------------:|
| Predicted Positive |  True Positive  |  False Negative |
| Predicted Negative | False Negative  |   True Negative |

#### 12. Area Under the Curve (AUC)
Is the area encapsulated between the curve and x-axis. 
![[ML/assets/0 Basic Terms/image-0 Basic Terms-030351285.png|500]]



#### 13. Receiver Operating Characteristic (ROC) 
> The receiver operating characteristic (ROC) curve, which is defined as a plot of test sensitivity as the y coordinate versus its 1-specificity or false positive rate (FPR) as the x coordinate 

$$
ROC = \frac{hits}{hits + misses}

$$

![[ML/assets/0 Basic Terms/image-0 Basic Terms-024646901.png|500]]
This image from Wikipedia shows exact definition of ROC.



If you want me to include any other terms in this article comment them and I will do my best to include them. 
## References

- https://www.javatpoint.com/classification-algorithm-in-machine-learning
- Park SH, Goo JM, Jo CH. Receiver operating characteristic (ROC) curve: practical review for radiologists. Korean J Radiol. 2004 Jan-Mar;5(1):11-8. doi: 10.3348/kjr.2004.5.1.11. PMID: 15064554; PMCID: PMC2698108.
- https://en.wikipedia.org/wiki/Receiver_operating_characteristic
- https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc
