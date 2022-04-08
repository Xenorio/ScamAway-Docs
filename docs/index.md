# Getting Started
Welcome to the ScamAway API documentation!

This documents interaction with the [API](https://github.com/Xenorio/ScamAway-API) for the [ScamAway Discord bot](https://github.com/Xenorio/ScamAway)

If you want to host the API yourself, head to [Setup](setup.md)

## Requesting
All requests must be sent to ``https://scamaway.xenorio.xyz/api/<endpoint>``

Depending on the endpoint, you need to send either a ``GET`` or ``POST`` request

### Get Parameters
Parameters for ``GET`` requests must be added to the URI by appending ``?parameter1=value&parameter2=value`` to the end

### Post Parameters
Parameters for ``POST`` requests must be added as JSON data inside the request body. Please make sure to set the ``Content-Type`` header to ``application/json``

## Identification
You may provide some identifying info like your website, GitHub profile, Discord guild, or similar with the ``X-Identity`` header.
If the ``forceIdentification`` config entry is set to ``true`` (which it is on scamaway.xenorio.xyz) this is mandatory.

## Authorization
Administrative endpoints need an API key sent in the ``Authorization`` header. This key needs to match with the API configuration.

## Errors
When an error is encountered, the API will respond with a non-200 response code and JSON data with more information

```json
{
    "error": "Something went wrong!"
}
```