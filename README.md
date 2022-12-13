### Quintilian at SemEval-2023 Task 4: ValueEval: Identification of Human Values behind Arguments

Group members:
Hemanth Chenna, 
Ajay Narasimha Mopidevi

Task:
Task 4: ValueEval
https://touche.webis.de/semeval23/touche23-web/index.html


# Proposed Architectures:


1. <b>L-label classifier</b>: The output of final classification layer is L(=20) nodes 
<p >
  <img width="360" height="320" src="https://github.com/HemanthCU/NLP_SharedTask_Task_4/blob/main/Results/Llabel.png" alt = "L-label classifier" title="L-label classifier">
</p>

2. <b>L-Binary classifiers</b>: L-binary classifier each handling the prediction for a label
<p >
  <img width="360" height="320" src="https://github.com/HemanthCU/NLP_SharedTask_Task_4/blob/main/Results/L-binary_label.png" alt = "L-Binary classifiers" title="L-Binary classifiers">
</p>

3. <b>Grouped classifier</b>: Combined a subset of labels based to commonality, created grouped layers and finally the labels are predicted with binary classifiers within the group.
<p >
  <img width="360" height="320" src="https://github.com/HemanthCU/NLP_SharedTask_Task_4/blob/main/Results/Grouped_label.png" alt = "Grouped classifier" title="Grouped classifier">
</p>



# Results:

<i>Performance of aour approaches compared to the baseline </i>

| Model | Precision | Recall | F1 | Accuracy |
| --- | --- | --- | --- | --- |
| 1-Baseline | 0.18 | 1.0 | 0.28 | 0.18 |
| SVM | 0.30 | 0.30 | 0.3 | 0.77 |
| BERT | 0.39 | 0.30 | 0.34 | 0.84 |
| L-label classifier | 0.29 | 0.48 | 0.36 | 0.76 |
| L-Binary classifiers | 0.3 | 0.45 | 0.35 | 0.77 |
| Hybrid + CE loss | 0.32 | 0.42 | 0.39 | 0.77 |
| Hybrid + CE + HD loss | 0.33 | 0.43 | 0.40 | 0.77 |






<i>Comparison of individual test set F1 scores for each of the labels by the different models we have trained and tested</i>

![Comparison of individual test set $F_1$ scores for each of the labels by the different models we have trained and tested](https://github.com/HemanthCU/NLP_SharedTask_Task_4/blob/main/Results/F1-Comparision.png)
