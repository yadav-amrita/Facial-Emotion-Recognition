# 😊 Facial Emotion Recognition

A Machine Learning and Deep Learning based Facial Emotion Recognition system built with **Python**, **PyTorch**, **OpenCV**, and **Streamlit**.

This project detects human emotions from uploaded facial images using image feature extraction techniques such as **HOG (Histogram of Oriented Gradients)** and **LBP (Local Binary Patterns)** combined with a Deep Neural Network classifier.

---

## Features

* Upload face images through a simple Streamlit web interface
* Detect emotions instantly
* Displays confidence scores for all emotions
* Uses HOG + LBP feature extraction
* Deep Neural Network model built using PyTorch
* Face preprocessing with OpenCV

---

## Technologies Used

* Python
* PyTorch
* OpenCV
* Streamlit
* NumPy
* scikit-image
* Joblib

---

## Project Structure

```bash
Facial_Emotion_Recognition_HSW/
│
├── app.py                     # Main Streamlit application
├── emotion_model.pth          # Trained PyTorch model
├── scaler.pkl                 # Feature scaler
├── labels.pkl                 # Emotion labels
├── features.pkl               # Selected feature indices
├── Final_HSW_QIGA.ipynb       # Training/experimentation notebook
├── ck+.zip                    # Dataset archive
├── Images/                    # Sample images and assets
└── README.md
```

---

## Supported Emotions

The model can classify emotions such as:

* Happy
* Sad
* Anger
* Fear
* Surprise
* Disgust
* Contempt

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Facial_Emotion_Recognition_HSW.git
cd Facial_Emotion_Recognition_HSW
```

### 2. Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
```

Activate environment:

#### Windows

```bash
venv\Scripts\activate
```

#### Linux / Mac

```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

If you don't have a requirements.txt file, install manually:

```bash
pip install streamlit opencv-python numpy torch scikit-image joblib
```

---

## Run the Application

```bash
streamlit run app.py
```

Then open the local URL shown in the terminal.

---

## How It Works

1. User uploads a facial image.
2. Image is converted to grayscale and resized.
3. HOG and LBP features are extracted.
4. Features are scaled and selected.
5. PyTorch DNN model predicts the emotion.
6. Predicted emotion and confidence scores are displayed.

---

## Model Details

* Feature Extraction:

  * HOG (Histogram of Oriented Gradients)
    * HOG is used to capture the structural and edge information of facial expressions.
  * LBP (Local Binary Pattern)
    * LBP is used for extracting local texture information from facial images.

* Deep Learning Model:

  * Fully Connected Neural Network
  * Batch Normalization
  * Dropout Regularization
  * ReLU Activation

---

## Sample Interface

You can add screenshots from the `Images/` folder here.

Example:

```markdown
![App Screenshot](Images/img1.png)
```

---

## Future Improvements

* Real-time webcam emotion detection
* Support for multiple faces
* Improved CNN-based architecture
* Deployment on cloud platforms
* Better UI/UX

-----

## License

This project is for educational and learning purposes.

---

## Author

Developed by **Amrita**.
