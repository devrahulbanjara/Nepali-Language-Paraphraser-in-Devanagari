# Nepali -Language-Paraphraser-In-Devanagari-Dataset-Preparation

This repository contains the steps and resources used to prepare a Nepali paraphrase dataset by leveraging English paraphrase datasets and machine translation.

## Overview

To build a dataset for fine-tuning a multilingual language model to paraphrase Nepali sentences (in Devanagari script), we started with two well-known English paraphrase datasets:

- **Quora Question Pairs** (~400,000 pairs of questions)
- **PAWS Wiki Labeled Dataset** (~50,000 pairs of sentences including questions and answers)

Using these datasets helped cover diverse types of paraphrases, including questions and general sentence pairs.

## Data Preparation Steps

1. **Extract sentence pairs**  
   We extracted the paired sentences from both datasets (questions from Quora and sentences from PAWS) into separate plain text files.

2. **Translate sentences from English to Nepali**  
   Using the `deep-translator` API, half of the dataset (approximately 200,000 sentence pairs) was translated from English to Nepali, creating Nepali sentence pairs corresponding to the original English pairs.

3. **Back-translation to increase data diversity**  
   The remaining 200,000 sentence pairs were generated using back-translation techniques to further diversify the dataset and improve paraphrasing quality.

4. **Recombine translated and back-translated pairs**  
   Both sets of Nepali sentence pairs were combined and shuffled to ensure a diverse mix of paraphrase examples.

5. **Split into training, validation, and test sets**  
   The final dataset of approximately 400,000 Nepali paraphrase pairs was split into:
   - 300,000 pairs for training  
   - 10,000 pairs for validation  
   - 10,000 pairs for testing  

This prepared dataset is ready for fine-tuning multilingual pretrained models for Nepali paraphrasing.

---

## Summary

- Started with English paraphrase datasets  
- Created ~200K Nepali pairs by direct English-to-Nepali translation  
- Created ~200K Nepali pairs via back-translation for diversity  
- Combined and shuffled data for a balanced dataset  
- Split data for training and evaluation  

This approach leverages existing English data and translation tools to build quality resources for Nepali NLP tasks.

---

Feel free to explore and use this data for Nepali paraphrase model training!
