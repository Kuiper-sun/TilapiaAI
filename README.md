# 🐟 Tilapia Freshness Detection Tool (Gills Only)

A desktop application that analyzes the **gills only** of a Tilapia fish image to determine freshness using a trained deep learning model.

## 💡 Features

- Upload an image of a Tilapia fish
- Real-time freshness detection based exclusively on **gill appearance**
- Outputs one of three labels: `Fresh`, `Not Fresh`, or `Old`
- Color-coded result display for clarity
- Clean and intuitive Tkinter GUI with image preview

## 🧠 Model Approach: Gill-Focused RT-DETRv2

- Utilizes **RT‑DETRv2** (a real-time Detection Transformer model) customized to detect and evaluate fish gills.
- Focuses solely on the gill region for freshness prediction, ignoring other features like eyes.
- Trained on a curated dataset where gill visuals are categorized by freshness level.

## 🛠️ Technologies Used

- Python
- Tkinter for GUI
- Pillow (PIL) for image handling
- PyTorch (or ONNX) for running the RT‑DETRv2 model
- Custom dataset with labeled Tilapia gill images

## 🚀 Setup & Usage

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/tilapia-gill-detector.git
   cd tilapia-gill-detector

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt


3. **Download model weights:**

- Place gill_model.pth (or equivalent) in the project root.
- Ensure load_model() in model.py points to this file.

4. **Run the application:**

   ```bash
   python app.py

## Collaborators
- Gabriel R. Abesamis
- Abdurasheed A. David
- Pamela T. Solosinda
- Kieferson Carl G. Supnet

## Licenses
MIT License

Copyright (c) 2025 Abesamis, David, Golosinda, Supnet

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
