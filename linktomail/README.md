# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Mailto QR Code Generator

### Required Structure 
user Inputs: You need to gather input from the user, such as:
>Sender's Email (from field)
>CC Email IDs (optional, can be multiple)
>Body Content (email message)


## Overview
The Mailto QR Code Generator is a tool that allows users to generate a mailto link with pre-filled details such as the recipient's email, CC email, subject, and body. This link is converted into a QR code that can be scanned and shared with others. When scanned, the QR code opens the user's default email client with the prefilled details, making it easier for a group of people to send the same email to a specific organization or person.

Features:
User inputs: Sender email, CC email, subject, and body of the email.
Generates a mailto link with prefilled details.
Displays a QR code of the generated mailto link, which can be scanned or clicked to open the email client.
Tech Stack
Vite - Frontend tooling for fast development and optimized builds.
React.js - JavaScript library for building the user interface.
QRCode.react - React component for generating QR codes.
Tailwind CSS - Utility-first CSS framework for styling.


### Project Structure


```php 
.
├── public
│   └── index.html           # Entry point for the app
├── src
│   ├── components
│   │   ├── EmailForm.jsx     # Form to collect user email, CC, subject, and body
│   │   ├── GeneratedLink.jsx # Displays the generated mailto link
│   │   └── QRCodeGenerator.jsx # Displays the QR code
│   ├── utils
│   │   └── mailtoUtils.js    # Function to generate the mailto link
│   ├── App.jsx               # Main application logic
│   └── index.css             # Global styling (Tailwind CSS)
│   └── main.jsx              # Entry point for React
├── package.json              # Project dependencies and scripts
└── README.md                 # Project documentation

```


#### How It Works
Input: Users enter their email address, CC email, the subject of the email, and the email body.
Generate: Upon submitting the form, the app generates a mailto link using these details.
Display: The generated mailto link is displayed on the page, along with a QR code representation of the link.
Action: When a user scans the QR code, the default mail app opens with the email pre-filled with the provided details.



Contributions
Feel free to open issues or submit pull requests if you would like to contribute to the project.