# 1. Make Toingg

## Description
This API endpoint allows you to make a Toingg.

## Request Method
POST

## URL
`/make_toingg/`

## Parameters
- `apiKey` (*string*, query) - The API key required for authentication.

## Request Body
- Content Type: application/json
- Example Value:
```json
{
  "campaign": "string",
  "name": "string",
  "phoneNumber": "string"
}
```

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```

# 2. Make Toingg Details

## Description
This API endpoint allows you to make details for a Toingg.

## Request Method
POST

## URL
`/make_toingg_details/`

## Parameters
- `apiKey` (*string*, query) - The API key required for authentication.

## Request Body
- Content Type: application/json
- Example Value:
```json
{
  "campaignName": "string",
  "campaignScript": "string",
  "name": "string",
  "phoneNumber": "string"
}
```

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```


# 3. Make Batch Toingg

## Description
This API endpoint allows you to make a batch Toingg.

## Request Method
POST

## URL
`/make_batch_toingg/`

## Parameters
- `apiKey` (*string*, query) - The API key required for authentication.

## Request Body
- Content Type: application/json
- Example Value:
```json
{
  "campaign": "string",
  "numberList": [
    {
      "clientName": "string",
      "clientNumber": "string"
    }
  ]
}
```

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```

# 4. Send SMS

## Description
This API endpoint allows you to send an SMS.

## Request Method
POST

## URL
`/send_sms/`

## Parameters
- `apiKey` (*string*, query) - The API key required for authentication.

## Request Body
- Content Type: application/json
- Example Value:
```json
{
  "name": "string",
  "phoneNumber": "string",
  "message": "string"
}
```

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```

# 5. Hang Up Call

## Description
This API endpoint allows you to hang up a call.

## Request Method
POST

## URL
`/hang_up_call/`

## Parameters
- `callSid` (*string*, query) - The unique identifier for the call session.
- `apiKey` (*string*, query) - The API key required for authentication.

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```

# 6. Create Checkout Session

## Description
This API endpoint allows you to create a checkout session.

## Request Method
POST

## URL
`/create-checkout-session`

## Parameters
No parameters are required.

## Request Body
- Content Type: application/json
- Example Value:
```json
{
  "apikey": "string"
}
```

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
- **422** - Validation Error
  - Media Type: application/json
  - Example Value:
```json
{
  "detail": [
    {
      "loc": [
        "string",
        0
      ],
      "msg": "string",
      "type": "string"
    }
  ]
}
```

# 7. Stripe Webhook

## Description
This API endpoint represents a Stripe webhook.

## Request Method
POST

## URL
`/webhook`

## Parameters
No parameters are required.

## Responses
- **200** - Successful Response
  - Media Type: application/json
  - Example Value: `"string"`
```