Team Members: Name: USN: 1) A Manoj 
[KUB23CSE001] 2) Mahanthesh HS 
[KUB23CSE074]3)Anurag  [KUB23CSE011]

# AUTOMATIC GRADING SYSTEM

## Overview
This repository contains an **Automatic Grading System** web application with:
- A **Flask (Python) backend** to serve the web UI and provide API-like endpoints.
- A **static frontend** built using **HTML/CSS/JavaScript**.
- **PHP** scripts used by the frontend for operations such as uploads/clearing answers.
- An **Android project** (Gradle) included under `Android/`.
- Supporting **machine learning utilities** under `MachineLearning/`.

## Languages used
- **Python**
  - Backend server: `WebApp/flask_server.py`
  - ML utilities: `MachineLearning/` (e.g., `evaluation.py`)
- **HTML / CSS / JavaScript**
  - Frontend pages and assets under `WebApp/` (e.g., `index.html`, `css/`, `js/`, `images/`)
- **PHP**
  - Server-side scripts under `WebApp/*.php` (e.g., upload/clear handlers)
- **Gradle (Android/Java/Kotlin tooling)**
  - Mobile project under `Android/` and `Android/AEP/`

## Folder structure (key parts)
- `WebApp/`
  - `flask_server.py` - Flask app that serves the static site
  - `*.html` - UI pages
  - `css/`, `js/`, `images/`, `fonts/` - static assets
  - `*.php` - endpoints used by the UI
- `MachineLearning/`
  - Python scripts/notebooks for evaluation logic
- `Android/`
  - Android project files

## How to run the web app
1. Install required Python dependencies (if not already installed):
   - Flask
   - PyPDF2

2. Start the Flask server:
   - Run from the repo folder `automatic-grading-system-main/automatic-grading-system-main`:
     ```bash
     python -u WebApp/flask_server.py
     ```

3. Open the app in your browser:
- Local: **http://127.0.0.1:8080/**
- Network (bound on all interfaces): **http://10.137.229.176:8080/**

## Notes about building/constructing the site
- The Flask server is configured to serve static frontend files directly from `WebApp/`.
- The web pages load their assets (CSS/JS/images) from `WebApp/css`, `WebApp/js`, and `WebApp/images`.
- Form submissions or actions from the frontend may call PHP scripts under `WebApp/*.php`.

