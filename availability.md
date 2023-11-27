# Availability

* Availability by Room Type Code
* Availability by Rate Plan Code

#### Availability by Room Type Code <a href="#availability-availabilitybyroomtypecode" id="availability-availabilitybyroomtypecode"></a>

**Method:** GET\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/roomTypes/{roomTypeCode}/availability?startDate={yyyy-MM-dd}` or\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/roomTypes/{roomTypeCode}/availability?startDate={yyyy-MM-dd}&range={NumberOfDays}`\
**Description:** Get all availability for a publisher, hotel, room type and date range.\
\
**Parameters**

| Name          | Located in | Description                                                                                                                                                                                             | Required | Type   |
| ------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ------ |
| publisherCode | path       | The unique identifier for the data publisher. Please refer to [PMS RequestorID/publisherCode](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383432813/PMS+RequestorID+publisherCode) list | Yes      | string |
| hotelCode     | path       | The code that uniquely identifies a single hotel property.                                                                                                                                              | Yes      | string |
| roomTypeCode  | path       | The code that identifies a Room Type.                                                                                                                                                                   | Yes      | string |
| startDate     | query      | Start date to query for availability. Format like `yyyy-MM-dd` i.e `2017-07-21`.                                                                                                                        | Yes      | date   |
| range         | query      | The number of days to query for. Maximum `30`.                                                                                                                                                          | No       | number |

**Responses**

| Code | Description           | Schema                                                                                                    |
| ---- | --------------------- | --------------------------------------------------------------------------------------------------------- |
| 200  | OK                    | [Availability](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Availability) |
| 401  | Unauthorized          | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 403  | Forbidden             | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 405  | Method Not Supported  | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 429  | Too Many Requests     | TooManyRequests                                                                                           |
| 500  | Internal Server Error | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |

***

#### Availability by Rate Plan Code <a href="#availability-availabilitybyrateplancode" id="availability-availabilitybyrateplancode"></a>

**Method:** GET\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/availability?startDate={yyyy-MM-dd}` or\
**Path:** `/publishers/{publisherCode}/hotels/{hotelCode}/ratePlans/{ratePlanCode}/availability?startDate={yyyy-MM-dd}&range={NumberOfDays}`\
**Description:** Fetch the availability for a given publisher, hotel, rate plan and date range.\
\
**Parameters**

| Name          | Located in | Description                                                                                                                                                                                             | Required | Type   |
| ------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ------ |
| publisherCode | path       | The unique identifier for the data publisher. Please refer to [PMS RequestorID/publisherCode](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383432813/PMS+RequestorID+publisherCode) list | Yes      | string |
| hotelCode     | path       | The code that uniquely identifies a single hotel property.                                                                                                                                              | Yes      | string |
| ratePlanCode  | path       | The rate plan code.                                                                                                                                                                                     | Yes      | string |
| startDate     | query      | Start date to query for rates. Format like `yyyy-MM-dd` i.e `2017-07-21`.                                                                                                                               | Yes      | date   |
| range         | query      | The number of days to query for. Maximum `30`.                                                                                                                                                          | No       | number |

**Responses**

| Code | Description           | Schema                                                                                                    |
| ---- | --------------------- | --------------------------------------------------------------------------------------------------------- |
| 200  | OK                    | [Availability](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Availability) |
| 401  | Unauthorized          | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 403  | Forbidden             | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 405  | Method Not Supported  | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |
| 429  | Too Many Requests     | TooManyRequests                                                                                           |
| 500  | Internal Server Error | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)               |

***

Response JSON Samples: [Availability Samples](broken-reference)
