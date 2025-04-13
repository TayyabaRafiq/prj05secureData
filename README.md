# prj05secureData
This is a Streamlit-based application for securely storing and retrieving encrypted data using a user-defined passkey. It includes features like user authentication and protection against brute-force login attempts.
# Secure Data Encryption System (Streamlit App)

This is a Streamlit-based application for securely storing and retrieving encrypted data using a user-defined passkey. It includes features like user authentication and protection against brute-force login attempts.

---

## Features

- User Registration and Login System  
- Passkey-based Encryption and Decryption  
- Lockout after multiple failed login attempts  
- Encrypted data stored in a local JSON file  
- User-friendly Streamlit Interface  

---

## Technologies Used

- Python 3.x  
- Streamlit  
- cryptography (Fernet)  
- hashlib  
- JSON  

---

## How It Works

### Registration  
Users register with a username and password. The password is hashed and saved securely.

### Login  
Users log in with valid credentials. After 3 failed attempts, login is locked for 60 seconds.

### Store Encrypted Data  
Logged-in users can enter text and encrypt it using a passkey. The encrypted data is stored in a local JSON file.

### Retrieve Encrypted Data  
Users can view their encrypted entries and decrypt them using the correct passkey.

---

## File Structure

- `datasecure.py` - Main application file  
- `secure_data.json` - Stores encrypted user data  
- `README.md` - Project documentation  

---

## How to Run

1. Clone the repository  
2. Install required packages using pip  
3. Run the app with Streamlit  

```bash
pip install streamlit cryptography
streamlit run datasecure.py
