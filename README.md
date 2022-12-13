### Quintilian at SemEval-2023 Task 4: ValueEval: Identification of Human Values behind Arguments

Group members:
Hemanth Chenna
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
![Comparison of individual test set $F_1$ scores for each of the labels by the different models we have trained and tested](https://github.com/HemanthCU/NLP_SharedTask_Task_4/blob/main/Results/F1-Comparision.png)
