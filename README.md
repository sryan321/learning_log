# Learning Log Application

A simple Django-based web application for keeping track of what you've learned. 
It allows users to create, view and manage entries related to topics or subjects they are studying.

## Features

- **Create new entries** for topics or lessons learned.
- **View a list of all entries** with title, date, and details.
- **Edit and delete entries** for each learning log.
- **Simple user authentication** via login system.
- **Tag entries** with categories or keywords (optional feature).

## Requirements

- Python 3.8 or newer
- Django 3.0 or newer
- SQLite (default database), or another database (PostgreSQL, MySQL, etc.)
- pip (Python package manager)

## Installation

### 1. Clone the Repository

Clone this repository to your local machine:

    git clone https://github.com/sryan321/learning-log.git
    cd learning-log

### 2. Create a Virtual Environment (Optional but Recommended)

It's recommended to use a virtual environment to isolate the project dependencies:

    python3 -m venv venv

Activate the virtual environment:

On Windows:

    venv\Scripts\activate

On macOS/Linux:

    source venv/bin/activate


### 3. Install Dependencies

Install the required packages using pip:

    pip install -r requirements.txt


### 4. Set Up the Database

Run the following command to apply the initial migrations and set up the database:

    python manage.py migrate


### 5. Run the Development Server

To start the Django development server, use the following command:

    python manage.py runserver

Visit http://127.0.0.1:8000 in your web browser to view the application.



### Usage

Once the server is running, you can:

Create a learning log entry: After logging in (if authentication is enabled), go to the "Add New Entry" page, fill in the details about your learning experience and submit the form.
View all entries: The homepage will display a list of all your learning entries. You can click on any entry to view its details.
Edit or delete an entry: If you created an entry, you can edit or delete it via the entry's detail page.

### Configuration

Database: The application uses SQLite by default, but you can configure it to use other databases such as PostgreSQL or MySQL by updating the DATABASES setting in settings.py.

Authentication: The application supports user authentication. Users can create an account to log in and have their own separate learning logs.

### Running Tests

To run tests for the Learning Log app, use the Django test command:

    python manage.py test
