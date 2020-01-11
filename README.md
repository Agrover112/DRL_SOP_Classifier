# DRL_StatementOfProcedure_Classification(SOP)

Libraries: sklearn,numpy,pandas,eli5,seaborn,matplotlib,spacy.

**The following repository contains the code to the classifier for action classifcation task**.
### Data Analysis
- A corpus of **2K sentences** labelled sentences consisting of valid and invalid SOPs collected from DRL web portal
used for SOP generation.

- Dataset was unbalanced *random sampling* was used for balancing the dataset , has drawbacks.

### Feature Extraction

  Performed using *TF-IDF* measure with smoothing.
  
  Nature of dataset prevented from applying techniques such as *Stemming,Normalization or StopWords removal*(requirement).
 
 ### Models Used
 All models were tuned on dev set and performed well on test set.
 
 - LSVM-Support Vector Machines
 - MNB-Multinomial Naive Bayes 
 - LR-Logistic Regression

