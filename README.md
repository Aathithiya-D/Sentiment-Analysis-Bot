Here's a sample README file for your GitHub repository:

---

# Sentiment Analysis Chatbot

This repository contains a simple sentiment analysis chatbot that uses both an NLP-based approach (VADER) and a machine learning model (SVM) to determine the sentiment of user inputs. 

## Features

- **NLP Sentiment Analysis**: Uses VADER from the NLTK library to analyze sentiment.
- **Machine Learning Sentiment Analysis**: Uses a Support Vector Machine (SVM) classifier trained on a small dataset of sentiment-labeled words.
- **Interactive Chat**: The chatbot interacts with the user and provides responses based on the detected sentiment.

## Requirements

- Python 3.x
- NLTK
- Scikit-learn

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/Aathithiya-D/sentiment-analysis-chatbot.git
    cd sentiment-analysis-chatbot
    ```

2. Install the required Python packages:
    ```sh
    pip install nltk scikit-learn
    ```

3. Download the VADER lexicon:
    ```python
    import nltk
    nltk.download('vader_lexicon')
    ```

## Usage

Run the chatbot:
```sh
python chatbot.py
```

The chatbot will start and greet you. You can interact with it by typing messages. To exit the chat, type `exit`.

## Code Overview

### Main Functions

- **analyze_sentiment_nlp(user_input)**: Analyzes sentiment using the VADER sentiment analyzer.
- **analyze_sentiment_ml(user_input)**: Analyzes sentiment using the trained SVM model.
- **main()**: Main function that runs the chatbot.

### Training Data

The training data for the SVM classifier is a small set of manually labeled words. For better results, a larger and more comprehensive dataset should be used.

### Sample Training Data
```python
documents = ["Love", "Hate", "Joy", "Sad", "Excitement", "Fear", "Hope", "Anger", "Peace", "Grief", "Smile", "Tears", "Success", "Failure", "Friendship", "Loneliness", "Gratitude", "Disappointment", "Adventure", "Pain", "Died", "cool", "regret", "good", "bad", "normal", "okay"]
labels = ["pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "pos", "neg", "neg", "pos", "neg", "pos", "neg", "neu", "pos"]
```

## Future Improvements

- Use a larger and more diverse dataset for training the machine learning model.
- Implement more advanced NLP techniques for better sentiment analysis.
- Add more interactive features to the chatbot.

## License

This project is licensed under the MIT License.

## Acknowledgements

- [NLTK](https://www.nltk.org/)
- [Scikit-learn](https://scikit-learn.org/)

---

Feel free to customize this README file further according to your project's specifics and preferences.
