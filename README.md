
# SignBridge

**SignBridge** is an interactive, educational game that helps users—especially children and beginners—learn American Sign Language (ASL) through real-time sign detection and engaging levels. By combining computer vision, machine learning, and a gamified frontend, SignBridge bridges the communication gap and promotes inclusivity in a fun and intuitive way.

## 🌟 Features

- ✋ **Real-Time ASL Detection** using MediaPipe and TensorFlow.
- 🧠 **LSTM Model** for accurate gesture recognition.
- 🎮 **Multi-Level Learning Game**: Learn alphabets, words, and basic sentences step-by-step.
- 🌐 **MERN Stack Frontend** for a seamless and interactive UI.
- 🔁 **Feedback Loop**: Real-time visual feedback to guide learning.
- 📚 **Educational Tool**: Ideal for schools, inclusive learning environments, and ASL enthusiasts.

---

## 📂 Project Structure

```
SignBridge/
│
├── backend/             # Flask server for ML model inference
│   ├── model/           # Trained LSTM model and preprocessing logic
│   └── app.py           # Flask routes for prediction API
│
├── frontend/            # React.js game interface
│   ├── src/
│   └── public/
│
├── training/            # ASL training pipeline (MediaPipe + LSTM)
│   └── train_model.ipynb
│
├── utils/               # Helper scripts (e.g., data preprocessing)
│
├── requirements.txt     # Backend Python dependencies
├── package.json         # Frontend dependencies
└── README.md            # You're here!

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Node.js & npm
- pip / virtualenv

### 1. Clone the Repository

```bash
git clone https://github.com/Medhamishraa/signbridge.git
cd signbridge
```

### 2. Setup Backend

```bash
cd backend
pip install -r requirements.txt
python app.py
```

The Flask server will start on `http://localhost:5000`

### 3. Setup Frontend

```bash
cd ../frontend
npm install
npm start
```

Frontend will start on `http://localhost:3000`

---

## 🧠 Model Architecture

- **Feature Extraction**: MediaPipe Hands extracts 21 key landmarks.
- **Model**: A Long Short-Term Memory (LSTM) model classifies sequences of landmarks.
- **Trained on**: Custom ASL dataset (A-Z and select words).
- **Accuracy**: ~XX% (Update with actual performance)

---

## 🎯 Use Cases

- ASL learning in schools
- Inclusive communication games
- Early language development tools
- Assistive education tech for hearing-impaired users

---

## 🛠 Tech Stack

- **Frontend**: React.js, Tailwind CSS
- **Backend**: Flask, TensorFlow, OpenCV, MediaPipe
- **Model**: LSTM-based gesture recognition
- **Others**: Socket.io (if real-time), Google Colab (training), JSON, REST API

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Create issues for bugs or suggestions
- Submit pull requests
- Star ⭐ the repo if you like it!

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).

---

## 👩‍💻 Author

**Medha Mishra**  
📫 [medhamishra1708@gmail.com](mailto:medhamishra1708@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/medha-mishra-b17166250/) | [GitHub](https://github.com/Medhamishraa)

---

## 🙌 Acknowledgements

- TensorFlow & MediaPipe
- OpenCV Community
- ASL Alphabet Dataset Contributors
