# Posture Assistant App

This is a full-stack version of the Posture Assistant application.

## Structure
- **public/**: Contains the frontend code (HTML, JS, CSS).
  - `index.html`: The main entry point.
  - `js/`: Application logic (`app.js`, `detector.js`, `ui.js`).
  - `lib/`: Third-party libraries (FaceMesh, Lucide, etc.).
  - `css/`: Styles.
- **server/**: Contains the backend code.
  - `server.js`: The Express server that serves the app and handles logging.
  - `logs.json`: Stores posture event logs.

## Prerequisites
To run this application, you need **Node.js** installed on your computer.
1. Download Node.js from [nodejs.org](https://nodejs.org/).
2. Install it.

## How to Run
1. Open a terminal (Command Prompt or PowerShell) in this folder.
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   npm start
   ```
4. Open your browser and go to:
   [http://localhost:3000](http://localhost:3000)

## Features
- **Real-time Posture Detection**: Uses camera to detect slouching or head tilt.
- **Backend Logging**: "Bad Posture" events are logged to `server/logs.json`.
- **Privacy**: Processing happens locally in the browser. Only log events are sent to the backend.
