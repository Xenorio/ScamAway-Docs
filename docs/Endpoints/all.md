# GET /all
Get a list of all domains in the local blocklist

!!! warning "This does not include external lists (phish.sinking.yachts)

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
