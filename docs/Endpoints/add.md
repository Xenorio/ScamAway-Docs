# POST /add
!!! info "Administrative Endpoint"
Adds a domain to the blocklist

## Request Parameters
| Name | Type | Description | Optional |
|---|---|---|---|
| domain | String | Domain that should be added | :x: |
| reason | String | Reason for adding the domain | :white_check_mark: |
| forward | String | URL to forward to Fish Fish | :white_check_mark: |

## Response

```json
{
    "success": true
}
```

## Errors
- No domain provided
- Invalid domain
- Domain is already being blocked
