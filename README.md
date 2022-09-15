# FastAPI Authentication Example With OAuth2, Tortoise-orm & Sqlite3
### 1. Clone this repository 
``` sell
git clone https://github.com/henyana/fastapioauth2.git 
cd fastapioauth2
code . (will automatically open VS Code)
```

### 2. Open the terminal and Create the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
python -m venv env
```

### 3. Activate the Pyton virtual environment for Windows Users
In command terminal run the following command
```shell
env/Scripts/activate
```
### 4. Install the requirements library for Windows Users
In command terminal run the following command
```shell
python -m pip install -U pip
pip install -r requirements.txt
```

### 5. Test run the development
```shell 
hypercorn main:app --reload
```
### 5. Open in your favorite browser 
1. http://127.0.0.1:8000/
2. Swagger documentation http://127.0.0.1:8000/docs
### 6. Open Swagger documentation http://127.0.0.1:8000/docs
```
1. Collapse POST /users to Create a User
2. Click the Try it out button
3. Request body
{
   "username": "User1",
   "password_hash": "mysecret"
}
4. Clik the Execute button, make sure return Successful Response (200)
{
  "id": 1,
  "username": "User1",
  "password_hash": "$2b$12$VmoEoW6uiG75e4OtX3LAluzwanoztPwJqR6bdnQ3T1qbc5tAOBolO"
}
```

### 7. Test Generate Token
```
1. Collapse POST /token to Generate Token
2. Click the Try it out button
3. Request body, fill the 
    username field in as "User1",
    password field in as "mysecret"
}
4. Clik the Execute button, make sure return Successful Response (200)
{
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpZCI6NCwidXNlcm5hbWUiOiJVc2VyMSIsInBhc3N3b3JkX2hhc2giOiIkMmIkMTIkVm1vRW9XNnVpRzc1ZTRPdFgzTEFsdXp3YW5venRQd0pxUjZiZG5RM1QxcWJjNXRBT0JvbE8ifQ.t0Ii_txABTHjP0ZyrD-s8sobjWqkvwmXpJtyjzOV_PI",
  "token_type": "bearer"
}
```
### Python Libraries
#fastapi
#hypercorn
#python-multipart
#tortoise-orm
#passlib
#bcrypt
#pyjwt

# Forked from this Youtube video https://www.youtube.com/watch?v=6hTRw_HK3Ts