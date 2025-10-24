# Python Health Check App

A minimal Flask application that exposes a `/health` endpoint for basic service monitoring.

## 🔧 Features

- Lightweight Flask setup
- `/health` route returns `{"status": "ok"}` with HTTP 200
- Ready for CI/CD integration and containerization

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/python-healthcheck-app.git
cd python-healthcheck-app

### 2. Create and aacitvate virtual environment
'''bash
python -m venv venv
venv\Scripts\activate  # Windows

### 3. Install dependencies
pip install -r requirements.txt
### Troubleshooting
ModuleNotFoundError: No module named 'flask'
  -make sure the virtual environment is activated
  '''bash
  venv\Scripts\activate  # Windows
  -you should see (venv) at the start of your terminal prompt
  -confirm you are using the correct python
  '''bash
  where python
  -you should see a path like (..python-healthcheck-app\venv\Scripts\python.exe
  -if it points your system python (eg., C:\Windows\...), your virtual environment is not active
  -install Flask manually
  -if requirements.txt fails, try:
  '''bash
  pip install flask
  -then re-run
  '''bash
  python app.py
  -you should see running on http://127.0.0.1:5000/
DO NOT FORGET TO CREATE THE "DOCKERFILE", otherwise, you will have a problem in the buildspec.yaml when trying to build the docker file in the build phase.
