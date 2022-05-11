---
layout: default
title: Create a random planet
front: false
permalink: /planets/random
---

## {{page.title}}

Generate a 2D planet sprite randomly.

```
GET /planets
```

### Authorization
You can get an authorization token via the [login](./#login) endpoint.
- Bearer `token`


### Parameters

None

### Response
`200` status with a JSON object, containing:
- `type`: The type of planet generated
- `sprite_url`: The URL of the sprite asset

```json
{
    "type": "string",
    "sprite_url": "url"
}
```

> Note: Sprite URLs stay open during 30 seconds before being removed from the server.