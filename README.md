# Authentication API with JWT Token in Node.js




## Authentication 
Process of verifying the user. (verifying what they have to access )
## Authorization 
Determines what users can and cannot access
## JWT
It consist of three parts separated by dots (.),

1. Header-  consists of two parts: the type of the token, which is JWT, and the signing algorithm 
2. Payload-  contains the claims. Claims are statements about an entity (typically, the user) and additional data
3. Signature- encoded header
![image](https://user-images.githubusercontent.com/64850016/171610337-c29c2e0e-e679-4348-9f42-afa24e09304c.png)

```bash
xxxxx.yyyyy.zzzzz

eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJ1c2VyX2lkIjoiNjI5ODUxNTcyODdiNzkyNTNmYzE5YjM1IiwiZW1haWwiOiJzdWRhbUBnbWFpbC5jb20iLCJpYXQiOjE2NTQxNTcwMjAsImV4cCI6MTY1NDE2NDIyMH0.CZ01aCZfpF0k8Pdvun4SJWtOE_EJl6gZusr91csHnQc
```
## Access token
Access tokens are used as bearer tokens. A bearer token means that the bearer (who holds the access token) can access authorized resources without further identification.

Have a short lifespan for security purpose. When it expires, the user must authenticate again to get a new access token.

## Refresh token
This token is a long-lived token compared to the access token and is used to request a new access token in cases where it is expired.


