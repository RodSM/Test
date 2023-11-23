# Error Handling

/\*\*/

* Error Responses to SMX
  * Content-Type
  * Invalid Hotel Code
  * Invalid Username or Password
* Warning Responses to SMX
  * Content-Type
  * Required Information Not Present - Missing email address
  * Required Information Not Present - Missing phone number
* Recommended OTA Error Codes
  * Error Warning Type (EWT)
  * Error Codes (ERR)

#### Error Responses to SMX <a href="#errorhandling-errorresponsestosmx" id="errorhandling-errorresponsestosmx"></a>

**Important**\
Errors must be returned within a 'SOAP Envelope' and use the defined response message container depending on the message being responded to. Please see the relevant parts of our specification within the SMX For Applications API section for more information on the error response message. If the error is specifically related to application level errors, please do not respond any other error types (HTTP etc.). If you have server level issues, then it is OK to respond with HTTP standard error codes

It is expected that your application has a robust error handling process in place. An error response should contain a short description of the error to assist our Support teams in troubleshooting.

Error Responses using the \<Errors>\</Errors> tag will flag the reservation delivery from SMX to your endpoint as **Failed**.

**Content-Type**

The ‘Content-Type’ for all `SOAP` XML messages must be `application/xml; charset=utf-8`.

**Invalid Hotel Code**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
        <OTA_HotelResNotifRS xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" TimeStamp="2022-08-01T09:30:47+08:00" EchoToken="abc123-unique">
          <Errors>
            <Error Type="6" Code="392">Hotel not found for HotelCode=XXXXXX</Error>
          </Errors>
        </OTA_HotelResNotifRS>
    </soap-env:Body>
</soap-env:Envelope>
```

**Invalid Username or Password**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">       
       <OTA_HotelResNotifRS xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" TimeStamp="2022-08-01T09:30:47+08:00" EchoToken="abc123-unique">
          <Errors>
             <Error Type="6" Code="497">Invalid Username and/or Password</Error>
         </Errors>
       </OTA_HotelResNotifRS>
    </soap-env:Body>
</soap-env:Envelope>
```

#### Warning Responses to SMX <a href="#errorhandling-warningresponsestosmx" id="errorhandling-warningresponsestosmx"></a>

Any other warning responses that are not application or server level issues should be sent as Success + Warning to avoid reservation delivery failures. Please review [https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383759931/OTA+HotelResNotifRS#Success-and-Warning](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383759931/OTA+HotelResNotifRS#Success-and-Warning).

Our Reservations API specifications will have non-mandatory fields/attributes that a Publisher might not send in the reservation XML if its not supported by them. Publishers should always send the mandatory reservation fields. Please review our [https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383432331/OTA+HotelResNotifRQ#Request-Specification](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383432331/OTA+HotelResNotifRQ#Request-Specification) to view the mandatory and non-mandatory attributes.

**Content-Type**

The ‘Content-Type’ for all `SOAP` XML messages must be `application/xml; charset=utf-8`.

**Required Information Not Present - Missing email address**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">       
       <OTA_HotelResNotifRS xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" TimeStamp="2022-08-01T09:30:47+08:00" EchoToken="abc123-unique">
			<Success/>
			<Warnings>
				<Warning Type="10" Code="321">Guest email address is required</Warning>
			</Warnings>
			<HotelReservations>
				<HotelReservation>
					<UniqueID ID="LH123456789"/>
					<ResGlobalInfo>
						<HotelReservationIDs>
							<HotelReservationID ResID_Type="10" ResID_Value="LH123456789"/>
						</HotelReservationIDs>
					</ResGlobalInfo>
				</HotelReservation>
			</HotelReservations>          
       </OTA_HotelResNotifRS>
    </soap-env:Body>
</soap-env:Envelope>
```

**Required Information Not Present - Missing phone number**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">       
       <OTA_HotelResNotifRS xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" TimeStamp="2022-08-01T09:30:47+08:00" EchoToken="abc123-unique">
			<Success/>
			<Warnings>
				<Warning Type="10" Code="316">Phone number is required</Warning>
			</Warnings>
			<HotelReservations>
				<HotelReservation>
					<UniqueID ID="LH123456789"/>
					<ResGlobalInfo>
						<HotelReservationIDs>
							<HotelReservationID ResID_Type="10" ResID_Value="LH123456789"/>
						</HotelReservationIDs>
					</ResGlobalInfo>
				</HotelReservation>
			</HotelReservations>          
       </OTA_HotelResNotifRS>
    </soap-env:Body>
</soap-env:Envelope>
```

***

#### Recommended OTA Error Codes <a href="#errorhandling-recommendedotaerrorcodes" id="errorhandling-recommendedotaerrorcodes"></a>

SMX recommends (but is not limited to) the following error codes from OTA Warning Type (EWT). Any OTA Warning Type can be used.

**Error Warning Type (EWT)**

| Code | OTA Description        |
| ---- | ---------------------- |
| 1    | Unknown                |
| 2    | No implementation      |
| 3    | Biz rule               |
| 4    | Authentication         |
| 5    | Authentication timeout |
| 6    | Authorization          |
| 7    | Protocol violation     |
| 8    | Transaction model      |
| 9    | Authentical model      |
| 10   | Required field missing |
| 11   | Advisory               |
| 12   | Processing exception   |
| 13   | Application error      |

**Error Codes (ERR)**

**Error Codes - General**\
These are recommended (but not limited to) Error Codes to be returned for general errors. Any OTA Error Code (ERR) entry can be used.

| Code | OTA Description              | Field      |
| ---- | ---------------------------- | ---------- |
| 187  | System currently unavailable |            |
| 400  | Invalid property code        | Hotel code |
| 448  | System error                 |            |
| 450  | Unable to process            |            |
| 497  | Authorization error          |            |

**Error Codes - Updates**\
These are recommended (but not limited to) Error Codes to be returned for update errors. Any OTA Error Code (ERR) entry can be used.

| Code | OTA Description                     | Usage                                                                                                  |
| ---- | ----------------------------------- | ------------------------------------------------------------------------------------------------------ |
| 16   | Invalid date                        |                                                                                                        |
| 310  | Required data missing: last name    |                                                                                                        |
| 311  | Required data missing: first name   |                                                                                                        |
| 316  | Required data missing: phone number |                                                                                                        |
| 321  | Required field missing              | Used when a required field is missing that does not have a dedicated error code (ie: Room ID required) |
| 375  | Hotel not active                    |                                                                                                        |
| 392  | Invalid hotel code                  |                                                                                                        |
