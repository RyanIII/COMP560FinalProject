# COMP560FinalProject - Emotion Detection Using Transformer Models

## Overview
This project explores emotion detection from text using Transformer-based language models. We compare multiple pretrained architectures including BERT, RoBERTa, and DistilBERT,to determine which models best capture emotional content in short text.

## Dataset
We use the Kaggle dataset “Emotion Detection from Text,” containing samples labeled with emotions such as joy, sadness, and anger. Each entry includes:
- content (snippet of text)  
- id (unique identifier)  
- target (emotion)  

## Related Work
We reviewed studies on emotion classification and Transformer architectures:  
- FLAIRS Conference: Comparative analysis of BERT, RoBERTa, ELECTRA, XLM-R, and XLNet for fine-grained emotion detection in short-text social media data.  
- Comparative studies on pretrained models, including BERT, RoBERTa, and DistilBERT, highlighting accuracy, preprocessing effects, and fine-tuning strategies (e.g., Rezapour, 2024).  
- RoBERTa base model: pretrained on large English corpora using a masked language modeling (MLM) objective; learns bidirectional sentence representations and is fine-tuned for tasks like sequence classification (HuggingFace).  

These works highlight the strengths of contextual embeddings and motivate our comparison of BERT-family models.

## Methods
Experiments were implemented in Google Colab and include:  

1. Preprocessing and tokenization  
2. Fine-tuning BERT, RoBERTa, and DistilBERT  
3. Monitoring model performance using training loss and validation loss across epochs  

Each individual model was trained in a separate Jupyter Notebook

Bert: https://colab.research.google.com/drive/1oEduzuCU6EvOdo9q7Q-QH4c52dq_MXyw 

## Results
For BERT, the model outputs accuracy 0.393, precision 0.3517, recall 0.39 and F1-Scire 0.36. It identifies class 12 and 8 the best and underpredicts labels 0-3, this may be caused by lack of data due to resample to 20,000 and lack of epoch that was reduced from 5 to 2. 

## Conclusion
This study demonstrates the effectiveness of pretrained Transformers for emotion detection and provides a comparative analysis of BERT, RoBERTa, and DistilBERT.
