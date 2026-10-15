# BERT IMDB Sentiment Analysis

## Project Overview
This project uses a fine-tuned BERT model to classify IMDB movie reviews as positive or negative.

## Technologies Used
- Python
- Hugging Face Transformers
- PyTorch
- Scikit-learn
- Google Colab

## Model
I fine-tuned the pretrained `bert-base-uncased` model for binary sentiment classification using the IMDB dataset.

**Fine-tuned Model on Hugging Face:**

[View My BERT Sentiment Analysis Model]([https://huggingface.co/krupaj/my-bert-imdb2](https://huggingface.co/krupaj/my-bert-imdb2/blob/main/README.md))

## Results
- Validation Accuracy: 88%
- Validation F1 Score: 0.868

## How to Use
```python
from transformers import pipeline

classifier = pipeline(
    "text-classification",
    model="krupaj/my-bert-imdb2"
)

result = classifier("This movie was amazing!")
print(result)
```

## Project Description
This project demonstrates how a pretrained BERT model can be fine-tuned using Hugging Face Transformers to perform sentiment analysis on movie reviews.
