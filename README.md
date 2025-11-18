# COMP560FinalProject - Emotion Detection Using Transformer-Based Generative Models

## Overview
This project explores emotion detection from text using Transformer-based language models. We compare multiple pretrained architectures—including BERT, RoBERTa, and DistilBERT—and evaluate whether a generative Transformer approach can improve classification accuracy.

## Dataset
We use the Kaggle dataset “Emotion Detection from Text,” containing samples labeled with emotions such as joy, sadness, and anger. Each entry includes:
- content (snippet of text)  
- id (unique identifier)  
- target (emotion)  

## Related Work
We reviewed studies on emotion classification and Transformer architectures:  
- FLAIRS Conference: Comparative analysis of BERT, RoBERTa, ELECTRA, XLM-R, and XLNet for fine-grained emotion detection in short-text social media data.  
- Comparative studies on pretrained models, including BERT, RoBERTa, and DistilBERT, highlighting accuracy, preprocessing effects, and fine-tuning strategies (e.g., Rezapour, 2024).  
- Study of generative Transformer approaches to model complex emotional patterns in text.  
- RoBERTa base model: pretrained on large English corpora using a masked language modeling (MLM) objective; learns bidirectional sentence representations and is fine-tuned for tasks like sequence classification (HuggingFace).  

These works highlight the strengths of contextual embeddings and motivate our comparison of BERT-family models.

## Methods
Experiments were implemented in Google Colab (`roBERTa_stuff.ipynb`) and include:  
1. Preprocessing and tokenization  
2. Fine-tuning BERT, RoBERTa, and DistilBERT  
3. Training a small generative Transformer variant  
4. Evaluating performance across models  

## Results
fill this in

## Conclusion
This study demonstrates the effectiveness of pretrained Transformers for emotion detection and explores generative models for improvement.
