## Set up

```bash
$ # Clone sources
$ git clone https://github.com/app-generator/flask-pandas-dataframe.git
$ cd flask-pandas-dataframe

$ sudo apt install python3-virtualenv

$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
$
$ # Install dependencies
$ pip3 install -r requirements.txt
$
$ # Create database via Flask CLI
$ flask shell
>>> from app import db  # import SqlAlchemy interface
>>> db.create_all()     # create SQLite database and Data table
>>> quit()              # leave the Flask CLI  
$
$ # Load the data into the database
$ flask load-data titanic-min.csv
$
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=app.py
$
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$
$ flask run --host=0.0.0.0 --port=31201
```
