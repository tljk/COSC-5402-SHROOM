## Parsed data  
JSON file
## Results
XLSX file

# Hand Labeled Baseline

This branch contains code used to produce the results for the hand labeled baseline. This process consisted of manually labeling 200 samples for each task present in the training data (definition modeling, paraphrase generation, and machine translation). With this small labeled training set, we could then experiment with simple models like KNN, SVM, and logistic regression for hallucination classification.

## Files

* silverDataTraining.csv: 600 hand-labeled samples, 200 for each task
* silverDataTraining_embeddings.csv: the mBERT embeddings for the source, target, and hypothesis texts for each hand-labeled samples
* train.csv: the unlabeled SHROOM training set
* silverData.ipynb: code to process and generate the silver data. This is all consolidated into a single file, with explanations throughout the code file.
* silverData.csv: the pseudo labeled training data
* embeddingBatches: directory of batches for the training set; too bulky to upload