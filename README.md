# SpamDetector – AI-Powered Email Threat Detection System

An AI-powered email spam detection application built using Python, Flask, Scikit-learn, React, and Vite.

The application analyzes email content and predicts whether an email is **Spam** or **Ham (Legitimate)** using Machine Learning.

## 1. Project Features

- AI-based email spam classification.
- TF-IDF text feature extraction.
- Multinomial Naive Bayes classification.
- Prediction confidence score.
- Flask REST API backend.
- React and Vite frontend.
- Interactive user interface.
- Machine Learning model training.

## 2. Technologies Used

| Component | Technology |
|---|---|
| Programming Language | Python |
| Backend | Flask |
| Frontend | React.js |
| Frontend Build Tool | Vite |
| Machine Learning | Scikit-learn |
| Feature Extraction | TF-IDF |
| Classification | Multinomial Naive Bayes |
| Data Processing | Pandas |

## 3. Project Structure

```text
spam-email-detector/
│
├── backend/
│   ├── app.py
│   ├── requirements.txt
│   └── ...
│
├── frontend/
│   ├── src/
│   ├── index.html
│   ├── script.js
│   ├── style.css
│   ├── package.json
│   └── ...
│
├── .vscode/
│   └── launch.json
│
└── README.md
```

## 4. Prerequisites

Install the following before running the project:

- Python 3.10 or later
- Node.js and npm
- Git
- VS Code (optional)

Verify installation:

```bash
python3 --version
node --version
npm --version
```

## 5. Backend Setup (Flask)

Open your terminal in the project root directory.

### Step 1: Navigate to backend

```bash
cd backend
```

### Step 2: Create a virtual environment

```bash
python3 -m venv venv
```

### Step 3: Activate the virtual environment

For Linux / Kali Linux:

```bash
source venv/bin/activate
```

### Step 4: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 5: Start the Flask backend

```bash
python app.py
```

The backend should start at:

```text
http://127.0.0.1:5000
```

Keep this terminal running.

## 6. Frontend Setup (React + Vite)

Open a second terminal.

### Step 1: Navigate to frontend

```bash
cd frontend
```

### Step 2: Install dependencies

```bash
npm install
```

### Step 3: Start the development server

```bash
npm run dev
```

The frontend should be available at:

```text
http://localhost:5173
```

Open the URL in your browser.

## 7. Running the Complete Application

You need two terminal sessions.

**Terminal 1 – Backend**

```bash
cd backend
source venv/bin/activate
python app.py
```

**Terminal 2 – Frontend**

```bash
cd frontend
npm run dev
```

Access the application:

http://localhost:5173

## 8. How the Application Works

1. User enters an email message.
2. Frontend sends the email content to the Flask API.
3. Backend preprocesses the email.
4. TF-IDF converts the text into numerical features.
5. The trained Naive Bayes model classifies the email.
6. The application returns the prediction and confidence score.
7. Frontend displays the result.

## 9. Troubleshooting

**Problem: Python module not found**

```bash
pip install -r requirements.txt
```

**Problem: npm dependencies missing**

```bash
cd frontend
npm install
```
```bash
cd frontend
xdg-open index.html
```

**Problem: Port 5000 already in use**

Check the process:

```bash
sudo lsof -i :5000
```

**Problem: Port 5173 already in use**

```bash
sudo lsof -i :5173
```

**Problem: Virtual environment not activated**

```bash
source backend/venv/bin/activate
```

Run this command from the project root.

## 10. Future Improvements

- Advanced spam detection algorithms.
- Phishing URL detection.
- Email attachment security analysis.
- Explainable AI predictions.
- Model performance monitoring.
- Authentication and secure API access.
- Deployment with HTTPS.

## 11. Security Notice

This project is intended for educational and research purposes.

The development server is intended for local testing. Production deployment should include authentication, HTTPS, input validation, API security, and appropriate logging.

## 12. Author

**Project:** SpamDetector –  Email Threat Detection System

**Category:**  Machine Learning | Cybersecurity

