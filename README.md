# FetalAI-Using-Machine-Learning


🏥 Fetal Health Prediction System

Flask | Machine Learning | scikit-learn | REST API

A professional web-based application that leverages a Machine Learning model to predict fetal health conditions using Cardiotocogram (CTG) data. Built using Flask and a Random Forest model, this system provides real-time predictions with high accuracy.

🌟 Key Features
🖥️ Web Application
🏠 Modern Home Page with feature overview
🔍 Prediction Interface with 21 CTG inputs
📞 Contact Page with user interaction
🤖 Machine Learning Capabilities
Real-time prediction using trained model
Accuracy: ~95% (Random Forest Classifier)
Confidence score with probability distribution
Input validation & error handling
⚙️ Advanced Features
REST API for external integration
Fully responsive (mobile + desktop)
Clean UI with animations and gradients
Lightweight (~2MB trained model)
📁 Project Structure
fetal-health-prediction/
│
├── app.py                          # Flask backend
├── requirements.txt                # Dependencies
├── README.md                       # Documentation
├── model_training.ipynb            # ML training notebook
├── dataset/
│   └── fetal_health.csv            # Dataset (2126 rows)
│
├── templates/
│   ├── home.html
│   ├── predict.html
│   ├── result.html
│   ├── contact.html
│   └── model_info.html
│
└── model.pkl                       # Trained ML model
🚀 Getting Started
🔧 Prerequisites
Python 3.7+
pip
Git
📥 Installation

# Navigate into folder
cd fetal-health-prediction

# Create virtual environment
python -m venv venv


# Activate environment
# Windows:
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
▶️ Run the Application
python app.py

Open in browser:

http://127.0.0.1:5000
🧠 Model Details
Algorithm: Random Forest Classifier
Dataset Size: 2126 samples
Features: 21 CTG parameters
Classes:
✅ Normal
⚠️ Suspect
❌ Pathological
🔍 How It Works
User inputs CTG values
Data is preprocessed
Model predicts fetal condition
Output includes:
Predicted class
Confidence score
Probability distribution
🔌 API Usage
📌 POST /api/predict
curl -X POST http://127.0.0.1:5000/api/predict \
-H "Content-Type: application/json" \
-d '{ "baseline value": 120, "accelerations": 0, ... }'
📌 Response
{
  "success": true,
  "prediction": "Normal",
  "confidence": 94.2
}
⚠️ Disclaimer
This project is for educational purposes only
Not intended for real clinical use
Always consult medical professionals
🐛 Troubleshooting
Issue: Flask not found
pip install Flask
Issue: Model missing
Run Jupyter notebook and train model
Issue: Port already in use
app.run(port=5001)
📈 Future Improvements
📱 Mobile App
🔐 User Authentication
☁️ Cloud Deployment (AWS/Render)
📊 Analytics Dashboard
🔄 Model Versioning
🤝 Contributing
git checkout -b feature/your-feature
git commit -m "Added feature"
git push origin feature/your-feature

Then open a Pull Request.

📞 Contact
👨‍💻 Developer: Anuj Kadam
📧 Email: anujkadam3554@gmail.com
🔗 GitHub:https://github.com/Anujkadam1881
⭐ Support

If you like this project:

⭐ Star the repo
🍴 Fork it
📢 Share it
