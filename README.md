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
- FLAIRS Conference: Comparison of BERT, RoBERTa, ELECTRA, XLM-R, and XLNet for fine-grained emotion detection in short social media text. 
- Comparative studies on pretrained models, including BERT, RoBERTa, and DistilBERT, highlighting accuracy, preprocessing effects, and fine-tuning strategies (e.g., Rezapour, 2024).  
- RoBERTa base: pretrained on large English corpora with a masked language modeling objective, producing strong bidirectional representations for sequence classification. (HuggingFace).  

## Methods
Experiments were implemented in Google Colab and include:  

1. Preprocessing and tokenization  
2. Fine-tuning BERT, RoBERTa, and DistilBERT  
3. Monitoring model performance using training loss and validation loss across epochs
4. Evaluation using accuracy, precision, recall, F1 score, and confusion matrices

## Results
For BERT, the model outputs accuracy 0.393, precision 0.3517, recall 0.39, and F1-Score 0.36. It identifies class 12 and 8 the best and underpredicts labels 0-3, this may be caused by lack of data due to resample to 20,000 and lack of epoch that was reduced from 5 to 2.

For roBERTa, the model outputs accuracy 0.376, precision 0.3149, recall 0.376, and F1-Score 0.32. Predicts class 12 and 8 the best and underpredicts 0-4 and 9.

For DistilBERT the model outputs accuracy 0.387, precision 0.3515, recal 0.387, and F1-Score 0.35. Predicts class 5, 8, and 12 the best and underpredicts 0-3 and 11.
