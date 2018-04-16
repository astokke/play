# Getting Started

## Overview

The Yr API Yr is a joint service by the Norwegian Meteorological Institute and the Norwegian Broadcasting Corporation.

## Technical Overview

The Yr API is a REST API that can be used to access weather data from around the world.
Response from the API will be in JSON format.

Endpoint:

```
http://www.yr.no/api/
```

### Authentication

Include your API key in requests to authenticate your account. The Yr API is free to use, but it requires you to register to get an API key.
If you do not have an API key yet, [click here](https://api.yr.no/) to register.

### Caching

[ to do ]

### Error Handling

The Yr API uses standard HTTP response codes to indicate whether or not the API request was a success.

## Object Model

```curl
    curl -X GET --header 'Accept: application/json' 'https://www.yr.no/api/v0/locations/1-72837'
```

```javascript
{
  "category": {
    "id": "CB09",
    "name": "By"
  },
  "id": "1-72837",
  "name": "Oslo",
  "position": {
    "lat": 59.91273,
    "lon": 10.74609
  },
  "elevation": 10,
  "timeZone": "Europe/Oslo",
  "urlPath": "Norge/Oslo/Oslo/Oslo",
  "country": {
    "id": "NO",
    "name": "Norge"
  },
  "region": {
    "id": "NO/03",
    "name": "Oslo"
  },
  "subregion": {
    "id": "NO/03/0301",
    "name": "Oslo"
  },
  "_links": {
    "self": {
      "href": "/api/v0/locations/1-72837"
    },
    "celestialevents": {
      "href": "/api/v0/locations/1-72837/celestialevents"
    },
    "forecast": {
      "href": "/api/v0/locations/1-72837/forecast"
    },
    "notifications": {
      "href": "/api/v0/locations/1-72837/notifications"
    },
    "now": {
      "href": "/api/v0/locations/1-72837/forecast/now"
    }
  }
}
```

[to do]

## Symbols

[to do]

## Changelog

Follow yr-api @github [ ? ]

## Mobile developers

Find our API clients for mobile development here:

iOs: [YR SwiftClient](https://github.com/YR/yr-swiftclient)

Android: ??
