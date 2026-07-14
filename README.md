# Phishing Awareness Analyzer

## Description
The Phishing Awareness Analyzer is a Python-based cybersecurity project that helps users identify potential phishing emails and messages. It analyzes the content using rule-based detection techniques and checks for common phishing indicators such as suspicious keywords, malicious links, urgency, password or OTP requests, banking information requests, and untrusted domains. Based on the analysis, it classifies the message as **Likely Safe**, **Suspicious**, or **Phishing** and provides detailed reasons for the decision.

## Features
- Analyzes text entered by the user or loaded from a file
- Detects common phishing keywords
- Identifies suspicious URLs
- Detects untrusted domains (e.g., `.xyz`, `.ru`)
- Detects personal email addresses used in suspicious messages
- Identifies excessive urgency in messages
- Detects requests for passwords, OTPs, and banking information
- Assigns a phishing risk score
- Classifies messages as:
  - Likely Safe
  - Suspicious
  - Phishing
- Displays detected red flags and explains the security risks

## Requirements
- Python 3.x
- Python `re` (Regular Expressions) module *(built into Python)*

## How to Run

1. Save the program as `phishing_analyzer.py`.
2. Open a terminal or command prompt.
3. Navigate to the project folder.
4. Run the following command:

```bash
python phishing_analyzer.py
```

5. Choose one of the following options:
   - **1** – Type or paste a message directly.
   - **2** – Read a message from a text file.

6. The program will analyze the message and display:
   - Verdict
   - Risk Level
   - Detected Red Flags
   - Explanation of the security risk

## Example

**Input**
```
Dear Customer,

Your bank account has been suspended.
Click here immediately to verify your account:
http://secure-bank.xyz

Please confirm your password and OTP to restore access.
```

**Output**
```
Verdict : PHISHING
Risk Level : HIGH

Red Flags Found:
1. Suspicious keyword detected: bank
2. Suspicious keyword detected: verify
3. Suspicious keyword detected: password
4. Suspicious link detected
5. Untrusted domain detected
6. Requests password
7. Requests OTP
8. Requests banking information
```

## Project Structure
```
project_folder/
│── phishing_analyzer.py
│── sample_messages.txt
└── README.md
```

## Technologies Used
- Python 3
- Regular Expressions (`re` module)

## Author
Fabiha Tariq