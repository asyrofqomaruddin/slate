# Consumers

## Register

> JSON response after register:

```json
{
  "status": "success",
  "data": {
    "consumer": {
      "id": 3,
      "email": "consumer@qvc.com",
      "fullname": "consumer",
      "authentication_token": "qmgg8t_sPyCJbNuMEXxyN",
      "user_channel": "consumer_16837950aa3911eb41e1b3f89d2ed140_channel",
      "balance": 0
    }
  }
```

This endpoint returns consumer credentials after creating consumer with the email and password.

### HTTP Request

`POST /consumers`

### Parameters

Parameter | Description
--------- | -----------
consumer[email] | The consumer's email.
consumer[password] | The consumer's password.
consumer[password_confirmation] | The consumer's password, again

<aside class="warning">
Remember — email are case insensitive
</aside>

## Login

> JSON response after login:

```json
{
  "status": "success",
  "data": {
    "consumer": {
      "id": 3,
      "email": "consumer@qvc.com",
      "fullname": "consumer",
      "authentication_token": "qmgg8t_sPyCJbNuMEXxyN",
      "user_channel": "consumer_16837950aa3911eb41e1b3f89d2ed140_channel",
      "balance": 0,
      "first_login": true
    }
  }
}
```

This endpoint returns consumer credentials after sending email and password.

### HTTP Request

`POST /consumers/session`

### Parameters

Parameter | Description
--------- | -----------
email | The consumer's email.
password | The consumer's password.


