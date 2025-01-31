# AuthEase - OTP Verification System

## Overview

**AuthEase** is an OTP (One-Time Password) verification system that allows users to authenticate themselves through email by sending an OTP. The system is simple, secure, and designed with a sleek user interface using HTML, CSS, and JavaScript. It's powered by a Flask backend to handle OTP generation and verification.

This project aims to demonstrate the implementation of OTP-based email authentication in a web application.

## Features

- **OTP Generation**: Users provide their email, and an OTP is sent to their email for verification.
- **OTP Verification**: Users enter the received OTP, which is verified by the backend.
- **Resend OTP**: If the OTP expires or is not received, users can request to resend the OTP.
- **Aesthetic UI**: Modern and user-friendly design with gradient backgrounds, styled buttons, and a responsive layout.

## Technologies Used

- **Frontend**:
  - HTML
  - CSS (with gradient effects, responsive design)
  - JavaScript (for handling form submissions and OTP generation/verification)
  
- **Backend**:
  - Python (Flask framework)
  - SMTP (for email handling)
  
- **Dependencies**:
  - Flask: Web framework for handling requests and routing.
  - SMTP: To send OTPs to user emails.

## Installation

To set up and run this project locally, follow these steps:

### 1. Clone the repository

```bash
git clone https://github.com/your-username/AuthEase.git
cd AuthEase
```

###2. Set up a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

###3. Install dependencies
```bash
pip install -r requirements.txt
```

###4. Set up your email configuration

Before running the app, make sure to set up your SMTP email credentials in the config.py file.

###Example:

```python
MAIL_USERNAME = 'your_email@gmail.com'
MAIL_PASSWORD = 'your_email_password'
MAIL_SERVER = 'smtp.gmail.com'
MAIL_PORT = 465
```

###5. Run the Flask app
```bash
python app.py
```

## Usage

The application should now be running on [http://127.0.0.1:5000/](http://127.0.0.1:5000/).

### Steps to Use:
1. Visit the home page where you can enter your name and email to receive the OTP.
2. Enter the OTP received in your email to verify your identity.
3. If needed, click the **Resend OTP** button to request a new OTP.

## Screenshots

1. **Landing Page**
   ![Landing Page](path-to-your-landing-page-screenshot.png)

2. **OTP Verification**
   ![OTP Verification](path-to-your-otp-verification-screenshot.png)

## Contributing

We welcome contributions to this project! 

###**License**

This project is licensed under the MIT License.
