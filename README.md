FLASK URL SHORTENER
===================

OVERVIEW
--------
This Flask-based URL shortener allows users to create short URLs that redirect to longer URLs or serve files directly from the server. The project includes features like file uploads, session management, and error handling, all managed through a simple and responsive interface.

FEATURES
--------
- Shorten URLs:
  Users can create short URLs that redirect to specified long URLs.
  
- File Uploads:
  Users can upload files and generate short URLs that link directly to these files.

- Session Management:
  The application keeps track of shortened URLs created within the current session.

- JSON Storage:
  URL mappings are stored in a JSON file (`urls.json`), making it easy to manage and access shortened URLs.

- Error Handling:
  Custom 404 error page displayed when a non-existent short code is accessed.

- API Endpoint:
  An API endpoint is available to retrieve the list of URL codes created in the session.

USAGE
-----
1. Clone the Repository:
2. git clone https://github.com/yourusername/flask-url-shortener.git
cd flask-url-shortener


2. Install Required Dependencies:
pip install -r requirements.txt

3. Run the Flask Application:
python app.py

4. Access the Application:
- Open your web browser and visit `http://localhost:5000` to access the URL shortener.

TECHNOLOGIES USED
-----------------
- Flask
- Werkzeug
- JSON
- HTML/CSS
- JavaScript

LICENSE
-------
This project is licensed under the MIT License. See the LICENSE file for deta
