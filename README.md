# 🤟 Sign Language to Text & Speech

A real-time computer vision application that recognizes American Sign Language (ASL) hand gestures through a webcam and converts the recognized gestures into text and speech.

The application uses hand landmark detection and a CNN-based classification pipeline to recognize fingerspelling gestures and combine recognized characters into words and sentences.

---

## ✨ Features

- 🎥 Real-time webcam-based sign recognition
- ✋ Hand detection and landmark tracking
- 🧠 CNN-based gesture classification
- 🔤 American Sign Language alphabet recognition
- 📝 Character-to-sentence conversion
- 🔊 Text-to-speech output
- 🖥️ Desktop graphical interface
- ⚡ Real-time prediction

---

## 🛠️ Tech Stack

- **Python**
- **TensorFlow**
- **Keras**
- **OpenCV**
- **MediaPipe**
- **CVZone**
- **NumPy**
- **pyttsx3**
- **Tkinter**

---

## 🔄 How It Works

```text
                    Webcam
                       │
                       ▼
              Hand Detection
                       │
                       ▼
            MediaPipe Landmarks
                       │
                       ▼
             Landmark Processing
                       │
                       ▼
              Image Preprocessing
                       │
                       ▼
                 CNN Model
                       │
                       ▼
              Sign Prediction
                       │
                       ▼
                  Character
                       │
                       ▼
                 Sentence
                       │
                       ▼
              Text-to-Speech
````

---

## 🧠 Sign Language Recognition

The application captures frames from the webcam and detects the user's hand using MediaPipe.

The detected hand landmarks are extracted and processed into a simplified representation. This representation is then passed through a CNN-based classification pipeline to predict the corresponding sign.

The recognition approach groups visually similar alphabet gestures before performing further classification to identify the individual character.

---

## 🔤 Supported Signs

The system is designed for American Sign Language fingerspelling and alphabet recognition.

Recognized characters can be combined sequentially to form words and sentences.

---

## 💻 Requirements

### Hardware

* Windows PC/Laptop
* Working webcam
* Speaker or headphones for speech output

### Software

* Python
* Webcam drivers
* Required Python packages

---

## 🚀 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/mehuldangda/Sign-Language-To-Text-and-Speech-Conversion.git
cd Sign-Language-To-Text-and-Speech-Conversion
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
```

### 3. Activate the Virtual Environment

#### Windows PowerShell

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks script execution, use Command Prompt:

```cmd
venv\Scripts\activate.bat
```

### 4. Install Dependencies

```bash
pip install -r requirements-working.txt
```

### 5. Run the Application

```bash
python -u final_pred.py
```

Make sure your webcam is connected and camera permissions are enabled.

---

## 🖥️ Application Workflow

Once the application starts:

1. The webcam captures the video stream.
2. MediaPipe detects the hand.
3. Hand landmarks are extracted.
4. The landmarks are processed for classification.
5. The CNN model predicts the corresponding gesture.
6. The predicted character is displayed on the interface.
7. Characters are combined to form a sentence.
8. The recognized text can be converted into speech.

---

## 🔊 Text-to-Speech

The application uses `pyttsx3` for text-to-speech conversion.

The recognized text can be converted into audible speech, providing a communication bridge between people who use sign language and people who may not understand sign language.

---

## 📁 Project Structure

```text
Sign-Language-To-Text-and-Speech-Conversion/
│
├── final_pred.py
├── prediction_wo_gui.py
├── data_collection_final.py
├── data_collection_binary.py
│
├── cnn8grps_rad1_model.h5
├── white.jpg
│
├── requirements-working.txt
├── README.md
└── .gitignore
```

### Important Files

**`final_pred.py`**

Main application that starts the webcam-based sign recognition interface.

**`prediction_wo_gui.py`**

Contains prediction-related functionality used by the recognition pipeline.

**`data_collection_final.py`**

Used for collecting sign-language image data.

**`data_collection_binary.py`**

Used for binary/group-based data collection.

**`cnn8grps_rad1_model.h5`**

Pre-trained CNN model used for gesture classification.

**`white.jpg`**

Image asset used during the landmark-based preprocessing pipeline.

---

## 🧩 Recognition Pipeline

```text
Camera Frame
     │
     ▼
Hand Detection
     │
     ▼
Hand Landmarks
     │
     ▼
Landmark Visualization
     │
     ▼
Preprocessing
     │
     ▼
CNN Classification
     │
     ▼
Gesture Group
     │
     ▼
Individual Character
     │
     ▼
Sentence
     │
     ▼
Speech
```

This approach reduces dependency on the original camera background by using hand landmark information during the recognition process.

---

## 🎯 Objective

The objective of this project is to develop a computer-based system capable of recognizing American Sign Language hand gestures and converting them into text and speech in real time.

The system aims to make communication easier between sign-language users and people who do not understand sign language.

---

## 🔮 Future Improvements

* 🎨 Modern and responsive user interface
* 📊 Prediction confidence scores
* 📝 Improved sentence formation
* 🎤 Better speech controls
* 📷 Camera selection support
* 🌙 Dark/light themes
* 🚀 Improved model architecture
* 🤖 Support for additional gestures
* 🌐 Cross-platform support
* 📦 Standalone executable application
* ⚡ Faster inference
* 🧹 Modular project architecture

---

## 📌 Project Status

**Current Status: Working Prototype**

The current version successfully performs real-time webcam-based hand detection, gesture prediction, character generation, and text-to-speech conversion.

Future versions will focus on improving the interface, code architecture, portability, and overall user experience.

---

## 🙌 Credits

This project is based on and inspired by an existing open-source sign-language recognition implementation.

**Original Project:**
[https://github.com/Devansh-47/Sign-Language-To-Text-and-Speech-Conversion](https://github.com/Devansh-47/Sign-Language-To-Text-and-Speech-Conversion)

This repository is intended as a modified and extended version of the original implementation.

Planned improvements include UI redesign, project restructuring, dependency modernization, improved usability, and additional functionality.

Please retain the applicable attribution and license requirements of the original project when redistributing derivative work.

---

## 📄 License

This project is based on an existing open-source implementation.

Please refer to the original repository and its license for applicable licensing and attribution requirements:

[https://github.com/Devansh-47/Sign-Language-To-Text-and-Speech-Conversion](https://github.com/Devansh-47/Sign-Language-To-Text-and-Speech-Conversion)

---

## ⭐ Acknowledgements

Thanks to the open-source computer vision and deep learning ecosystem, particularly:

* TensorFlow
* Keras
* OpenCV
* MediaPipe
* CVZone
* NumPy
* pyttsx3

for providing the technologies used in this project.

