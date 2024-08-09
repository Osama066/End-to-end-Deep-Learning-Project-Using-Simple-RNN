# End-to-end-Deep-Learning-Project-Using-Simple-RNN
1)# IMDB Movie Review Sentiment Analysis

This project is a simple web application for sentiment analysis of IMDB movie reviews. It uses a pre-trained Recurrent Neural Network (RNN) model with ReLU activation to classify user-provided movie reviews as either "Positive" or "Negative".

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Acknowledgements](#acknowledgements)

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
