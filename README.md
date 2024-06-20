# Simple Chatbot with PyTorch

Welcome to the Simple Chatbot project! This repository contains the implementation of a basic chatbot using PyTorch. The chatbot uses a dataset in JSON format, which can be easily customized to alter the bot's behavior and responses.

## Features

- Simple and easy-to-understand implementation using PyTorch.
- Customizable dataset in JSON format.
- Basic NLP preprocessing and tokenization.
- Training and inference scripts.

## Installation

To get started with the project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/pratikamrit316/Simple-ChatBot-using-Pytorch.git
cd Simple-ChatBot-using-Pytorch
```

## Datasets
The dataset is stored in a JSON file (data.json). The JSON structure is straightforward, making it easy to add, remove, or modify the intents and responses. Here's an example structure of the JSON file:

```json
{
    "intents": [
        {
            "tag": "greeting",
            "patterns": ["Hi", "Hello", "How are you?", "Good morning"],
            "responses": ["Hello!", "Hi there!", "Greetings!", "Good to see you!"]
        },
        {
            "tag": "goodbye",
            "patterns": ["Bye", "See you later", "Goodbye"],
            "responses": ["Goodbye!", "See you later!", "Have a great day!"]
        }
        // Add more intents here
    ]
}
```

## Usage

Training the Model
To train the chatbot model, run the following command:
