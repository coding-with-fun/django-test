# django-test

## Requests

1. API URL -
```
curl -X POST -H "Content-Type: application/json" -d '{"username":"testuser", "password1":"testpassword", "password2":"testpassword"}' localhost:8000/registration/
```
```
Response: {"key":"1565c60a136420bc733b10c4a165e07698014acb"}
```

2. API URL -
```
curl -X GET -H 'Authorization: Token 1565c60a136420bc733b10c4a165e07698014acb' localhost:8000/api/welcome
```
```
Response {"message": "Welcome AH_Bookstore App!"}
```

3. API URL -
```
curl -X GET -H '' localhost:8000/api/welcome
```
```
Response {"detail":"Authentication credentials were not provided."}
```