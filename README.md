# Authurship-Attribution-For-Ancient-Greek-Classics
Navie Bayes and Random Forest Classifition for Ancient Greek Literature

## Introduction  <a name="introduction"></a>
### Problem Area <a name="problem_area"></a>
Authorship attribution  has been a long-standing problem in the field of Ancient Greek literature study. Scholars have made a lot of effort in determining the genuine authorship of anonousy works, and giving answer to literatures of debated authorship. However, authorship attribution can be seen as a kind of text classification using statistics method, in which the authors are the categories to which each text is to be classified.

Statistical analysis of texts for author determination starts in in the late nineteenth century with the works of Mendenhall and Mascol. Computerized analysis of lexical features for authorship determination, however, shows its potential when Mosteller and Wallace applied Naive Bayes model, by analysing vairous lexical features, to determine the authorship of Federalist Papers in 1964. 

Currently, there are two approaches for lexical-based text-classification, as Stamatatos suggests in 2001. The first method is to measure the richness of vocabulary of authors. Another is based on the occurrence of individual words.

In this study, we made attempts to address this issue by using two machine learning model: Navie Bayes and Random Forest, with feature extraction method based on the occurrence of words.

### Objective <a name="objectives"></a>
This study aims to address the authorship attribution problems in Greek Literature. We would first train a model using works with known authorship, and thereby try to give from the persepective of computational linguistic answers to the authorship of contested Greek works. 

### Dataset <a name="dataset"></a>
We select 77 works from fourteen ancient Greek authors that ranged from 8th BCE to 3rd CE. The topics covered include religons, philosophy, myth, history, drama, while the genres include poetry, prose, epic, comedy, tragedy, history and biography. The corpus are represented as plain text in .txt format. The dataset was obtained from Wikisource and Project Gutenberg. A list of data source is included in the `Reference` section.

### Evaluation methodology <a name="evaluation_methodology"></a>
We use Precision, Recall, F1-score and Accuracy to meausre the performance of our model. However, Recall and accuracy are considered as the most important measurements in this study.


## Result
For our model, TF-IDF measurement is used as the representation of corpus. The Navie Bayes model achieves 76% accuracy in authorship attribution by using, while the Random Forest model achieves 91% accuracy.

### Random Forest
#### Confusion Matrix for Random Forest Model
![](https://github.com/katcom/Authurship-Attribution-For-Ancient-Greek-Classics/blob/main/IMG/random_forest_confusion_matrix.png | width=200px)

#### Classification Performance Report
![](https://github.com/katcom/Authurship-Attribution-For-Ancient-Greek-Classics/blob/main/IMG/random_forest_report.PNG | width=200px)

### Naive Bayes
### Confusion Matrix for Random Forest Model
![](https://github.com/katcom/Authurship-Attribution-For-Ancient-Greek-Classics/blob/main/IMG/naive_bayes_confusion_matrix.png | width=200px)

### Classification Performance Report
![](https://github.com/katcom/Authurship-Attribution-For-Ancient-Greek-Classics/blob/main/IMG/naive_bayes_report.PNG | width=200px)
