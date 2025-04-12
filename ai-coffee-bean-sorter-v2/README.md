# ☕ AI-Powered Coffee Bean Sorting System

This project automates the classification and sorting of coffee beans using a Raspberry Pi and a CNN model (MobileNetV2). It identifies Arabica, Robusta, Liberica, and Excelsa beans based on size, shape, and texture, then uses servo motors to physically sort them.

## 🔧 Components

- Raspberry Pi 3B+
- Smartphone camera (IP Webcam)
- SG90 Servo Motors
- DC motor + L298N driver
- 5V relay
- Conveyor Belt (A3 leather)
- Logic Level Shifter

## 🧠 Deep Learning Model

- Model: MobileNetV2 (fine-tuned)
- Framework: PyTorch
- Dataset: 1600 high-res images (400/class)
- Accuracy: 96.93% train, 82.24% test

## 📁 Repository Structure

- `training/`: Contains training and testing code (`train.py`, `test.py`)
- `model/`: Saved PyTorch model
- `raspberry-pi/`: Script for real-time classification and servo control
- `images/`: Hardware diagrams and result graphs
- `data/`: (Optional) Dataset structure
- `docs/`: Full report PDF

## 🚀 Getting Started

### Requirements
```bash
pip install -r requirements.txt
```

### Training the Model
```bash
cd training
python train.py
```

### Testing
```bash
python test.py
```

### Running on Raspberry Pi
```bash
cd raspberry-pi
python classifier.py
```

## 📈 Results

- Training Accuracy: 96.93%
- Test Accuracy: 82.24%
- Confusion Matrix included in `images/`

## 📄 License

MIT License
