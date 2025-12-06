# Phishing Website Detection System

A machine learning-based web application that detects and classifies phishing websites in real-time.

![Phishing Detection](https://img.shields.io/badge/Phishing-Detection-red)
![Python](https://img.shields.io/badge/Python-3.7%2B-blue)
![Flask](https://img.shields.io/badge/Flask-2.0.1-green)
![scikit-learn](https://img.shields.io/badge/scikit--learn-0.24.2-orange)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Overview
This project implements a machine learning model to detect phishing websites based on URL analysis. The system classifies URLs as either legitimate (good) or phishing (bad) using a pre-trained model.

## Features
- Real-time URL classification
- Simple and intuitive web interface
- Fast prediction using pre-trained models
- Easy to deploy and use
- Supports both HTTP and HTTPS URLs

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/Phishing-Website-Detection-System.git
   cd Phishing-Website-Detection-System
   ```

2. **Create a virtual environment (recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Run the application**
   ```bash
   python app.py
   ```

2. **Access the web interface**
   Open your web browser and navigate to `http://127.0.0.1:5000/`

3. **Enter a URL**
   - Type or paste a URL in the input field
   - Click "Check URL" to get the prediction
   - The result will indicate if the website is legitimate or phishing

## How It Works

The system uses a machine learning model trained on a dataset of both legitimate and phishing URLs. The model analyzes various features of the URL to make its prediction:

1. **URL Preprocessing**: The input URL is cleaned and normalized
2. **Feature Extraction**: Relevant features are extracted from the URL
3. **Prediction**: The pre-trained model classifies the URL
4. **Result Display**: The classification result is shown to the user

## Dependencies

- Python 3.7+
- Flask 2.0.1
- scikit-learn 0.24.2
- pandas 1.3.0
- numpy 1.21.0
- requests 2.26.0
- tldextract 3.1.2
- whois 0.9.5
- python-whois 0.8.0

## Project Structure

```
Phishing-Website-Detection-System/
├── app.py                # Main Flask application
├── requirements.txt      # Project dependencies
├── phishing.pkl         # Pre-trained model
├── vectorizer.pkl       # Feature vectorizer
├── templates/           # HTML templates
│   └── index.html       # Main web interface
└── README.md            # This file
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Dataset used for training the model
- Flask for the web framework
- scikit-learn for machine learning capabilities
