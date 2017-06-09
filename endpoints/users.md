# /users

`GET /users` or `GET /users?key=value`  
Returns an array of [user objects](/models/User.md) (matching the given URL parameters)

---

`POST /users`  
Creates a new user account  
Parameters:  

| Key      | Type   | Description                        | Example             |
|----------|--------|------------------------------------|---------------------|
| email    | STRING | The email address to use for login | "matmen@menchez.me" |
| username | STRING | Your public display name           | "matmen"            |
| password | STRING | Your password                      | "secret12345"       |

---

`GET /users/:id`  
Returns an array filled with a single user object

---

:lock: `PUT /users/:id`  
Modifies the given user account.  
This takes in the same parameters as the `POST` request

---

:lock: `DELETE /users/:id`  
Deletes the given user account
