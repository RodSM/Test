# Availability Samples

* Availability by Room Type Code
* Availability by Rate Plan Code

#### Availability by Room Type Code <a href="#availabilitysamples-availabilitybyroomtypecode" id="availabilitysamples-availabilitybyroomtypecode"></a>

**Method:** GET\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/roomTypes/{roomTypeCode}/availability?startDate={yyyy-MM-dd}` or\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/roomTypes/{roomTypeCode}/availability?startDate={yyyy-MM-dd}&range={NumberOfDays}`\
**Description:** Get all availability for a publisher, hotel, room type and date range.\
\
**Sample Response**

```
[
  {
    "hotelCode": "sample",
    "bookingLimit": 3,
    "date": "2018-04-13",
    "ratePlanCode": "BAR",
    "roomTypeCode": "PRES",
    "minLOS": 1,
    "maxLOS": 5,
    "restriction": "Departure",
    "status": "Close"
  },
  {
    "hotelCode": "sample",
    "bookingLimit": 3,
    "date": "2018-04-12",
    "ratePlanCode": "BAR",
    "roomTypeCode": "PRES",
    "minLOS": 1,
    "maxLOS": 5,
    "restriction": "Departure",
    "status": "Close"
  },
  {
    "hotelCode": "sample",
    "bookingLimit": 3,
    "date": "2018-04-11",
    "ratePlanCode": "BAR",
    "roomTypeCode": "PRES",
    "minLOS": 1,
    "maxLOS": 5,
    "restriction": "Departure",
    "status": "Close"
  }
]
```

***

#### Availability by Rate Plan Code <a href="#availabilitysamples-availabilitybyrateplancode" id="availabilitysamples-availabilitybyrateplancode"></a>

**Method**: GET\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/availability?startDate={yyyy-MM-dd}` or\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/availability?startDate={yyyy-MM-dd}&range={NumberOfDays}`\
**Description:** Fetch the availability for a given publisher, hotel, rate plan and date range.

**Sample Response**

```
[
  {
    "hotelCode": "sample",
    "bookingLimit": 20,
    "date": "2018-04-13",
    "ratePlanCode": "CORP1",
    "roomTypeCode": "EKC",
    "minLOS": 1,
    "maxLOS": 14,
    "restriction": "Master",
    "status": "Open"
  },
  {
    "hotelCode": "sample",
    "bookingLimit": 20,
    "date": "2018-04-12",
    "ratePlanCode": "CORP1",
    "roomTypeCode": "EKC",
    "minLOS": 1,
    "maxLOS": 14,
    "restriction": "Master",
    "status": "Open"
  },
  {
    "hotelCode": "sample",
    "bookingLimit": 20,
    "date": "2018-04-11",
    "ratePlanCode": "CORP1",
    "roomTypeCode": "EKC",
    "minLOS": 1,
    "maxLOS": 14,
    "restriction": "Master",
    "status": "Open"
  }
]
```
