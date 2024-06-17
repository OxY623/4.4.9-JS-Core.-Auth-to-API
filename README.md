1.Register User

POST https://blog.kata.academy/api/users
Body: {
  "user": {
    "username": "artem",
    "email": "artem@mail.com",
    "password": "12345678"
  }
}

2.Login User

POST https://blog.kata.academy/api/users/login
Body: {
  "user": {
    "email": "artem@mail.com",
    "password": "12345678"
  }
}

3.Current User

GET https://blog.kata.academy/api/user
Authorization Token "my_token"


Response:
{
    "user": {
        "username": "artem",
        "email": "artem@mail.com",
        "token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpZCI6IjY2NzA3ZThjZWYwMzkxMWIwMGFlZTA4YyIsInVzZXJuYW1lIjoiYXJ0ZW0iLCJleHAiOjE3MjM4MzMxODcsImlhdCI6MTcxODY0OTE4N30.D9H_tWk_tCg8vuZs8cJieeosYGp-Bt5yA7LB4tfacvc"
    }
}
