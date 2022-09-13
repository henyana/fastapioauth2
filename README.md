### 1. Create the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
python -m venv env
```

### 2. Activate the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
env/Scripts/activate
```
### 3. Install the requirements library for Windows Users
In command terminal run the following command
```shell
python -m pip install -U pip
pip install -r requirements.txt
```

### 4. Test run the development
> hypercorn main:app --reload

### Open in your favorite browser 
1. http://127.0.0.1:8000/
2. Swagger documentation http://127.0.0.1:8000/docs

### Python Libraries
#fastapi
#hypercorn
#python-multipart
#tortoise-orm
#passlib
#bcrypt
#pyjwt

# Forked from this Youtube video https://www.youtube.com/watch?v=6hTRw_HK3Ts