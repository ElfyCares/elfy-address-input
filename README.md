[![Build Status](https://travis-ci.org/ElfyCares/elfy-address-input.svg?branch=master)](https://travis-ci.org/ElfyCares/elfy-address-input)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/ElfyCares/elfy-address-input)

# \<elfy-address-input\>

A Polymer 2 element which helps you to input addresses with ease and allows users to adjust the details.

## `address` property

```
{   
    "name": "Solomon R. Guggenheim Museum",
    "street": "1071 5th Avenue",
    "streetNumber": "10",
    "city": "New York",
    "state": "New York",
    "stateCode": "NY",
    "postalCode": "10128",
    "country": "United States",
    "countryCode": "US",
    "phone": "(212) 423-3500"
    "latLng": {
        "lat": 40.7829796,
        "lng": -73.95897059999999
    },
    "address_1": `${address.street} ${address.streetNumber || ''}`,
    "address_2": `${address.postalCode || ''} ${address.state || ''}`,
    "address_3": `${address.country || ''}`,
    "address_full": `${address.address_1}, ${address.address_2}, ${address.address_3}`,
    "address_short": `${address.address_1}, ${address.address_2}`
}
```

## `place` property

```
{
  "place_id": "ChIJmZ5emqJYwokRuDz79o0coAQ",
  "formatted_address": "1071 5th Ave, New York, NY 10128, USA",
  "search": "Guggenheim Museum, 5th Avenue, New York, NY, United States",
  "latLng": {
    "lat": 40.7829796,
    "lng": -73.95897059999999
  },
  "basic": {
    "name": "Solomon R. Guggenheim Museum",
    "address": "1071 5th Avenue",
    "city": "New York",
    "state": "New York",
    "stateCode": "NY",
    "postalCode": "10128",
    "country": "United States",
    "countryCode": "US",
    "phone": "(212) 423-3500"
  },
  "placeDetails": {
    "address_components": [
      {
        "long_name": "1071",
        "short_name": "1071",
        "types": [
          "street_number"
        ]
      },
      {
        "long_name": "5th Avenue",
        "short_name": "5th Ave",
        "types": [
          "route"
        ]
      },
      {
        "long_name": "Upper East Side",
        "short_name": "UES",
        "types": [
          "neighborhood",
          "political"
        ]
      },
      {
        "long_name": "Manhattan",
        "short_name": "Manhattan",
        "types": [
          "sublocality_level_1",
          "sublocality",
          "political"
        ]
      },
      {
        "long_name": "New York",
        "short_name": "New York",
        "types": [
          "locality",
          "political"
        ]
      },
      {
        "long_name": "New York County",
        "short_name": "New York County",
        "types": [
          "administrative_area_level_2",
          "political"
        ]
      },
      {
        "long_name": "New York",
        "short_name": "NY",
        "types": [
          "administrative_area_level_1",
          "political"
        ]
      },
      {
        "long_name": "United States",
        "short_name": "US",
        "types": [
          "country",
          "political"
        ]
      },
      {
        "long_name": "10128",
        "short_name": "10128",
        "types": [
          "postal_code"
        ]
      }
    ],
    "icon": "https://maps.gstatic.com/mapfiles/place_api/icons/museum-71.png",
    "international_phone_number": "+1 212-423-3500",
    "permanently_closed": false,
    "types": [
      "museum",
      "point_of_interest",
      "establishment"
    ],
    "website": "http://www.guggenheim.org/new-york",
    "url": "https://maps.google.com/?cid=333297768485043384",
    "utc_offset": -240
  }
}
```
