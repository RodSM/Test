# RoomTypes

* RoomType by Hotel
* RoomType by Room Type Code

#### RoomType by Hotel <a href="#roomtypes-roomtypebyhotel" id="roomtypes-roomtypebyhotel"></a>

**Method:** GET\
**Path:** `/publisher​s/{publisherCode}​/hotel​s/{hotelCode}​/roomTypes`\
**Description:** Lists all the room types for a specific publisher and hotel.\
\
**Parameters**

| Name          | Located in | Description                                                                                                                                                                                                        | Required | Type   |
| ------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------- | ------ |
| publisherCode | path       | The unique identifier for the data publisher. Please refer to [PMS RequestorID/publisherCode](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1508714248/SMX+PMSs+Reservations+Capabilities+Table) list | Yes      | string |
| hotelCode     | path       | The code that uniquely identifies a single hotel property.                                                                                                                                                         | Yes      | string |

**Responses**

| Code | Description           | Schema                                                                                            |
| ---- | --------------------- | ------------------------------------------------------------------------------------------------- |
| 200  | OK                    | [RoomType](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#RoomType) |
| 401  | Unauthorized          | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 403  | Forbidden             | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 405  | Method Not Supported  | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 429  | Too Many Requests     | TooManyRequests                                                                                   |
| 500  | Internal Server Error | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |

***

#### RoomType by Room Type Code <a href="#roomtypes-roomtypebyroomtypecode" id="roomtypes-roomtypebyroomtypecode"></a>

**Method:** GET\
**Path:** `​/publisher​s/{publisherCode}​/hotel​s/{hotelCode}​/roomTypes​/{roomTypeCode}`\
**Description:** Get a specific room type for a specific publisher and hotel.\
\
**Parameters**

| Name          | Located in | Description                                                                                                                                                                                             | Required | Type   |
| ------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------- | ------ |
| publisherCode | path       | The unique identifier for the data publisher. Please refer to [PMS RequestorID/publisherCode](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383432813/PMS+RequestorID+publisherCode) list | Yes      | string |
| hotelCode     | path       | The code that uniquely identifies a single hotel property.                                                                                                                                              | Yes      | string |
| roomTypeCode  | path       | The code that identifies a Room Type.                                                                                                                                                                   | Yes      | string |

**Responses**

| Code | Description           | Schema                                                                                            |
| ---- | --------------------- | ------------------------------------------------------------------------------------------------- |
| 200  | OK                    | [RoomType](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#RoomType) |
| 401  | Unauthorized          | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 403  | Forbidden             | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 405  | Method Not Supported  | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |
| 429  | Too Many Requests     | TooManyRequests                                                                                   |
| 500  | Internal Server Error | [Error](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383212147/Models#Error)       |

***

Response JSON Samples: RoomTypes Samples
