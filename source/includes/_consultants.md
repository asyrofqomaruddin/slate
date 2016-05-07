# Consultant

## Register

> JSON response after register:

```json
{
  "status": "success",
  "data": {
    "id": 2,
    "email": "consultant2@email.mock",
    "fullname": "consultant2",
    "verified": false,
    "authentication_token": "qEGzV6ZG-UYrT6sy61ygz",
    "user_channel": "consultant_26a4de8dddaf9e5cfffa5846e70060d4_channel",
    "rate": 0,
    "available": false,
    "balance": 0,
    "image": "https://someplace.com/uploads/consultants/2"
  }
}
```

This endpoint returns consultant credentials after creating consultant with the email and password.

### HTTP Request

`POST /consultants`

### Parameters

Parameter | Description
--------- | -----------
consultant[email] | The consultant's email.
consultant[password] | The consultant's password.
consultant[password_confirmation] | The consultant's password, again

<aside class="warning">
Remember — email are case insensitive
</aside>

## Login

> JSON response after login:

```json
{
  "status": "success",
  "data": {
    "id": 2,
    "email": "consultant2@email.mock",
    "fullname": "consultant2",
    "verified": false,
    "authentication_token": "qEGzV6ZG-UYrT6sy61ygz",
    "user_channel": "consultant_26a4de8dddaf9e5cfffa5846e70060d4_channel",
    "rate": 0,
    "available": false,
    "balance": 0,
    "image": "https://someplace.com/uploads/consultants/2"
  }
}
```

This endpoint returns consultant credentials after sending email and password.

### HTTP Request

`POST /consultants/session`

### Parameters

Parameter | Description
--------- | -----------
email | The consultant's email.
password | The consultant's password.


