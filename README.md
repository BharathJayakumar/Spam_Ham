# Spam_Ham
Spam_Ham Email classification

This project contains a script to connect to a Gmail IMAP server, fetch emails, classify them using a pre-trained model, and move them based on the classification. The script uses IMAP to interact with Gmail, and joblib to load the pre-trained machine learning model and vectorizer.

## Prerequisites

- Python 3.x
- Gmail account with app-specific password (if 2-Step Verification is enabled)
- Pre-trained model (`joblib_model.sav`) and vectorizer (`vectorizer.pkl`)

## Installation

1. **Clone the repository**:
   ```sh
   git clone https://github.com/BharathJayakumar/Spam_Ham.git
   cd email-spam-classifier

2. **Install the required packages**:   
    pip install -r requirements.txt


3. **Script Overview**:
    The script performs the following steps:

    1.Connect to the Gmail IMAP server.
    2.Log in using the provided email and app-specific password.
    3.Fetch all emails from the inbox.
    4.Extract the body of each email.
    5.Preprocess the email content using a pre-trained vectorizer.
    6.Classify the email using a pre-trained machine learning model.
    7.Move the email to the spam folder if classified as spam.

4. **Usage**:
    1.Ensure your Gmail account is set up:
        Generate an app-specific password if you have 2-Step Verification enabled.
    2.Place your pre-trained model and vectorizer:
        Ensure joblib_model.sav and vectorizer.pkl are in the project directory.


5. **Notes**:
Ensure you have appropriate permissions to access and move emails in your Gmail account.
The script processes all emails in the inbox, which may include a large number of emails depending on your account usage.
You may need to adjust the script to handle specific email formats or additional preprocessing steps based on your dataset and model requirements.


6. **Contributing**:
Feel free to submit issues or pull requests if you find any bugs or have suggestions for improvements.