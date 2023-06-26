# BART_LSG

## Abstract
Summarization is a challenging task in Natural Language Processing (NLP) that involves producing shorter versions of documents while capturing their main essence. In this project, we focus on summarizing legal documents using extractive and abstractive summarization techniques. The goal is to provide meaningful summaries that can save time for legal professionals and aid in finding precedence for ongoing cases.

## Introduction
Legal documents, often lengthy and complex, pose challenges for legal workers and clients. Reading through thousands of words to find relevant information can be time-consuming. To address this issue, we aim to leverage NLP advancements and develop techniques for summarizing legal documents. Our project explores both extractive and abstractive summarization methods.

## Motivation
The production of legal information is extensive, with numerous courts generating large quantities of documents. In India alone, there are 25 High Courts and 672 District Courts that publish legal reports publicly. With the use of automatic text summarization techniques, legal practitioners can benefit by reducing manual effort and quickly finding relevant information or precedence for ongoing cases.

## Design of Approach
Our approach involves leveraging the BART (Bidirectional and AutoRegressive Transformers) model with an enhanced attention mechanism called LSG (Local, Sparse, and Global) attention. We extrapolate the existing pretrained BART model to handle longer sequences by integrating LSG attention, which has a linear time complexity. We fine-tune this model on Indian legal datasets for both extractive and abstractive summarization. The extractive summarization is performed using a

 BERT-based model to identify important sentences, while the abstractive summarization is performed using BART with LSG attention to generate concise summaries.

## Dataset
We use a dataset consisting of 1,000 full legal case documents and their corresponding abstractive summaries. The dataset was crawled from the Indian Supreme Court's official website, ensuring the availability of diverse legal topics and precedents.

## Evaluation
We evaluate the performance of our hybrid model using standard evaluation metrics such as ROUGE (Recall-Oriented Understudy for Gisting Evaluation). Additionally, we consider the feedback of legal professionals to assess the practical utility and accuracy of the generated summaries.

## Conclusion
This project aims to develop an effective approach for legal document summarization using both extractive and abstractive techniques. By providing shorter and meaningful summaries, we strive to enhance the efficiency of legal professionals in navigating and understanding complex legal documents.

## References : 
1. Hugging Face - Summarization Tasks: [Link](https://huggingface.co/tasks/summarization)
2. Two-Stage-Sum GitHub Repository - Model Image: [Link](https://github.com/GeekAlexis/two-stage-sum/blob/main/assets/535%20model.png)
3. Elsevier - "Long Document Summarization Using Deep Learning": [Link](https://reader.elsevier.com/reader/sd/pii/S1319157820303712?token=F6B14B0B0C3130C6FC66848D4DFC0F607E5E7EF936E330D858AC963E68A23503652E20EE72B55A371E76275F3DD1originRegion=us-east-1&originCreation=20230324090157)
4. Cinnamon AI - "Bootcamp Tech Blog #4: Long Document Summarization": [Link](https://cinnamonai.medium.com/bootcamp-tech-blog-4-long-document-summarization-6bc25e3add94)
5. IIT-RD - "A Survey on a Hybrid Method for Query-Based Automatic Summarization System for Text" (PDF): [Link](http://www.iit-rd.com/FinalPaper/FinalPaperA%20Survey%20on%20A%20hybrid%20method%20for%20query%20based%20automatic%20summarization%20system%20for%20text150046.pdf)
6. BERT Extractive Summarizer GitHub Repository: [Link](https://github.com/dmmiller612/bert-extractive-summarizer)
7. Medium - "Techniques for Extractive and Abstractive Text Summarization": [Link](https://medium.com/@devilchauhan0/techniques-for-extractive-and-abstractive-text-su)
8. Kaggle - Extractive and Abstractive Text Summarization: [Link](https://www.kaggle.com/code/abhinavkrjha/extractive-and-abstractive-text-summarization)
9. Medium - "Fine-Tuning a Chat Summarizer": [Link](https://medium.com/@ferlatti.aldo/fine-tuning-a-chat-summarizer-c18625bc817d)
10. Width.ai - BART Text Summarization: [Link](https://www.width.ai/post/bart-text-summarization)
11. LSG - [Link](https://github.com/ccdv-ai/convert_checkpoint_to_lsg)

