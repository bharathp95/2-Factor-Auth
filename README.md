# OTP Authentication Script Using Twilio

This Python script is a simple command-line authentication system that first validates a static password and then uses Twilio to send a one-time password (OTP) via SMS for a second layer of verification.

## 🚀 Features

- Password-based authentication
- OTP generation (6-digit)
- OTP delivery via SMS using [Twilio](https://www.twilio.com/)
- Retry mechanism for incorrect password attempts
- Basic error handling

## 🔧 Requirements

- Python 3.x
- Twilio Account (for SMS functionality)
- Active internet connection

## 🧰 Dependencies

Install the required dependency using pip:
- pip install twilio
  
## 🧪 How It Works

1. The user is prompted to enter a password.
2. The script allows up to **5 password attempts**.
3. Upon correct password entry:
   - A **6-digit OTP** is generated.
   - The OTP is sent to the specified phone number using **Twilio**.
   - The user is prompted to enter the received OTP.
4. If the OTP is correct, the user is **authenticated**.
