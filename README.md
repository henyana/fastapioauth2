### Create the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
python -m venv env
```

### Activate the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
env/Scripts/activate
```

### Test run the development
> hypercorn main:app --reload

### Open in your favorite browser 
1. http://127.0.0.1:8000/
2. Swagger documentation http://127.0.0.1:8000/docs

### Libs
fastapi
hypercorn
python-multipart
tortoise-orm
passlib
bcrypt
pyjwt
