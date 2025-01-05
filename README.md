# 📚 Comprehensive Math Tutor

**Your all-in-one solution for solving math problems with detailed explanations and visual aids!**  
This application uses **OCR (Optical Character Recognition)**, problem-type detection, and **LLM-based AI** to generate step-by-step solutions to math problems, tailored to various student grade levels. Whether it’s arithmetic, algebra, calculus, or geometry, this app is here to help!

---

## ✨ Features

- 📷 **Upload or Capture a Math Problem:** Analyze math problems directly from images.
- 🧠 **Dynamic Complexity Detection:** Automatically determines the complexity of the question.
- 🏫 **Grade-Level Adaptation:** Custom explanations tailored for different grades (Grade 1-12).
- 🖼️ **Visual Aids:** Generates geometric shapes, graphs, and diagrams to aid understanding.
- 🤖 **AI-Powered Explanations:** Uses cutting-edge LLM (WizardMath-7B) for detailed solutions.
- 🎨 **Custom Visualization Styles:** Adapts visuals based on grade-level preferences.

---

## 🛠️ Requirements

Before you begin, ensure you have the following installed:

- **Python 3.8 or later**
- **pip (Python Package Manager)**
- **Tesseract OCR**  
  [Download Tesseract OCR](https://github.com/tesseract-ocr/tesseract) and configure the path in the script:
  ```python
  pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
  ```
- **CUDA-Enabled GPU (Optional)** for faster model execution (if available).

---

## 📦 Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/comprehensive-math-tutor.git
   cd comprehensive-math-tutor
   ```

2. **Create and Activate a Virtual Environment** (Optional but recommended)
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Required Packages**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download the Model from Hugging Face**
   The script automatically downloads the required model based on your hardware setup (GPU or CPU).

---

## 🚀 How to Run

1. **Start the Application**
   ```bash
   python app.py
   ```
   This launches the Gradio web interface.

2. **Upload or Capture a Problem**
   - Provide an image containing a math problem.
   - Select the appropriate grade level.
   - Click on **Solve!**

3. **Explore Results**
   - Get a detailed explanation in Markdown format.
   - View a visual aid (if applicable).

---

## 📋 Example Workflow

1. Upload a problem image or take a snapshot.
2. Choose a grade level (e.g., **Grade 5-6**).
3. Receive:
   - A step-by-step explanation.
   - Visual aids (if the problem involves geometry or graphing).

---

## 📂 Directory Structure

```
📁 comprehensive-math-tutor
├── app.py                # Main application script
├── requirements.txt      # List of dependencies
├── README.md             # Project documentation
└── assets/               # Placeholder for future assets like demo images
```

---

## 🔧 Configuration

### Update Tesseract Path
Ensure the Tesseract OCR executable path matches your system:
```python
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"
```

### GPU/CPU Model Selection
The script detects available hardware and downloads the best model:
- **GPU Available:** Downloads `WizardMath-7B-V1.1-GGUF`.
- **CPU Only:** Downloads `WizardMath-7B-V1.0-GGML`.

---

## 🤝 Contribution Guidelines

We welcome contributions to enhance the project!  
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature description"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 🎉 Acknowledgments

- **Gradio:** For the seamless web interface.
- **Hugging Face:** For providing robust LLM models.
- **Tesseract OCR:** For enabling text recognition.
- **Matplotlib:** For creating stunning visual aids.

---

## 🖼️ Demo

![App Screenshot](assets/demo-screenshot.png)

---
