# Project Setup and Execution Guide

## This guide provides step-by-step instructions to set up and execute the project on macOS.
### Installations on macOS

Step 1: Install Python using Homebrew
* Install Homebrew (if not already installed):
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

* Install Python:
brew install python

* Verify Python installation:
python3 --version

Step 2: Install pip
* Download get-pip.py:
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py

* Install pip:
python3 get-pip.py

* Verify pip installation:
pip3 --version

Step 3: Install Flask
* Install Flask:
pip3 install Flask

Step 4: Install SQLite3
* Install SQLite3 using Homebrew:
brew install sqlite
* Verify SQLite3 installation:
sqlite3 --version

Step 5: Create a Database and a Table using SQLite3
* Open SQLite3:
sqlite3 mydatabase.db
* Create a table:
CREATE TABLE users (
    id INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    email TEXT NOT NULL UNIQUE
);
* Insert data into the table:
INSERT INTO users (name, email) VALUES ('John Doe', 'john@example.com');
* Query data from the table:
SELECT * FROM users;

Step 6: Set Up a Virtual Environment
* Create a virtual environment:
python3 -m venv venv
* Activate the virtual environment:
source venv/bin/activate

Step 7: Install Required Python Packages
* Install requests:
sudo pip install requests

* Install passlib:
pip install passlib

Step 8: Run the Server
* Execute the server:
python3 server.py
