# CS569 Homework 13
### Delegated Authorization with OAuth 2.0 and Authentication
Add a new `user` entity to Homework 12:
```javascript
[{ 
   _id: ObjectId, 
   fullname: String, 
   email: String, 
   password: String, 
   active: Boolean
}]
```
Create two public routes: `/signup`, `/signin` both routes will generate a new token and send it as JSON in the response body.
Protect all other routes with a middleware that checks the token validity in the header of all incoming requests.