
express is a backend framework for node. used to create api from your databases which can be accessed by the frontend.

```
npm install express
```

```
const express = require('express')
```

then you create a function that invokes the app

## Nodemon

just like live server. updates backend without closing and opening again.

i used nodemon- script dev. -> npm run dev

---
### Routing
```
app.get('/',(req, res)=>{

res.json({mssg: 'welcome to the app'});

})
```

![[Pasted image 20260621171121.png]]



---

### POSTMAN

whenever creating a full stack app.**create backend first**.

now to test backend. use postman

in it there is option to check the----
GET,  POST, PUT, PATCH, DELETE...etc

now what these are---

-> these are http requests

#### GET
server bring this data to me

#### POST
server i have some data. take this and put it in the database

#### PUT / PATCH
server update this data

#### DELETE
server find this data using the id and delete it.

---


