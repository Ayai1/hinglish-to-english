# Hinglish-to-English Translation (Neural Machine Translation)

This project fine-tunes a pretrained model to translate **Hinglish (Hindi–English code-mixed text)** into fluent English.  
It uses the **Hugging Face Transformers** library for efficient model loading, tokenization, training, and evaluation.

---

##Overview

Code-mixed languages like **Hinglish** (Hindi words written in English script) are widely used on social media, chats, and everyday text.  
Most translation models fail on Hinglish because they are trained on **pure Hindi** or **pure English**, not mixed input.

This project fine-tunes a multilingual transformer model to better understand:

- Romanized Hindi  
- Hinglish grammar  
- Informal sentence structure  
- Social-media-style text  

The trained model outputs fluent English translations with improved accuracy.

---

##Features

- Loads and fine-tunes a **pretrained NMT transformer model**
- Handles **Hinglish text preprocessing, cleaning, and normalization**
- Supports **BLEU / ROUGE evaluation**
- Generates translated sentences with improved fluency
- Easily extendable to other code-mixed language pairs
- Works on Jupyter/Colab with GPU acceleration

---

## Example Translations

| Hinglish Input | Model Output (English) |
|----------------|------------------------|
| "Kal main market gaya tha aur bahut rush tha" | "I went to the market yesterday and it was very crowded." |
| "Tum kahan ho? main aa raha hu" | "Where are you? I am coming." |
| "Yeh movie bohot mast thi" | "This movie was really great." |
| "Mujhe samajh nahi aa raha ye kyun ho raha hai" | "I don't understand why this is happening." |

---

## Model Details

The project fine-tunes a pretrained multilingual translation model from Hugging Face: Facebook/nllb-200-distilled-600M

Pipeline:

- Text cleaning + normalization  
- Tokenization  
- Hinglish → English mapping  
- Mini-batch training with AdamW  
- BLEU/ROUGE evaluation
  
Results:

<img width="1000" height="359" alt="image" src="https://github.com/user-attachments/assets/e73f221c-2d32-4ae0-92dd-2c4a7e481bdd" />



<img width="226" height="52" alt="image" src="https://github.com/user-attachments/assets/e0753a0c-40f0-4b7b-bcdc-2efd6f505b95" />



```bash
# Clone the repository
git clone https://github.com/Ayai1/hinglish-to-english.git
cd hinglish-to-english

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook


Results:

<img width="1000" height="359" alt="image" src="https://github.com/user-attachments/assets/e73f221c-2d32-4ae0-92dd-2c4a7e481bdd" />

Evaluation Metrics:

<img width="226" height="52" alt="image" src="https://github.com/user-attachments/assets/e0753a0c-40f0-4b7b-bcdc-2efd6f505b95" />


