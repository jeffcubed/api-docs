# /users

`GET /users` or `GET /users?key=value`  
Returns an array of [user objects](/models/User.md) (matching the given URL parameters)

---

`POST /users`  
Creates a new user account  
Returns a [verification token](../VerificationToken.md)    
Parameters:  

| Key      | Type   | Description              | Example       |
|----------|--------|--------------------------|---------------|
| username | STRING | Your public display name | "matmen"      |
| password | STRING | Your password            | "secret12345" |

---

`GET /users/:id`  
Returns an array filled with a single user object matching the ID

---

:lock: `PUT /users/:id`  
Modifies the given user account  
Returns the updated user model  
This takes in the same parameters as the `POST` request

---

:lock: `DELETE /users/:id`  
Deletes the given user account
Returns the deleted account's data
