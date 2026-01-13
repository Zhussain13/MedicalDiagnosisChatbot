# Symptom Checker Chatbot AI

A simple chatbot that helps users check their symptoms and provides relevant information. The chatbot uses natural language processing (NLP) techniques and a recurrent neural network (RNN) model to understand user queries and respond accordingly.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Training](#training)
- [Dependencies](#dependencies)


## Introduction

This project implements a symptom checker chatbot capable of engaging in conversations with users, gathering symptom information, and providing suggestions about potential conditions or nearby medical centers. It uses a pre-trained RNN model for natural language understanding.

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/Zhussain13/MedicalDiagnosisChatbot.git
````

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Ensure the following data files are available in the project directory:

   * `intents.json` – Predefined chatbot intents.
   * `data_rnn.pth` – Pre-trained RNN model.
   * `medical_centers.json` – Information about medical centers.

## Usage

Start the chatbot by running:

```bash
python app.py
```

This launches a Flask web application. Open `http://localhost:5000` in your browser to chat with the bot.

## Training

To retrain the RNN model or customize the chatbot:

1. Update intents and patterns in `intents.json`.

2. Retrain the model using:

   ```bash
   python train.py
   ```

3. Save the trained model and update the filename in `chat.py`.

## Dependencies

* Python 3.x
* PyTorch
* Flask
* NLTK
* geocoder

All dependencies can be installed via `requirements.txt`.

