<div align="center">

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:667eea,100:764ba2&height=180&section=header&text=Codo%20File&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=Speak%20It.%20Snap%20It.%20Ship%20It.&descAlignY=58&descSize=20&animation=fadeIn" alt="Codo File Banner"/>

### 🎙️ Voice-driven Coding &nbsp;|&nbsp; 📷 OCR Image-to-Code &nbsp;|&nbsp; 🧪 Multi-Language Playground

<p>
<img src="https://img.shields.io/badge/Frontend-React%2018-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
<img src="https://img.shields.io/badge/Backend-Express-000000?style=for-the-badge&logo=express&logoColor=white" />
<img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" />
<img src="https://img.shields.io/badge/Auth-JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" />
<img src="https://img.shields.io/badge/License-ISC-blue?style=for-the-badge" />
</p>

<p>
<img src="https://img.shields.io/badge/Node.js-v16+-339933?style=flat-square&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Python-3.x-3776AB?style=flat-square&logo=python&logoColor=white" />
<img src="https://img.shields.io/badge/Dart-SDK-0175C2?style=flat-square&logo=dart&logoColor=white" />
<img src="https://img.shields.io/badge/OCR-Tesseract.js-FF6F00?style=flat-square" />
<img src="https://img.shields.io/badge/PRs-Welcome-brightgreen?style=flat-square" />
</p>

**⭐ Star this repo if you like it — it keeps the coffee flowing ☕**

[🚀 Features](#-key-features) • [🛠️ Tech Stack](#️-tech-stack--key-libraries) • [📂 Structure](#-project-structure) • [⚡ Quick Start](#-quick-setup--run-instructions) • [🤝 Contribute](#-contributing)

</div>

<br/>

<div align="center">
<img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="600">
</div>

<br/>

## ✨ Overview

> **Codo File** reimagines the modern coding workspace. Talk to your editor, snap a photo of handwritten code, and compile across languages — all inside one sleek browser tab. Built for developers who want speed, accessibility, and a little bit of magic. ✨

<br/>

## 🚀 Key Features

<table width="100%">
<tr>
<td width="50%" valign="top">
<h3>🎙️ Voice-to-Code Converter</h3>
<p>Write code <b>hands-free</b>. Powered by the Web Speech API, Codo File listens and intelligently converts vocalized English instructions and punctuation into valid, ready-to-run code.</p>
</td>
<td width="50%" valign="top">
<h3>📷 Image-to-Code (OCR)</h3>
<p>Snap or upload a photo of handwritten/printed code. <code>tesseract.js</code> scans it client-side and hands you a clean, copyable, executable script in seconds.</p>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<h3>🧪 Multi-Language Playgrounds</h3>
<p>Live <b>HTML/CSS/JS</b> sandbox, an instant <b>JavaScript console</b>, a backend-powered <b>Python compiler</b>, and secure <b>Dart</b> execution via child processes.</p>
</td>
<td width="50%" valign="top">
<h3>🔒 Auth & Dashboard</h3>
<p>Full registration/login/logout flow. Passwords hashed with <code>bcryptjs</code>, sessions secured with signed <code>JWT</code> tokens.</p>
</td>
</tr>
</table>

<details>
<summary><b>🎙️ Click to expand the full Voice Command Cheat-Sheet</b></summary>
<br/>

| 🗣️ Say This | ➜ | Symbol | 🗣️ Say This | ➜ | Symbol |
| :--- | :---: | :---: | :--- | :---: | :---: |
| `"semicolon"` | ➜ | `;` | `"comma"` | ➜ | `,` |
| `"colon"` | ➜ | `:` | `"dot"` | ➜ | `.` |
| `"open parentheses"` | ➜ | `(` | `"close parentheses"` | ➜ | `)` |
| `"open curly bracket"` | ➜ | `{` | `"close curly bracket"` | ➜ | `}` |
| `"open square bracket"` | ➜ | `[` | `"close square bracket"` | ➜ | `]` |
| `"open double quotes"` | ➜ | `"` | `"close double quotes"` | ➜ | `"` |
| `"open single quotes"` | ➜ | `'` | `"close single quotes"` | ➜ | `'` |

</details>

<br/>

## 🛠️ Tech Stack & Key Libraries

<table width="100%">
<tr>
<td valign="top" width="50%">

### 🎨 Client (Frontend)

| Library | Purpose |
| :--- | :--- |
| **React** `v18.2.0` | Hooks & context state |
| **React Router DOM** | Client-side routing |
| **React Speech Recognition** | Web Speech API wrapper |
| **Tesseract.js** | Pure JS OCR engine |
| **React CodeMirror** | Syntax-highlighted IDE editor |
| **React Use Clipboard** | One-click copy |
| **React Hot Toast** | Notification banners |

</td>
<td valign="top" width="50%">

### ⚙️ Server (Backend)

| Library | Purpose |
| :--- | :--- |
| **Express.js** | REST APIs & execution routes |
| **MongoDB Atlas + Mongoose** | Accounts & sessions |
| **Bcrypt.js** | Secure password hashing |
| **JSON Web Tokens** | Session authentication |
| **Child Process** | Sandboxed script execution |

</td>
</tr>
</table>

<br/>

## 📂 Project Structure

```text
Codo-File-main/
├── package.json                 # Parent workspace configurations
├── package-lock.json
│
├── backend/                     # Server-Side Source
│   ├── app.js                   # Application gateway & Express configuration
│   ├── config.env               # Port details, database keys & JWT secret key
│   ├── db/
│   │   └── conn.js              # Mongoose MongoDB connection client
│   ├── model/
│   │   └── userSchema.js        # User mongoose schema with token generation methods
│   ├── python_runner/           # Workspace for compiling temporary .py scripts
│   ├── dart_runner/             # Workspace for compiling temporary .dart scripts
│   └── router/
│       ├── auth.js              # Combined auth & compile API routers
│       ├── executepy.js         # Launches python command processes
│       ├── generatePy.js        # Writes temporary python scripts to disk
│       ├── executeDart.js       # Launches dart execution processes
│       └── generateDart.js      # Writes temporary dart scripts to disk
│
└── frontend/                    # Client-Side Source
    ├── package.json             # Frontend dependencies
    ├── public/                  # Core static files
    └── src/
        ├── index.js             # Initial bootstrap entrypoint
        ├── index.css            # Stylesheet overrides
        ├── assets/              # Global icons & static graphics
        ├── reducer/
        │   └── UseReducer.js    # Auth states reducer
        └── Components/
            ├── App.jsx          # Setup routes and context hooks
            ├── Header.jsx       # Standard navigation header
            ├── Screens/         # Authentication and general screens
            └── Editor/          # Code editors (Python, JS, HTML/CSS, Dart, OCR, Voice)
```

<br/>

## ⚡ Quick Setup & Run Instructions

### ✅ Prerequisites

| Requirement | Notes |
| :---: | :--- |
| 🟢 **Node.js** | v16+ installed |
| 🐍 **Python 3** | Installed and added to system `PATH` |
| 🎯 **Dart SDK** | Required to compile Dart engine commands |
| 🍃 **MongoDB** | Local instance or MongoDB Atlas connection string |

<br/>

### 📥 Step 1 — Clone the Repository

```bash
git clone https://github.com/your-username/codo-file.git
cd codo-file/Codo-File-main
```

### 📦 Step 2 — Install Dependencies

```bash
# Root folder
npm install

# Frontend
cd frontend && npm install && cd ..

# Backend
cd backend && npm install && cd ..
```

### 🔧 Step 3 — Configure Environment Variables

Create a `config.env` file inside `backend/`:

```env
PORT=5000
DB=your_mongodb_atlas_connection_string
SECRET_KEY=your_secure_custom_jwt_secret_key
```

### ▶️ Step 4 — Launch 🚀

```bash
npm run both
```

<div align="center">

| 🎨 Frontend | ⚙️ Backend |
| :---: | :---: |
| [`http://localhost:3000`](http://localhost:3000) | [`http://localhost:5000`](http://localhost:5000) |

</div>

<br/>

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
Feel free to check the [issues page](../../issues) or open a pull request. ⭐ Don't forget to star the repo if you found it useful!

<br/>

<div align="center">
<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=0:764ba2,100:667eea&height=100&section=footer" alt="footer"/>

**Made with ❤️ for developers who'd rather talk than type.**

</div>
