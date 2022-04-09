# Psychiatrist ChatBot
## COSC 310 Software Engineering Individual Project
### Pavni Agarwal

------

### Local Environment Setup

### New Dependencies to install

`pip install googletrans`

`pip install wikipediaapi`

#### Install Dependencies

`pip install nltk`

`pip install numpy`

`pip install keras`

`pip install tensorflow`

`pip install spacy`

`python -m spacy download en_core_web_sm`

When first running the program, it may ask you to download certain NTLK packages. The only way I found I could download them was by running the code below:

```python
import nltk
import ssl

try:
    _create_unverified_https_context = ssl._create_unverified_context
except AttributeError:
    pass
else:
    ssl._create_default_https_context = _create_unverified_https_context

nltk.download()
```

Link to source can be found here: https://stackoverflow.com/questions/38916452/nltk-download-ssl-certificate-verify-failed


#### Train ChatBot

To train the chatbot you can run the file `app/chatbot/train.py`

#### Use ChatBot

To use the chatbot you can run the file `app/chatbot/chatbot_app.py`

------

### API Added (Individual Project)

## Google Translate API
The Google Translate API is used to translate any language typed by the user into English so the chatbot can understand the message

## Wikipedia API
The Wikipedia API is utilized such that when the user wants to know something, like depression, the chatbot will return the summary retrieved from the Wikipedia’s page on depression.
