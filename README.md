# Emotion Detection Application

A web-based AI application that detects emotions from text statements using Watson NLP, developed with Python and Flask.

## Project Overview

This project is part of the **Developing AI Applications with Python and Flask** course by IBM on Coursera. The application analyzes user-provided text and classifies the emotions present into five categories:
- **Anger**
- **Disgust**
- **Fear**
- **Joy**
- **Sadness**

It also determines the **dominant emotion** from the input text and displays the results through an intuitive web interface.

---

## Features

- **Watson NLP Integration**: Connects to the Watson NLP Emotion Predict service to evaluate emotional tone and confidence scores.
- **Python Package Architecture**: Encapsulates core logic into a reusable `EmotionDetection` package.
- **Robust Error Handling**: Handles HTTP status code 400 and invalid/blank inputs gracefully by returning `"Invalid text! Please try again!"`.
- **Unit Testing**: Fully tested using Python's built-in `unittest` framework.
- **Flask Web Interface**: Provides a responsive web front-end for real-time user interaction.
- **Static Code Analysis**: 100% compliant with PEP 8 standards, scoring `10.00/10` with `pylint`.

---

## Project Structure

```text
.
├── EmotionDetection/
│   ├── __init__.py               # Package initialization
│   └── emotion_detection.py      # Core emotion detection logic with Watson NLP
├── static/
│   └── mywebscript.js            # Client-side JavaScript handling AJAX requests
├── templates/
│   └── index.html                # Web interface HTML template
├── test_emotion_detection.py     # Unit testing script
├── server.py                     # Flask web server
├── requirements.txt              # Project dependencies
└── README.md                     # Project documentation
```

---

## Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Unit Tests:**
   ```bash
   python test_emotion_detection.py
   ```

4. **Run the Flask Web Application:**
   ```bash
   python server.py
   ```
   Access the web application at: `http://localhost:5000/`

5. **Run Static Code Analysis:**
   ```bash
   pylint server.py
   ```

---

## Author
Developed by Ganesh

