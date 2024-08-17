Flask URL Shortener
Overview
This is a simple URL shortener built with Flask. The application allows users to create short URLs that redirect to longer URLs or serve files directly from the server. The project is a demonstration of basic Flask functionalities, including routing, form handling, session management, and error handling.

Features
Shorten URLs: Users can create short URLs that redirect to longer URLs.
File Uploads: Users can upload files and generate short URLs that link directly to these files.
Session Management: The application keeps track of shortened URLs created in the current session.
JSON Storage: URL mappings are stored in a JSON file (urls.json), making it easy to manage and access shortened URLs.
Error Handling: Custom 404 error page when a URL code is not found.
API Endpoint: An API endpoint is available to retrieve the list of URL codes created in the session.

Installation
Clone the repository:
git clone https://github.com/yourusername/flask-url-shortener.git
cd flask-url-shortener

Install the required Python packages:
pip install flask werkzeug

Run the application:
python app.py

Open your browser:
Visit http://127.0.0.1:5000 to access the home page of the URL shortener.
Project Structure
app.py: Main entry point for the Flask application.
templates/: Contains HTML templates for the home page, URL creation page, and custom 404 page.
static/user_files/: Directory where uploaded files are stored.
urls.json: JSON file where all shortened URLs and file paths are stored.

Routes
/: Home page displaying a form for creating new shortened URLs and a list of URLs created in the current session.
/your-url: Handles the form submission for creating a new shortened URL or uploading a file.
/<code>: Redirects to the original URL or serves the uploaded file corresponding to the short code.
/api: API endpoint that returns the list of URL codes created in the current session in JSON format.
Custom 404 page: Displays when a non-existent short code is accessed.
Usage
Shorten a URL:

Enter a custom code and a long URL in the form on the home page.
Click "Submit" to generate a shortened URL.
Upload a File:

Choose a file to upload and enter a custom code.
Click "Submit" to generate a shortened URL that links directly to the file.
Access the Shortened URL:

Visit http://127.0.0.1:5000/<code> to be redirected to the original URL or file.
Example
Creating a short URL for https://www.example.com with the code example would generate http://127.0.0.1:5000/example.
Uploading a file document.pdf with the code doc would generate http://127.0.0.1:5000/doc, which serves the file.
License
This project is licensed under the MIT License.

