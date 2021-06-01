# CS569 Homework 10
### Delegated Authorization with OAuth 2.0 and Authentication
Create `UserModule` to allow users sign in, sign up, update their profile information for `user` entity as follows:
```javascript
[{ 
   _id: ObjectId, 
   fullname: String, 
   email: String, 
   password: String, 
   role: String,
   active: Boolean
}]
```
* Make sure the user's email is unique.
#### Backend
* Create two backend public routes: `POST /signup`, `POST /signin` both routes will generate a new token and send it as JSON in the response body.
* Create two backend private routes: `GET /user/:id`, `PUT /user/:id` to display and update user details. Users should be able to update their own profile.

### Research
Do your own research and explain what is a XSS scripting attack and what is a Cross-Site Request Forgery (CSRF) attack? How it happens? and How can we protect a web application from being vulnarable to CSRF attacks?
