# Fake News Detection Pipeline using DistilBERT

## Project Overview
This project implements a fake news detection pipeline using the DistilBERT model. It compares against a naive baseline that uses capitalization heuristic.

### Technologies Used
* Python (Pandas, NumPy, Scikit-Learn)
* Hugging Face Transformers (DistilBERT)
* PyTorch
* VESSL AI

### Short Reflection
In the beginning, I had 500 lines of Fake.csv and 500 lines of True.csv, but that took an extremely long time to compute, so I changed the dataset to take in 250 lines of Fake.csv and True.csv each.
Although the dataset decreased by half, the AI model still performed with 100% precision for Fake news classification and had a total accuracy of 92%.
Coming up with the naive baseline standard was the most difficult as I could not figure out a way to accurately identify fake articles. I definitely felt that only an AI model that can study the linguistic
patterns of true articles would be able to identify the fake articles.
For metrics, the recall and precision scores convey the quality of the models most accurately. For example, the overall accuracy for the baseline model is 0.61 despite the fact that it only has a 0.19
recall for fake articles. I do not think the overall accuracy score (especially for the baseline) says much about the results.
Next time, I would like to train the model on a larger dataset and try to increase the recall score for Fake classification and precision for True classification.
---
*Created by Seulbit Park for Yonsei CAS2105 Introduction to Computer Science Research*
