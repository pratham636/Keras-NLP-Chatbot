## ⚙️ How it Works
1.  **Preprocessing:** The bot tokenizes user input and lemmatizes words to find the base meaning.
2.  **Bag of Words:** It converts the input into a numerical array (0s and 1s) representing the presence of known words.
3.  **Classification:** The neural network predicts the probability of each "intent" tag.
4.  **Response:** The bot randomly selects a response from the matched intent in `intents1.json`.

## 📝 Customization
You can add new capabilities to the bot by editing the `intents1.json` file. Simply add a new tag, patterns (what the user says), and responses (what the bot says). Remember to re-run `training.pyBelow is a clean, professional `README.md` for your GitHub repository based on the code and file structure you provided.

---

# Neural: AI Contextual Chatbot

Neural is a context-aware chatbot built using Python, TensorFlow, and Natural Language Processing (NLP). It uses a deep learning model to classify user intent and provide relevant responses based on a custom dataset.

## 🚀 Features
*   **Deep Learning Backend:** Built with Keras/TensorFlow.
*   **Natural Language Processing:** Uses NLTK for tokenization and lemmatization.
*   **JSON Configured:** Easily update responses and patterns without changing the core logic.
*   **Scalable:** Can be trained on any custom set of intents.

## 📂 Project Structure
*   `training.py`: The script used to preprocess data and train the neural network.
*   `chartbox.py`: The main execution script to interact with the chatbot in real-time.
*   `intents1.json`: The data file containing patterns, tags, and responses.
*   `chatbot_model.h5`: The trained model file (generated after training).
*   `words.pkl` & `classes.pkl`: Pickled data structures for vocabulary and intent labels.

## 🛠️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone (https://github.com/pratham636/Keras-NLP-Chatbot.git)
   ```
   ```
   cd your-repo-name
   ```
2. **Install Dependencies:**
Make sure you have Python installed. You will need the following libraries:

```Bash
pip install nltk tensorflow numpy
```
3. **Download NLTK Data:**
Run a Python shell and download the necessary resources:

```
Python
import nltk
nltk.download('punkt')
nltk.download('wordnet')
```
## 🎮 Usage
1. **Training the Model**
Before running the bot, you must train the model using your intents file:

```Bash
python training.py
```
This will generate chatbot_model.h5, words.pkl, and classes.pkl.

**2. Running the Chatbot**
Start the interaction by running:

```Bash
python chartbox.py
```
## ⚙️ How it Works
Preprocessing: The bot tokenizes user input and lemmatizes words to find the base meaning.

Bag of Words: It converts the input into a numerical array (0s and 1s) representing the presence of known words.

Classification: The neural network predicts the probability of each "intent" tag.

Response: The bot randomly selects a response from the matched intent in intents1.json.

## 📝 Customization
You can add new capabilities to the bot by editing the intents1.json file. Simply add a new tag, patterns (what the user says), and responses (what the bot says). Remember to re-run training.py after making changes!
