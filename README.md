# End-to-end-Deep-Learning-Project-Using-Simple-RNN
1)# IMDB Movie Review Sentiment Analysis

This project is a simple web application for sentiment analysis of IMDB movie reviews. It uses a pre-trained Recurrent Neural Network (RNN) model with ReLU activation to classify user-provided movie reviews as either "Positive" or "Negative".

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)

## Installation

To run this project locally, follow these steps:

1. **Clone the repository:**

2. **Create a virtual environment (optional but recommended):**
    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required Python packages:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Download the pre-trained model:**
   - Place the `simple_rnn_imdb.h5` file in the project directory. If you don't have this model, you may need to train it first.

5. **Run the Streamlit app:**
    ```bash
    streamlit run app.py
    
    ```
## project structure
Model: The app uses a pre-trained RNN model that was trained on the IMDB dataset. The model is designed to classify the sentiment of movie reviews as either positive or negative.

User Input: Users can input a movie review into the text area provided in the web interface.

Preprocessing: The input text is tokenized and converted into a sequence of integers based on the IMDB word index. This sequence is then padded to a fixed length (500) to ensure compatibility with the model.

Prediction: The preprocessed input is fed into the model, which outputs a probability score. If the score is greater than 0.5, the review is classified as "Positive"; otherwise, it's classified as "Negative".

## Usage

1. Open your web browser and navigate to `http://localhost:8501`.
2. Enter a movie review in the provided text area.
3. Click the "Classify" button to see whether the review is classified as "Positive" or "Negative".
4. The app will also display the prediction score, indicating the confidence level of the classification.

## Project Structure

```plaintext
├── main.py                # Main application file containing the Streamlit code.
├── simple_rnn_imdb.h5    # Pre-trained TensorFlow model for sentiment analysis.
└── requirements.txt      # Python packages required to run the app.
