# Registration-and-Login-System using python along with File handling



This project is a simple registration and login system implemented in Python, using file handling.

## Features
- User registration: The system validates the email/username and password input, and stores the user's credentials in a file.
- User login: The system checks the user's input against the data stored in the file, and allows access if the credentials match.
- Forgotten password retrieval: The system allows the user to retrieve their password by providing their username.







## Requirements
- Python-3

## Usage
1. Run the script with `python main.py`
2. Choose the option to register or login.
3. Follow the prompts to enter your email/username and password.
4. If you choose to register, the system will validate your input and store your credentials in a file.
5. If you choose to login, the system will check your input against the data stored in the file.
6. If your credentials match, you will be granted access. If not, you will be prompted to register or retrieve your password.

## Note
- This project is for demonstration purposes only and should not be used in a production environment.

# Workflow

## Stage 1: Registration

When the user chooses to register, the following validation is applied to their email/username and password:

- Email/username:
    - Must contain "@" followed by a "."
        - Example: kishor@gmail.com, nothing@yahoo.in
    - Should not contain "." immediately after "@"
        - Example: my@.in
    - Should not start with special characters or numbers
        - Example: 123#@gmail.com
- Password:
    - Must be between 5 and 16 characters in length
    - Must contain at least one special character, one digit, one uppercase, and one lowercase character

## Stage 2: Data Storage

Once the username and password are validated, the data is stored in a file.

## Stage 3: Login

When the user chooses to login, the following process is followed:

- Check whether the inputted username and password exist in the file
- If the credentials do not exist:
    - Ask the user to go for registration
- If the user has chosen "forgot password":
    - Retrieve the original password based on the provided username (if it exists in the file)
    - Allow the user to provide a new password (if their username matches with the data in the file)
- If nothing matches in the file:
    - Ask the user to go for registration (since they do not have an account)
