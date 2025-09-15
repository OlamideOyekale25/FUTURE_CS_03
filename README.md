# 🛡️ File Encryption Web App

A simple Flask web application that lets you upload files and automatically encrypts them using AES-256 encryption.

## 🎯 What it does

- Upload any file through a web interface
- Files get encrypted automatically when uploaded
- Download either the encrypted version or get the original file back (decrypted)
- Clean, simple web interface

## 🚀 How to run it

1. **Clone this repo**
   ```bash
   git clone https://github.com/OlamideOyekale25/FUTURE_CS_03.git
   cd FUTURE_CS_03
   ```

2. **Set up virtual environment (Not compulsory but Recommended)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install requirements**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**
   ```bash
   python app.py
   ```

5. **Open your browser** and go to `http://localhost:5000`

## 📁 Files in this project

- `app.py` - Main Flask application with routes
- `encryption.py` - Handles AES encryption and decryption
- `templates/index.html` - Web page interface
- `requirements.txt` - Python packages needed
- `uploads/` - Where encrypted files are stored

## How the encryption works

- Uses AES-256 encryption in CBC mode
- Each file gets a random IV (initialization vector)
- Only encrypted files are saved to disk
- When you download the "decrypted" version, it decrypts the file in memory and sends it to you

## ⚠️ Academic Purpose & Disclaimer

This project was developed as an educational exercise to demonstrate:
- Practical application of cryptographic algorithms
- Secure web application development principles
- Integration of encryption libraries in Python

**Important Note**: This implementation is designed for learning purposes. Production deployments would require additional security measures including proper key management systems, user authentication, HTTPS implementation, and comprehensive access controls.

