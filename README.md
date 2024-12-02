# ChatPal

## **Overview**

This is a basic ChatBot designed to provide a simple conversational interface. It uses natural language processing (NLP) to understand and respond to user input. This is designed for the backend specialisation portfolio project.

## **Features**

- Basic conversation flow
- Support for simple queries and statements
- Ability to understand and respond to user input

## **Requirements**

- Python 3.x
- `nltk` library for NLP tasks

## **Installation**

1. Clone the repository: `git clone <https://github.com/beautyscribbles/chat_pal.git`>
2. Install required libraries: `pip install nltk`
3. Download the NLTK data: `python -m nltk.downloader punkt`

## **Usage**

1. Run the ChatBot: `python chat_pal.py`
2. Interact with the ChatBot by typing your input

## **Code**

```python
import nltk
from nltk.tokenize import word_tokenize

# Initialize the ChatBot
def chatbot():
    while True:
        user_input = input("User: ")
        # Tokenize the user input
        tokens = word_tokenize(user_input)
        # Process the user input
        response = process_input(tokens)
        print("ChatBot:", response)

# Process the user input
def process_input(tokens):
    # Simple logic to respond to user input
    if "hello" in tokens:
        return "Hello! How are you?"
    elif "goodbye" in tokens:
        return "Goodbye! See you later."
    else:
        return "I didn't understand that."

# Run the ChatBot
chatbot()

```

## **Note**

This is a basic implementation and can be improved by adding more features, such as:

- Support for more complex queries and statements
- Integration with external APIs or services
- Improved NLP capabilities

You can modify and extend this code to create a more advanced ChatBot.
