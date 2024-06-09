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




### Visual Demonstrations

<img width="1457" alt="Screenshot 2024-06-09 at 11 16 00 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/6e6d0bc5-e191-462f-bfcc-154410b55fa6">
<img width="1457" alt="Screenshot 2024-06-09 at 11 17 06 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/0f58de70-872e-4581-8487-da69784ad941">
<img width="1457" alt="Screenshot 2024-06-09 at 11 17 56 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/1b7a2176-3650-42b1-b625-5ab5866cd1ad">
<img width="1457" alt="Screenshot 2024-06-09 at 11 18 41 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/f4eb98ee-6031-40a1-a956-1d2dfc40765f">
<img width="640" alt="Screenshot 2024-06-09 at 11 19 30 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/d865a8d4-a35a-408b-93ba-6de86ac1ded5">
<img width="574" alt="Screenshot 2024-06-09 at 11 20 45 AM" src="https://github.com/akhilandeswariVegi/pythonFlaskWebFramework/assets/22704150/9fa886b7-a7e2-4b0c-91fd-8059420964aa">

