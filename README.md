# CS 224N Final Project - Multitask BERT

In this project,  I implement components of the BERT model and use the embeddings produced on downstream tasks: sentiment classification, paraphrase detection and semantic similarity.

## Implementation
Input sentences are tokenised using the WordPiece tokenizer and are padded to length 512. Tokens are given ids and passed to a trainable embedding layer of dimension 768. These are passed to the Encoder Transformer layer, where I implement multi-head self-attention, a feedforward network and LayerNorm.
The model outputs final embeddings for the input text.

## Datasets
- Stanford Sentiment Treebank (SST) for sentiment classification
- CFIMDB for binary sentiment classification
To finetune BERT for sentiment classification, I implement the Adam optimizer algorithm.

- Quora dataset for paraphrase detection
- SemEval dataset for semantic textual similarity detection




