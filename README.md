# Codeigniter REST API in 30 minutes

Support for Restful API using Codeigniter (login, CRUD) in 30 minutes.

# Demo
[Visit Here](https://youtu.be/X2i-rt0yxDQ)

# Setup
Download the setup
and then config & import MySQL database 

You can use [POSTMAN](https://www.getpostman.com/) or anything else for simulate frontend

# Test the API
You can test the API by including header `Content-Type`,`Client-Service` & `Auth-Key` with value `application/json`,`frontend-client` & `simplerestapi` in every request

And for API except `login` you must include `id` & `token` that you get after successfully login. The header for both look like this `User-ID` & `Authorization`

List of the API :

`[POST]` `/auth/login` json `{ "username" : "admin", "password" : "Admin123$"}`

`[GET]` `/book`

`[POST]` `/book/create` json `{ "title" : "x", "author" : "xx"}`

`[PUT]` `/book/update/:id` json `{ "title" : "y", "author" : "yy"}`

`[GET]` `/book/detail/:id`

`[DELETE]` `/book/delete/:id`

`[POST]` `/auth/logout`
