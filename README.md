# Magnitex API Documentation
---

### Models
##### [User](models/User.md) | [AccessToken](models/AccessToken.md) | [Bot](models/Bot.md)

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
