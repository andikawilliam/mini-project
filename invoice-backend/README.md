
# Django API Server

## Run

> **Step #1** -  Clone the sources

```bash
$ git clone https://github.com/app-generator/invoice-backend.git
$ cd invoice-backend
```
<br />

> **Step #2** - Create a virtual environment

```bash
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
```

<br />

> **Step #3** - Install dependencies using PIP

```bash
$ pip install -r requirements.txt
```

<br />

> **Step #4** - Start the API server

```bash
$ python manage.py migrate
$ python manage.py runserver
```

The API server will start using the default port `8000`.

<br />

## ✨ Tests

```bash 
$ python manage.py test
```

<br />

## API

> **Register** - `api/users/signup`

```
POST api/users/signup
Content-Type: application/json

{
    "username":"test",
    "password":"pass", 
    "email":"test@gmail.com"
}
```

<br />

> **Login** - `api/users/login`

```
POST /api/users/login
Content-Type: application/json

{
    "password":"pass", 
    "email":"test@gmail.com"
}
```

<br />

> **Logout** - `api/users/logout`

```
POST api/users/logout
Content-Type: application/json
authorization: JWT_TOKEN (returned by Login request)

{
    "token":"JWT_TOKEN"
}
```

<br />

---

