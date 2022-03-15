# GET /stats

API Statistics

## Response

```json
{
    "detections": Number,
    "checks": Number,
    "domains": Number,
    "detectionList": {
        "example.com": Number
    }
}
```

### Response Parameters

| Name      | Type   | Description                  |
| --------- | ------ | ---------------------------- |
| detections | Number | Amount of messages/links that were detected |
| checks | Number | Amount of messages/links that were checked |
| domains | Number | Amount of domains in the blocklist |
| detectionList | Object | Per-Domain detection amounts |
