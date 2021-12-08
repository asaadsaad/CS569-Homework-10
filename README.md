# CS569 Homework 10
### Authorization and Authentication
Following up on yesterday's homework, and having a schema with the following structure:
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
#### Backend
* Create two backend public routes: `POST /signup`, `POST /signin` both routes will generate a new token and send it as JSON in the response body.
* Protect all courses/students routes with a middleware that checks and validates the token in the header.
* Update the pagination functionality for the `GET /courses` and `GET /students` requests with standard response pagination headers.
* Create an index to assure the user's email is unique.
#### Frontend
* Create `SignIn` and `SignUp` components.
* Protect all other routes in your application with `Guards` to ensure a token exists before navigation.
* Implement an interceptor to support:
  * Sending the token in the request header if exists.
  * Parsing pagination headers in the response and passing it to the components if exist.
  
### Security
Do your research and explain what is a XSS scripting attack and find answers to the following questions:
* What is a Cross-Site Request Forgery (CSRF) attack? 
* What is Cross-Site Scripting (XSS) attack? 
* How can we protect a web application from being vulnarable to CSRF and XSS attacks?
* Explain how Angular protects your application from CSRF and XSS attacks?
