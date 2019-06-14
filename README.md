# Salary-Prediction-from-Name

DATASETS:
1)LinkedIn dataset (2016 - 2018): 
The Original dataset had 2 million records (~10GB)but we have considered  most recent jobs in the bay area(38,606 entries)for modeling.
reference (Yutao Zhang, Jie Tang, Zhilin Yang, Jian Pei, and Philip Yu. COSNET: Connecting Heterogeneous Social Networks with Local and Global Consistency. In Proceedings of the Twenty-First ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD'15 ).

2)US Bureau of Labor Statistics - Salary dataset (2018):
36,897 entries in salary data
802 types of jobs in California
https://www.bls.gov/oes/current/oes_ca.htm




The application consists of 2 models in a pipeline:

1)Neural Machine Translation with attention to predict job from name 
Input pairs: full name ⇒ job title (similar to the pairs of English ⇒ French).
Encoder/Decoder mechanism. 
GLoVe word embedding, <start> <end> indicators.

2)MLP network to predict salary from job (regression problem).
Pretty simple model with several dense layers with different numbers of connected neurons and ReLU activation function.
The last layer is a dense layer with one output as the predicted salary.

