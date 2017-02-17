![featured-image](https://raw.githubusercontent.com/andela-mnzomo/project-dream-team-three/master/flask-crud-part-three.jpg)

The complete code for my three-part tutorial, *Build a CRUD Web App With Python and Flask*, which you can find on Scotch.io [here](https://scotch.io/tutorials/build-a-crud-web-app-with-python-and-flask-part-three).

## Installation and Set Up
Prerequisites:
* [Python 2](https://www.python.org/download/releases/2.7.2/)
* [virtualenv](https://virtualenv.pypa.io/en/stable/)

Clone the repo from GitHub:
```
git clone https://github.com/andela-mnzomo/project-dream-team-three
```

Create a virtual environment for the project and activate it:
```
virtualenv dream-team
source dream-team/bin/activate
```

Install the required packages:
```
pip install -r requirements.txt
```

## instance/config.py file
Create a directory, `instance`, and in it create a `config.py` file. This file should contain configuration variables that should not be publicly shared, such as passwords and secret keys. The app requires you to have the following configuration
variables:
* SECRET_KEY
* SQLALCHEMY_DATABASE_URI

## Database configuration
You will need to create a database, after which you can run migrations as follows:

* `flask db migrate`
* `flask db upgrade`

## Launching the Program
Set the FLASK_APP and FLASK_CONFIG variables as follows:

* `export FLASK_APP=run.py`
* `export FLASK_CONFIG=development`

You can now run the app with the following command: `flask run`

## Testing
To test, run the following command: `python tests.py`

## Built With...
* [Flask](http://flask.pocoo.org/)

## Credits and License

Copyright (c) 2017 [Mbithe Nzomo](https://github.com/andela-mnzomo)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
