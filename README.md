# JwtSecureWebApi
Example of JWT Authethication in ASP.NET Core 3.1


## How to run

Use the `dotnet run` command to start the server listening on http:5000 and https:5001.

Next step is to authenticate by issuing a http POST request with a valid `user` credentials.
You can do that using Postaman or curl. Here's a working curl example:

```
curl -k -d '{"username" : "user", "password" : "1234", "userrole" : "user", "fullname" : "Dan the Brave"}' -H 'Content-Type: application/json' https://localhost:5001/login
```

This will in turn, return a Json Web Token (JWT) that can the be used to access secured APIs
