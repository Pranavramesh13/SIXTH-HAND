# ✋ SIXTH HAND: Sign Language to Speech & Text

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" alt="TensorFlow">
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white" alt="OpenCV">
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask">
</p>

<p align="center">
  <b>Empowering communication: Convert sign language gestures to text and speech using computer vision and deep learning.</b><br>
  <i>Bridging the gap for the hearing and speech impaired with real-time sign recognition and text-to-speech.</i>
</p>

---

## 📚 Project Overview

SIXTH HAND is a Python-based application that leverages deep learning and computer vision to recognize hand signs (ASL) from a webcam, converting them into text and optionally speech. The project aims to assist individuals with hearing or speech impairments by providing a seamless way to communicate using sign language, with outputs in both text and audio formats.

---

## 🗂️ Folder Structure

```
SIXTH-HAND-main/
│
├── app.py                        # Main Flask application
├── index.html                    # Landing page
├── signin.html                   # Sign-in page
├── service-details.html          # Service details page
├── assets/                       # Static assets (CSS, JS, images)
│   ├── css/
│   ├── js/
│   ├── img/
│   └── scss/
├── forms/                        # Contact form (PHP)
├── sign/                         # Sign language recognition
│   ├── camerahand.py             # Webcam sign capture and prediction
│   ├── model.py                  # Model loading and prediction logic
│   ├── predicted_text.txt        # Stores last predicted text
│   └── sign_mnist_test.csv       # Test data for sign language
├── smnist.h5                     # Trained Keras model (ASL recognition)
├── Text-To-Speech-main/          # Text-to-speech module
│   └── TTS.py                    # Text-to-speech script
├── test.mp3                      # Example audio output
├── Sixth_Hand.pptx               # Project presentation
└── README.md                     # Project documentation
```

---

## ✨ Features

- **Real-time Sign Language Recognition:**
  - Uses a webcam to capture hand gestures and recognizes them using a trained deep learning model.
- **Text Output:**
  - Converts recognized signs into readable text.
- **Text-to-Speech:**
  - Converts recognized text into speech using a TTS engine.
- **Web Interface:**
  - User-friendly web interface built with Flask and HTML/CSS.
- **Contact Form:**
  - Simple PHP-based contact form for user feedback.

---

## 🚀 Getting Started

### 1. Prerequisites
- Python 3.7 or higher
- `pip` package manager

### 2. Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/bchaitanya92/SIXTH-HAND.git
    cd SIXTH-HAND-main
    ```

2. **(Recommended) Create and activate a virtual environment:**
    ```sh
    # Windows
    python -m venv venv
    .\venv\Scripts\activate

    # macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3. **Install required libraries:**
    ```sh
    pip install -r requirements.txt
    ```
    *(If requirements.txt is missing, install: flask, tensorflow, opencv-python, numpy, pillow, pyttsx3, etc.)*

---

## 💡 Usage

1. **Start the Flask app:**
    ```sh
    python app.py
    ```
2. **Access the web interface:**
    - Open your browser and go to `http://localhost:5000`
3. **Sign Language Recognition:**
    - Use the interface to start the webcam and perform sign gestures.
    - The recognized sign will be displayed as text and can be converted to speech.

---

## 🧩 Key Components

| **File/Folder**         | **Description**                                              |
|------------------------|--------------------------------------------------------------|
| `app.py`               | Main Flask backend serving the web app                       |
| `sign/camerahand.py`   | Captures webcam input and predicts sign language             |
| `sign/model.py`        | Loads and runs the trained sign recognition model            |
| `sign/predicted_text.txt` | Stores the latest recognized text                        |
| `smnist.h5`            | Pre-trained Keras model for ASL recognition                  |
| `Text-To-Speech-main/TTS.py` | Converts text to speech using TTS engine              |
| `assets/`              | Static files: CSS, JS, images                                |
| `forms/contact.php`    | Contact form handler                                         |

---

## 👨‍💻 Author & Credits

Developed by:

- **PRANAV RAMESH**

- GitHub: [Pranavramesh13](https://github.com/Pranavramesh13)
- LinkedIn: [Pranav Ramesh](https://www.linkedin.com/in/Pranavramesh13)

*Feel free to explore, modify, and experiment with the code for your learning and projects. Contributions and feedback are always welcome!*
