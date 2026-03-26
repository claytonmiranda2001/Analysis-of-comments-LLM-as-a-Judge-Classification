#LLM as a Judge – Comment Classification

##Project Objective

This project aims to demonstrate the usability of a Large Language Model (LLM) as a judge or classifier.
A small dataset was used due to the computational cost of running the llama3:8b model locally via Ollama.

It is important to highlight that the goal is not to evaluate model performance, as the dataset size is not sufficient for a robust assessment.
The dataset was obtained from Kaggle.

##DataFrame Creation

A DataFrame was created containing:

*5 positive examples
*5 negative examples

This setup was designed to validate whether the LLM correctly understands and follows the provided instructions.

##Calling the LLM

The model was executed using Ollama with a structured prompt that defines:

*Expected inputs
*The role the LLM should assume
*The objective of the task
*The comment to be evaluated
*Labeling rules
*Instructions
*Expected output format ("positive" or "negative")

##Conclusion

The LLM correctly classified 9 out of 10 cases and followed the required output format in all responses.

These results suggest that this approach can be scaled to larger datasets, not only for sentiment analysis but also for various types of text classification tasks.

##Technologies Used

*Python
*Pandas
*Matplotlib
*Seaborn
*Sklearn
*Ollama (llama3:8b)
