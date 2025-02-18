# **Voice Deepfake Detection System**

## **Overview**
This project is a **Voice Deepfake Detection System** that classifies audio as **real or fake** using **MFCC feature extraction** and a **CNN-based deep learning model**. It is designed to help detect synthetic or manipulated voices.

---

## **Features**
✅ Extracts **MFCC features** from audio files  
✅ Supports dataset loading with **real** and **fake** voice samples  
✅ Uses a **Convolutional Neural Network (CNN)** for classification  
✅ Trained with **binary cross-entropy loss** and the **Adam optimizer**  
✅ Can be fine-tuned for different datasets  

---

## **Installation**
Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
```

Alternatively, manually install required packages:  
```bash
pip install librosa numpy scikit-learn tensorflow
```

---

## **Dataset Structure**
Organize your dataset as follows:

```
dataset/
├── real/  (Contains real voice audio files)
├── fake/  (Contains deepfake or synthetic voice files)
```

---

## **Usage**  

### **1. Extract Features from Audio Files**  
```python
from feature_extraction import extract_features
mfccs = extract_features("path/to/audio.wav")
```

### **2. Train the Model**  
Run the training script in the Jupyter Notebook or:
```python
python train_model.py
```

### **3. Test the Model on a New Audio File**  
```python
from predict import classify_audio
result = classify_audio("path/to/new_audio.wav")
print(f"Prediction: {result}")
```

---

## **Model Architecture**  
- **Conv2D Layer**: Extracts spatial features from MFCCs  
- **MaxPooling2D**: Reduces dimensionality  
- **Flatten & Dense Layers**: Classifies as **real (0) or fake (1)**  

---

## **Potential Applications**  
✅ Deepfake voice detection  
✅ Audio authentication for security  
✅ Fraud prevention in voice-based transactions  

---

## **Contributing**  
Feel free to open an issue or submit a pull request if you'd like to contribute!  

---

## **License**  
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## **Flowchart

