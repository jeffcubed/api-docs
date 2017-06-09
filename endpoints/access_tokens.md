# /access_tokens

`POST /access_tokens`  
Creates a new access token (logs the user in)  
Returns the generated access token token  
Parameters:  

| Key        | Type   | Description                  | Example             |
|------------|--------|------------------------------|---------------------|
| grant_type | STRING | The token type to generate   | "bearer"            |
| email      | STRING | The account's e-mail address | "matmen@menchez.me" |
| password   | STRING | The account's password       | "secret12345"       |

---

`GET /access_tokens/:token`  
Returns an array filled with the user corresponding to the access token

---

:lock: `DELETE /access_tokens/:id`  
Deletes the given access token (logs the user out)
Returns the deleted access token's data
