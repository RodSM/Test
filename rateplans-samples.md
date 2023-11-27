# RatePlans Samples

* RatePlans by Hotel
* RatePlans by Rate Plan Code

#### RatePlans by Hotel <a href="#rateplanssamples-rateplansbyhotel" id="rateplanssamples-rateplansbyhotel"></a>

**Method:** GET\
**Path:** `​/publisher​s/{publisherCode}​/hotel​s/{hotelCode}​/ratePlans`\
**Description:** Lists all the rate plans for a specific publisher and hotel.\
\
**Sample Response**

```
[
  {
    "code": "BAR",
    "hotelCode": "sample",
    "category": "rack",
    "yieldable": false,
    "marketCode": "rack-market-code",
    "confidential": false,
    "start": "2018-06-04",
    "end": "2019-12-31",
    "commissionable": true,
    "names": [
      {
        "lang": "EN",
        "name": "BAR"
      }
    ],
    "descriptions": [
      {
        "lang": "EN",
        "description": "Best Available Rate"
      }
    ],
    "commission": {
      "percentage": null,
      "amount": 100
    },
    "minimumAdvancedBookingOffset": 0,
    "maximumAdvancedBookingOffset": 3,
    "minLOS": 1,
    "maxLOS": 5,
    "arrivalWeekDays": [
      "mon",
      "sat",
      "sun"
    ],
    "availableWeekDays": [
      "tue",
      "wed",
      "thur"
    ],
    "lastModifiedAt": "2019-03-05T05:21:21.553Z",
    "createdAt": "2019-03-05T05:21:11.253Z"
  },
  {
    "code": "CORP1",
    "hotelCode": "sample",
    "category": "rack",
    "yieldable": true,
    "marketCode": "rack-market-code",
    "confidential": true,
    "start": "2018-07-05",
    "end": "2019-11-30",
    "commissionable": true,
    "names": [
      {
        "lang": "EN",
        "name": "CR1"
      }
    ],
    "descriptions": [
      {
        "lang": "EN",
        "description": "Corporate Rate 1"
      }
    ],
    "commission": null,
    "minimumAdvancedBookingOffset": 1,
    "maximumAdvancedBookingOffset": 7,
    "minLOS": 1,
    "maxLOS": 14,
    "arrivalWeekDays": [
      "mon",
      "tue",
      "wed",
      "thur",
      "fri",
      "sat",
      "sun"
    ],
    "availableWeekDays": [
      "mon",
      "tue",
      "wed",
      "thur",
      "fri"
    ],
    "lastModifiedAt": "2019-03-05T05:21:21.746Z",
    "createdAt": "2019-03-05T05:21:21.653Z"
  },
  {
    "code": "CORP2",
    "hotelCode": "sample",
    "category": "rack",
    "yieldable": true,
    "marketCode": "rack-market-code",
    "confidential": true,
    "start": "2018-07-05",
    "end": "2019-11-30",
    "commissionable": true,
    "names": [
      {
        "lang": "EN",
        "name": "CR2"
      }
    ],
    "descriptions": [
      {
        "lang": "EN",
        "description": "Corporate Rate 2"
      }
    ],
    "commission": null,
    "minimumAdvancedBookingOffset": 1,
    "maximumAdvancedBookingOffset": 7,
    "minLOS": 1,
    "maxLOS": 14,
    "arrivalWeekDays": [
      "mon",
      "tue",
      "wed",
      "thur",
      "fri",
      "sat",
      "sun"
    ],
    "availableWeekDays": [
      "mon",
      "tue",
      "wed",
      "thur",
      "fri"
    ],
    "lastModifiedAt": "2019-03-05T05:21:22.134Z",
    "createdAt": "2019-03-05T05:21:22.041Z"
  },
  {
    "code": "NEG",
    "hotelCode": "sample",
    "category": "rack",
    "yieldable": true,
    "marketCode": "rack-market-code",
    "confidential": true,
    "start": "2018-07-05",
    "end": "2019-12-31",
    "commissionable": true,
    "names": [
      {
        "lang": "EN",
        "name": "NR"
      }
    ],
    "descriptions": [
      {
        "lang": "EN",
        "description": "Negotiated Rate"
      }
    ],
    "commission": null,
    "minimumAdvancedBookingOffset": 1,
    "maximumAdvancedBookingOffset": 7,
    "minLOS": 1,
    "maxLOS": 21,
    "arrivalWeekDays": [
      "mon",
      "tue",
      "wed",
      "thur"
    ],
    "availableWeekDays": [
      "fri",
      "sat",
      "sun"
    ],
    "lastModifiedAt": "2019-03-05T05:21:21.941Z",
    "createdAt": "2019-03-05T05:21:21.846Z"
  }
]
```

***

#### RatePlans by Rate Plan Code <a href="#rateplanssamples-rateplansbyrateplancode" id="rateplanssamples-rateplansbyrateplancode"></a>

**Method:** GET\
**Path:** `​/publisher​s/{publisherCode}​/hotel​s/{hotelCode}​/ratePlans​/{ratePlanCode}`\
**Description:** Get a specific rate plan for a publisher and hotel.\
\
**Sample Response**

```
{
  "code": "CORP1",
  "hotelCode": "sample",
  "category": "rack",
  "yieldable": true,
  "marketCode": "rack-market-code",
  "confidential": true,
  "start": "2018-07-05",
  "end": "2019-11-30",
  "commissionable": true,
  "names": [
    {
      "lang": "EN",
      "name": "CR1"
    }
  ],
  "descriptions": [
    {
      "lang": "EN",
      "description": "Corporate Rate 1"
    }
  ],
  "commission": null,
  "minimumAdvancedBookingOffset": 1,
  "maximumAdvancedBookingOffset": 7,
  "minLOS": 1,
  "maxLOS": 14,
  "arrivalWeekDays": [
    "mon",
    "tue",
    "wed",
    "thur",
    "fri",
    "sat",
    "sun"
  ],
  "availableWeekDays": [
    "mon",
    "tue",
    "wed",
    "thur",
    "fri"
  ],
  "lastModifiedAt": "2019-03-05T05:21:21.746Z",
  "createdAt": "2019-03-05T05:21:21.653Z"
}
```
