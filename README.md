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
```python
python train.py
```

This script will load the data from data.json, preprocess it, and train a neural network using PyTorch. The trained model will be saved as chatbot_model.pth.

## Chat with the bot

Once the model is trained, you can start a conversation with the chatbot using the chat.py script.

## Customization

### Modifying the Dataset
To customize the chatbot's behavior, you can edit the data.json file. Add new intents, patterns, and responses as needed. For example, to add a new intent for weather queries and retrain the model:

```json
{
    "tag": "weather",
    "patterns": ["What's the weather like?", "Tell me the weather", "Weather forecast"],
    "responses": ["It's sunny!", "Expect rain today.", "It's quite chilly."]
}
```
