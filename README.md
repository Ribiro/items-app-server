# Items-App-Server
Items-App-Server is a Django Rest Framework API that serves the <a href="https://github.com/Ribiro/items-app-client">Items-App-Client</a> front end developed using Vue JS.
To execute the api, follow these procedures:

1. Clone the repository in your local machine:
```
git clone https://github.com/Ribiro/items-app-server

```

2. Create a new virtual environment using virtualenv or venv. If you don't have these packages installed, you can install them using pip:
```
pip install virtualenv

virtualenv env


```

4. Activate your virtual environment:

```
source env/bin/activate

```

or

```
source env/Scripts/activate (for Windows)

```

4. Install the dependencies by running the following command in the terminal:
```
pip install -r requirements.txt

```

5. Run the migrations by running the following command in the terminal:
```
python manage.py migrate

```

If for some reson step no. 5 fails, try these:
```
rm db.sqlite3
python manage.py makemigrations
python manage.py migrate users
python manage.py items_app
python manage.py migrate


```
NB: The purpose here is to ensure all migrationsa re executed, otherwise the server won't run.


6. Once the migrations are done, run the server:

```
python manage.py runserver

```


Once the server is up and running, proceed to start the <a href="https://github.com/Ribiro/items-app-client">Items-App-Client.</a>


