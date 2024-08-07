
# Chatbot Deployment with Flask and JavaScript

This project offers two deployment options for the chatbot:

1. **Deploy within a Flask app using Jinja2 templates**
2. **Serve only the Flask prediction API**
   - The HTML and JavaScript files can be integrated into any frontend application, running independently from the Flask app with minimal modifications.

## Initial Setup

Follow these steps to set up the project:

1. **Clone the repository and create a virtual environment:**
   ```bash
   $ git clone https://github.com/deepz2609/chatbot-deployment.git
   $ cd chatbot-deployment
   $ python3 -m venv venv
   $ . venv/bin/activate
   ```

2. **Install the necessary dependencies:**
   ```bash
   $ (venv) pip install Flask torch torchvision nltk
   ```

3. **Download the NLTK package:**
   ```bash
   $ (venv) python
   >>> import nltk
   >>> nltk.download('punkt')
   ```

4. **Modify `intents.json` to define your chatbot's intents and responses.**

5. **Train the chatbot:**
   ```bash
   $ (venv) python train.py
   ```
   This command will generate the `data.pth` file.

6. **Test the chatbot in the console:**
   ```bash
   $ (venv) python chat.py
   ```

## Implementation

For a visual guide on implementing the chatbot, check out the video below:

[![Chatbot Deployment Video](https://img.youtube.com/vi/OimrifZTsxY/hqdefault.jpg)](https://www.youtube.com/embed/OimrifZTsxY)

## Repository

Explore the complete code and additional resources in the [chatbot-deployment repository](https://github.com/deepz2609/chatbot-deployment).

