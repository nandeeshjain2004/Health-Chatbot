# Medical Chatbot

This is a web-based medical chatbot that answers questions based on the content of the "An Introduction to Infectious Diseases" PDF by Barry C. Fox.

## Setup

1.  **Install Dependencies:**
    *   You'll need to have Python and pip installed.
    *   Install the required Python packages using the `requirements.txt` file:
        ```bash
        pip install -r requirements.txt
        ```

2.  **Set Up Ollama:**
    *   This chatbot uses the Ollama library to run the LLaMA 3.1 language model locally.
    *   Follow the instructions on the [Ollama website](https://ollama.com/) to download and install it on your system.
    *   Once installed, run the following commands in your terminal to start the Ollama server and pull the LLaMA 3.1 model:
        ```bash
        ollama serve &
        ollama run llama3.1
        ```

## Running the Application

1.  **Start the Flask Server:**
    *   With the Ollama server running, start the Flask application by running:
        ```bash
        python app.py
        ```
    *   The application will be available at `http://127.0.0.1:5000`.

2.  **Access the Chatbot:**
    *   Open your web browser and navigate to `http://127.0.0.1:5000`.
    *   You can now start asking questions in the chat window.