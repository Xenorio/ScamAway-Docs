# POST /report
Report a URL

**Note:**
The API only accepts full URLs, only domains will be rejected.

If the report does not originate from a Discord user, please put other identifying info in the ``user`` parameter.

## Request Parameters

| Name   | Type   | Description                  | Optional           |
| ------ | ------ | ---------------------------- | ------------------ |
| url | String | URL to report  | :x:                |
| user | String | User tag of the reporter | :x: |

## Response

```json
{
  "success": true
}
```

## Errors

- No URL provided
- Invalid URL
- No user provided | If not reporting through Discord, please provide something identifying
