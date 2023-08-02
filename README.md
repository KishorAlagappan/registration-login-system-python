# Registration-and-Login-System using Python with File Handling

## Overview
This project presents a secure and user-friendly Registration-and-Login-System implemented in Python, incorporating file handling techniques. Designed for educational purposes, the system offers user registration, login verification, and password retrieval functionalities, ensuring a seamless user experience.

## Table of Contents
- [Features](#features)
- [Requirements](#requirements)
- [Usage](#usage)
- [Workflow](#workflow)
   - [Stage 1: Registration](#stage-1-registration)
   - [Stage 2: Data Storage](#stage-2-data-storage)
   - [Stage 3: Login](#stage-3-login)
- [Tools & Skills](#tools--skills)
- [Contribution](#contribution)

## Features
- **User Registration**: The system validates email/username and password inputs, storing user credentials securely in a file.
- **User Login**: User credentials are verified against stored data, granting access upon successful validation.
- **Forgotten Password Retrieval**: Users can retrieve passwords by providing their username.

## Requirements
- Python 3

## Usage
1. Run the ipynb file: `Registration_&_Login_System.ipynb`
2. Choose between registration or login.
3. Enter your email/username and password as prompted.
   - For registration, valid inputs are stored securely after validation.
   - For login, credentials are cross-checked against stored data.

## Workflow
**Stage 1: Registration**
- Validate email/username:
   - Must contain "@" followed by a "."
   - Cannot have "." immediately after "@"
   - Should not start with special characters or numbers
- Validate password:
   - Must be between 5 and 16 characters
   - Requires at least one special character, digit, uppercase, and lowercase character

**Stage 2: Data Storage**
- Validated username and password securely stored in a file.

**Stage 3: Login**
- Validate user-provided username and password against stored data.
   - If credentials do not exist, prompt the user to register.
   - If "forgot password" is chosen, retrieve the original password based on username (if in file) and allow the user to set a new password.
   - If no match is found, guide the user to register.

## Tools & Skills
- **Python Programming**: Developed the entire system using Python.
- **File Handling**: Implemented secure data storage and retrieval using file handling techniques.
- **Data Validation**: Ensured user inputs met specific criteria for registration and login.
- **User Authentication**: Created a reliable authentication system to verify user identities.
- **Command-Line Interface**: Utilized a command-line interface for user interaction.

## Contribution
Contributions and suggestions are welcome! Please open an issue or pull request if you have any feedback.
