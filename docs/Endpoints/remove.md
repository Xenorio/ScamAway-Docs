# POST /remove
!!! info "Administrative Endpoint"
Removes a domain from the blocklist

## Request Parameters

| Name   | Type   | Description                  | Optional           |
| ------ | ------ | ---------------------------- | ------------------ |
| domain | String | Domain that should be added  | :x:                |

## Response

```json
{
  "success": true
}
```

## Errors

- No domain provided
- Domain is not being blocked
