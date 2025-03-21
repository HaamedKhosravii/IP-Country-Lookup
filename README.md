# IP Country Lookup
This is a restful API which returns the country data of a specific IP address.

## Run with docker

* First of all clone the project:
```
git clone https://github.com/HaamedKhosravii/IP-Country-Lookup
```
* Then, run the application by docker compose:
```
sudo docker compose up --build
```

## Run without docker

* First of all clone the project:
```
git clone https://github.com/HaamedKhosravii/IP-Country-Lookup
```
* Then, we need a virtual environment you can create like this:
```
virtualenv venv
```
* Activate it with the command below:
```
source venv/bin/activate
```
* After that, you must install all of the packages in `requirements.txt` file in project directory:
```
pip install -r requirements.txt
```
* Then, you should install PostgreSQL for for using it with our django project. For this, get help from the link below:

[How To Use PostgreSQL with your Django Application](https://www.digitalocean.com/community/tutorials/how-to-use-postgresql-with-your-django-application-on-ubuntu-20-04)

* Create a `.env` file in root directory and add your created config:
```python
SECRET_KEY = 'Your secret key generated by https://djecrety.ir'
DEBUG = 'Project debug status'

DB_NAME = 'Database name'
DB_USER = 'Database password'
DB_PASSWORD = 'Database password'
DB_HOST = 'Database host'
DB_PORT = 'Database port'
```
* After that, migration:
```
python3 manage.py migrate
```
* That's finished now you can run the project:
```
python3 manage.py runserver
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


