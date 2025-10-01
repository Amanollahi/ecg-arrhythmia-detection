# ecg-arrhythmia-detection
Medical-grade ECG arrhythmia detection with >95% sensitivity and >90% classification accuracy
markdown# ECG Arrhythmia Detection System

A medical-grade system for detecting and classifying cardiac arrhythmias from ECG signals.

![Dashboard](ECG_Project_Dashboard.png)

## 🎯 Performance

- **R-Peak Detection**: >95% sensitivity (clinical standard)
- **Classification**: >90% accuracy (3-class problem)
- **Validation**: MIT-BIH Arrhythmia Database

## 🔧 Technical Implementation

### Signal Processing
- Butterworth high-pass filter (baseline wander removal)
- Notch filter (60 Hz powerline interference)
- Band-pass filter (0.5-40 Hz)

### Detection Algorithm
- Pan-Tompkins algorithm (implemented from scratch)
- Adaptive thresholding
- Real-time capable (<10ms per beat)

### Machine Learning
- Random Forest classifier
- 9 clinically-relevant features
- SMOTE for class balancing

## 📊 Dataset

MIT-BIH Arrhythmia Database (PhysioNet)
- 10+ patient records
- 10,000+ annotated heartbeats
- 3 arrhythmia classes: Normal, PVC, Atrial

## 🛠️ Technologies

- Python 3.x
- SciPy (signal processing)
- scikit-learn (machine learning)
- Pandas, NumPy, Matplotlib

## 🚀 Installation
```bash
pip install -r requirements.txt
