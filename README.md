# Magnitex API Documentation
---

### Models
##### [User](models/User.md) | [AccessToken](models/AccessToken.md) | [Bot](models/Bot.md)

---

### Endpoints
##### [users](endpoints/users.md) | [access_tokens](endpoints/access_tokens.md) | [bots](endpoints/bots.md)
<br>
Methods marked with a :lock: symbol must be called with valid authentication in the form of a Authentication header. The header must be in the form of `Authentication: Bearer TOKEN`

---

### Default Responses
##### Successful
```js
{
  meta: {
    total: 0
    count: 0,
    offset: 0,
    error: null
  },
  data: []  // Array of model objects
}
```

##### Error
```js
{
  meta: {
    total: 0
    count: 0,
    offset: 0,
    error: {
      message: "",  // A message describing what happened,
      details: {} // Optional, an Object<String, Array<String>> containing further info
    }
  },
  data: []  // Empty array
}
```
