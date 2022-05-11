---
layout: default
title: Login
front: false
permalink: /authentication/login
---

## {{page.title}}

Get a temporary access token.

```
POST /login
```

### Body
You must provide an API key inside a JSON body, with the key `api_key`.

```json
{
    "api_key": "Your API key as string"
}
```

### Response
`200` status with a JSON object, containing:
- `message`: The type of planet generated
- `token`: The access token, used to authenticate for your next requests

```json
{
    "message": "string",
    "token": "string"
}
```

> Note: Tokens are valid during 24h. You need to get a new token once a given one expires.