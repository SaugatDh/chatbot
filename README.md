# Chatbot Project

This repository contains the files for a simple chatbot project.

## Files:
- `chatbot_model.h5`: The trained model for the chatbot.
- `Chatbot.ipynb`: Jupyter Notebook for training and building the chatbot.
- `chatbott.ipynb`: Another Jupyter Notebook, possibly for testing or an alternative approach.
- `classes.pkl`: Pickled file containing the classes/categories of the chatbot.
- `intents.json`: JSON file defining the intents and responses of the chatbot.
- `word.pkl`: Pickled file containing the vocabulary/words used by the chatbot.

## Installation:

To set up this project, you will need to have Python installed. You can then install the necessary libraries using pip:

```bash
pip install tensorflow numpy nltk
```

## Usage:

To use the chatbot, you typically load the model and other necessary files, then implement a function to predict responses based on user input. Refer to the Jupyter notebooks for detailed usage examples.

```python
# Example (conceptual) of how to load and use the chatbot
import numpy as np
import nltk
from tensorflow.keras.models import load_model
import pickle
import json

# Load the trained model
model = load_model('chatbot_model.h5')

# Load intents, words, and classes
intents = json.loads(open('intents.json').read())
words = pickle.load(open('word.pkl', 'rb'))
classes = pickle.load(open('classes.pkl', 'rb'))

# Further code for prediction and interaction...
```
