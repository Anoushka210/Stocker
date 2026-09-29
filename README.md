# Stocker 📈

Stocker is a lightweight, responsive web application designed for tracking and managing stock portfolios. Built with Python and Flask, it leverages Amazon DynamoDB for scalable, low-latency data storage.

## 🚀 Features
* **Stock Tracking:** Monitor real-time or historical stock performance data.
* **Portfolio Management:** Add, update, and remove stock assets from your user profile.
* **AWS Integration:** Uses DynamoDB to ensure secure and fast data persistence.

## 📁 Project Structure
* `app.py` — The core Flask application server containing API routes and business logic.
* `setup_dynamodb.py` — A utility script to initialize AWS DynamoDB tables and schemas.
* `requirements.txt` — List of Python dependencies required to run the project.
* `templates/` — HTML layout files rendered dynamically by Flask.
* `static/` — Frontend assets including CSS styling, client-side JavaScript, and images.

## 🛠️ Installation & Setup

### 1. Clone and Navigate to the Repository
```bash
git clone https://github.com
cd Stocker
```

### 2. Set Up a Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure AWS Credentials
Ensure you have your AWS credentials configured locally to allow connection to DynamoDB:
```bash
aws configure
```

### 5. Initialize the Database
Run the setup script to create the required DynamoDB tables:
```bash
python setup_dynamodb.py
```

### 6. Run the Application
Start the Flask development server:
```bash
python app.py
```
Open `http://127.0.0.1:5000` in your web browser to view the application.
