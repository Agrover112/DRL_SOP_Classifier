# DRL_Statement_Of_Procedure_Classification(SOP)

**The following repository contains the code to the classifier for action classifcation task**.
### Data Analysis
- A corpus of **2K sentences** labelled sentences consisting of valid and invalid SOPs collected from DRL web portal
used for SOP generation.

- It was partially cleaned by data collector.

- Dataset was unbalanced *random sampling* was used for balancing the dataset , has drawbacks.
![](Images/TotalSentences_DRL.PNG)

### Text Feature Extraction

  Performed using *TF-IDF* measure with smoothing.
  
  Nature of dataset restricted me  applying techniques such as *Stemming,Normalization or StopWords removal*(requirement).
  The above cleaning techniques can be applied depending on the use case.
  
 
 ### Models Used

 All models were fine tuned on dev set and performed well on test set.
 
 Ensemble models yielded poor performance.
 
 
 - **LSVM**:Linear Support Vector Machine
 - **MNB** :Multinomial Naive Bayes 
 - **LR** :Logistic Regression
 
 **Visualizing SVM's learned weights** 
 
 ![](Images/Word_Weights(SVM).PNG)

### Classification Results

 **Note:** Results may vary based on corpus size and type.
 
**~89% accuracy** was produced as a result of classification using SVM on test set.(*Actual Test set is not used here.*)

**PCA/TSNE** dimensionality reduction techniques were used to visualize results.

 ![](Images/ClassificationViz_SVM.PNG)
