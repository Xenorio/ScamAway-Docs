# GET /whitelist
Get a list of all domains in the whitelist

Used to prevent API spam. This list is cached on the client, and any domains in it do not get checked with the API.

## Response

```json
[
    {
        "domain": String,
        "reason": String,
        "timestamp": Number
    }
]
```

### Response Parameters
| Name   | Type   | Description                  | 
| ------ | ------ | ---------------------------- |
| domain | String | The domain | 
| reason | String | Reason for adding the domain | 
| timestamp | Number | Time of adding the domain |
