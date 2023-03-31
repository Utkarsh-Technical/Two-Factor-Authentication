# Two-Factor Authentication

This is a simple application that demonstrates how to implement Two-Factor Authentication (2FA) using Node.js, Express.js, and MongoDB. 
The application uses the [Speakeasy](https://github.com/speakeasyjs/speakeasy) library to generate TOTP (Time-based One-Time Password) tokens and
[QRCode](https://github.com/soldair/node-qrcode) to generate QR codes.

## Prerequisites

Before you begin, you should have the following installed on your machine:

- Node.js (v14 or later)
- MongoDB

## Getting Started

1.  Clone this repository to your local machine:  

```bash
git clone https://github.com/Utkarsh-Technical/Authentication.git
```

2.  Install the project dependencies:

```bash
npm install
```

3.  Start the MongoDB server:
```bash
mongod
```

4.  Start the application:
```bash
npm start
```

5. Open your web browser and navigate to http://localhost:5000/


## UsageThe application has three routes:

 - "/" - This is the <strong>home page</strong>. You can click the "Generate Manual Code" button to generate a secret code that you can manually put with your 2FA app 
 (such as Google Authenticator or Microsoft Authenticator).
 - "/verify" - This is the <strong>verification page</strong>. After input the secret code with your 2FA app, enter the 6-digit token and click the "Verify" button.

## Tech Stack

- Node.js - an open-source, cross-platform JavaScript runtime environment
- Express.js - a fast, unopinionated, minimalist web framework for Node.js
- MongoDB - a document-oriented NoSQL database program
- Speakeasy - a library for generating Time-based One-Time Password (TOTP) tokens
