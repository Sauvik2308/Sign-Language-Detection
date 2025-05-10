
# Sign Language Detection

This project implements a basic Sign Language Detection system using a webcam. It collects image data for signs, creates a dataset, trains a classifier, and performs real-time inference.

## 📁 Project Structure

```
├── data/                 # Contains folders (0,1,2,3...) with webcam images for training
├── collect_imgs.py       # Script to collect images using a webcam
├── create_dataset.py     # Processes collected images into a usable dataset
├── train_classifier.py   # Trains a classifier model
├── inference_classifier.py # Performs real-time inference using the trained model
├── model.p               # Trained model file
├── data.pickle           # Serialized dataset
├── requirements.txt      # List of Python dependencies
├── README.md             # Project documentation
├── License               # Licensing information
```

## ⚙️ Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sign-language-detection.git
   cd sign-language-detection
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   pip install -r requirements.txt
   ```

## 📸 Data Collection

Use `collect_imgs.py` to capture images using your webcam:
```bash
python collect_imgs.py
```

Images will be stored in `data/` in folders like `0`, `1`, etc., each representing a different sign/class.

## 🛠️ Training

Generate a dataset and train the model:
```bash
python create_dataset.py
python train_classifier.py
```

## 🎯 Inference

Run the live prediction:
```bash
python inference_classifier.py
```

## 📄 License

This project is licensed under the MIT License. See the `License` file for more details.
