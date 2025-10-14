#Hinglish to English

This project fine-tunes a **pretrained neural machine translation (NMT)** model to translate **Hinglish (Hindi–English code-mixed text)** into fluent **English**.  
It uses Hugging Face Transformers library for efficient model loading, tokenization, and fine-tuning.

---

#Overview

Code-mixed languages like **Hinglish** (Hindi and English) are commonly used in social media and texts, but most translation models handle only monolingual input.  
This project adapts an existing multilingual model to better understand Hinglish syntax, romanized Hindi, and informal expressions.

---

##Features

- Loads and fine tunel pretrained model
- Handles **Hinglish text preprocessing and cleaning**
- Supports **batch evaluation** of translation quality (BLEU, ROUGE, etc.)
- Outputs translated sentences and performance metrics
- Easily extendable to other code-mixed language pairs


