# Email spam classification

Simple project, classify emails as spam or not-spam using an encoder-only transformer-based model with 2 layers and 4 heads. 

Tiktoken for BPE-encoding and Pytorch modules for everything except the higher-level model implementation. For more grass-roots implementations see my "neural network from scratch" and "LLM from scratch" repositories.

Uses dataset by Meruvu Likith, [text](https://www.kaggle.com/datasets/meruvulikith/190k-spam-ham-email-dataset-for-classification?resource=download). 
The dataset has an approximately 50-50 split of spam and not-spam. 


### Results
The model reached 0.96 testing accuracy with 3 epochs of training. After this it appeared to start overfitting to the training data.

Increasing dropout to 0.3 and training for 10 epochs led to a testing accuracy of 0.97. Unsurprisingly there was less overfitting.

