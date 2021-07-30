## Sentiment analysis using Pytorch and BERT

###  Dataset
IMDB dataset consists of 50k movie reviews. 25K positive reviews and 25k negative reviews (balanced dataset).

Link: http://ai.stanford.edu/~amaas/data/sentiment/ 

Transformers library from HuggingFace was used for bert model. Pytorch dataset and dataloader classes were used to process and load the dataset.

### Hyperparameters
Pre-trained model : bert-base-uncased\
Loss function : Cross-entropy loss\
Optimizer : AdamW\
train-test-split : 0.5\
Evaluation metric : Accuracy\
Epochs : 5\
Batch size : 16\
Maximum token length : 256

### Model architecture
The embedding of the CLS token from the bert model was passed through a linear layer to get the sentiment
![alt text](./images/bert_sentiment_flow_diagram.png?raw=true)