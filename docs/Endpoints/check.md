# GET /check
Check whether or not a domain is in the blocklist

## Request Parameters
| Name   | Type   | Description                  | Optional           |
| ------ | ------ | ---------------------------- | ------------------ |
| domain | String | Domain that should be checked  | :x:              |

## Response

```json
{
    "blocked": Boolean,
    "reason": String,
    "timestamp": Number
}
```

### Response Parameters
| Name      | Type   | Description                  |
| --------- | ------ | ---------------------------- |
| blocked    | Boolean | Whether the domain is blocked |
| reason    | String | Reason for adding the domain |
| timestamp | Number | Time of adding the domain    |

``reason`` is only provided when ``blocked`` is ``true``

``timestamp`` is only provided when ``blocked`` is ``true`` and the domain is in the local blocklist
