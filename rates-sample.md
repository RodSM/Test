# Rates Sample

#### Rates by Rate Plan Code <a href="#ratessample-ratesbyrateplancode" id="ratessample-ratesbyrateplancode"></a>

**Method:** GET\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/rates?startDate={yyyy-MM-dd}` or\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/rates?startDate={yyyy-MM-dd}&range={NumberOfDays}`\
**Description:** Fetch the rates for a rate plan code based on given publisher, hotel and date range.\
\
**Sample Response**

{% code fullWidth="true" %}
```json
[
  {
    "date": "2018-04-12",
    "roomTypeCode": "EKC",
    "currencyCode": "USD",
    "status": "open",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 800,
        "amountAfterTax": 850
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 950,
        "amountAfterTax": 1000
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-12",
    "roomTypeCode": "ETC",
    "currencyCode": "USD",
    "status": "close",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 900,
        "amountAfterTax": 990
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 1050,
        "amountAfterTax": 1150
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-12",
    "roomTypeCode": "PRES",
    "currencyCode": "USD",
    "status": "open",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 950,
        "amountAfterTax": 1050
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 1100,
        "amountAfterTax": 1200
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-12",
    "roomTypeCode": "SKW",
    "currencyCode": "USD",
    "status": "close",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 675,
        "amountAfterTax": 690
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 825,
        "amountAfterTax": 900
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-11",
    "roomTypeCode": "EKC",
    "currencyCode": "USD",
    "status": "open",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 800,
        "amountAfterTax": 850
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 950,
        "amountAfterTax": 1000
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-11",
    "roomTypeCode": "ETC",
    "currencyCode": "USD",
    "status": "close",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 900,
        "amountAfterTax": 990
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 1050,
        "amountAfterTax": 1150
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-11",
    "roomTypeCode": "PRES",
    "currencyCode": "USD",
    "status": "open",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 950,
        "amountAfterTax": 1050
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 1100,
        "amountAfterTax": 1200
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  },
  {
    "date": "2018-04-11",
    "roomTypeCode": "SKW",
    "currencyCode": "USD",
    "status": "close",
    "minLOS": 1,
    "maxLOS": 5,
    "baseGuestAmount": [
      {
        "ageQualifier": "adult",
        "guestCount": 1,
        "amountBeforeTax": 675,
        "amountAfterTax": 690
      },
      {
        "ageQualifier": "adult",
        "guestCount": 2,
        "amountBeforeTax": 825,
        "amountAfterTax": 900
      },
      {
        "ageQualifier": "child",
        "guestCount": 1,
        "amountBeforeTax": 200,
        "amountAfterTax": 220
      },
      {
        "ageQualifier": "child",
        "guestCount": 2,
        "amountBeforeTax": 250,
        "amountAfterTax": 275
      }
    ],
    "additionalGuestAmounts": [
      {
        "ageQualifier": "adult",
        "amount": 150
      },
      {
        "ageQualifier": "child",
        "amount": 50
      }
    ]
  }
]
```
{% endcode %}
