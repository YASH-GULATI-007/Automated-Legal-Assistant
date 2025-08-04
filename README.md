# Automated-Legal-Assistant

This project is a rule-based chatbot application that combines **Natural Language Processing (NLP)** with a simple **feedforward neural network** to classify user inputs and generate appropriate responses. It is implemented in **Python**, with the model built using **PyTorch** and the user interface created using **Tkinter**.

The chatbot is trained on a custom intent dataset defined in `intents.json`, which maps user input patterns to specific categories (tags) such as greetings, farewells, or questions. Each category contains a list of sample inputs and possible responses. The goal is to identify the intent behind a user's message and provide a suitable reply from the response list.

---

## 💡 Key Highlights

- **Custom Neural Network Classifier**  
  A multi-layer feedforward network is used to classify intents based on user input. It is trained from scratch using PyTorch.

- **Basic NLP Pipeline**  
  Text preprocessing includes tokenization, stemming, and bag-of-words vectorization using **NLTK**.

- **Custom Dataset**  
  `intents.json` serves as a lightweight dataset defining multiple user intents and response patterns.

- **Interactive Desktop GUI**  
  Built with **Tkinter**, the GUI enables real-time interaction between the user and the chatbot.

- **Threshold-Based Confidence**  
  The chatbot responds only when the model's prediction confidence exceeds a certain threshold; otherwise, it returns a fallback message like “I do not understand…”

- **Modular Codebase**  
  Clean separation between model definition, training logic, NLP utilities, and GUI logic.

---

## 🗂️ File Structure

├── app.py # Tkinter GUI application for chat interaction
├── chat.py # Loads the model and generates chatbot responses
├── train.py # Training script for the neural network model
├── model.py # PyTorch-based neural network architecture
├── nltk_utils.py # NLP functions: tokenization, stemming, bag-of-words
├── intents.json # JSON file containing intents, patterns, and responses
├── data.pth # Trained model saved as a binary PyTorch file
└── README.md # Project description and documentation

---

## 📘 Description

This chatbot was built as a learning project to understand how classic NLP techniques can be combined with simple machine learning models to create interactive systems. It demonstrates how even with basic tools like bag-of-words and feedforward networks, one can achieve reasonably effective intent classification and conversation handling.

It is ideal for beginners learning about:
- Text preprocessing
- Neural network design in PyTorch
- Intent classification
- GUI development in Python
- Applying ML to real-world conversational tasks
🗂️ File Structure## 🗂️ File Structure

