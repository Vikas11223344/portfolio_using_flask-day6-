# Portfolio using Flask (Day 6)

A simple portfolio website built with Flask. This project demonstrates a small personal portfolio application created as part of a Flask learning exercise (day 6). It includes routes, templates, static assets (CSS, images), and basic configuration to run locally and deploy.

Features
- Simple, responsive portfolio pages (Home, About, Projects, Contact)
- Uses Flask templating (Jinja2) and static assets
- Example contact form (server-side handling) or placeholder for integration
- Clear, minimal project structure suitable for extension

Prerequisites
- Python 3.7 or newer
- pip (Python package installer)
- (Optional) virtualenv or venv for an isolated environment

Installation
1. Clone the repository:
   git clone https://github.com/Vikas11223344/portfolio_using_flask-day6-.git
   cd portfolio_using_flask-day6-

2. Create and activate a virtual environment (recommended):
   python -m venv venv
   # On macOS/Linux
   source venv/bin/activate
   # On Windows (PowerShell)
   .\venv\Scripts\Activate.ps1

3. Install dependencies (if requirements.txt exists):
   pip install -r requirements.txt

Running the app locally
- If the project provides an entry point (app.py, run.py, or a package), run it directly, for example:
  python app.py

- Or use Flask's CLI:
  export FLASK_APP=app.py    # macOS/Linux
  set FLASK_APP=app.py       # Windows (cmd)
  $env:FLASK_APP = "app.py" # Windows (PowerShell)
  export FLASK_ENV=development
  flask run

Then open http://127.0.0.1:5000 in your browser.

Project structure (example)
- app.py or run.py         # Application entry point
- requirements.txt        # Python dependencies
- templates/              # Jinja2 templates (index.html, about.html, etc.)
- static/
  - css/                  # Stylesheets
  - js/                   # JavaScript files
  - images/               # Image assets
- README.md               # This file

Configuration and environment
- Keep secrets and API keys out of the repository. Use environment variables or a .env file and a library like python-dotenv if needed.

Deployment
- This project can be deployed to any WSGI-compatible host (Gunicorn + Nginx, Heroku, Render, Railway, etc.).
- For production, serve static files via a web server (Nginx) or the platform's static file handling, and run the Flask app with Gunicorn (or equivalent).

