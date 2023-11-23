# OTA\_HotelResNotifRS

/\*\*/

* Response Specification
* Response Time
* Content-Type
* Response Samples
  * Success
  * Success and Warning
  * Failure

#### Response Specification <a href="#ota_hotelresnotifrs-responsespecification" id="ota_hotelresnotifrs-responsespecification"></a>

This message will be returned by partner application (Subscriber) in response to the `OTA_HotelResNotifRQ` message sent by SMX. The message will confirms whether the `OTA_HotelResNotifRQ` message was processed successfully by the partner application or not.

#### Response Time <a href="#ota_hotelresnotifrs-responsetime" id="ota_hotelresnotifrs-responsetime"></a>

Response time should not exceed 1000ms.

#### Content-Type <a href="#ota_hotelresnotifrs-content-type" id="ota_hotelresnotifrs-content-type"></a>

The ‘Content-Type’ for all `SOAP` XML messages must be `application/xml; charset=utf-8`.\


Elements and attributes marked with Number=1 or more will always be sent. 0 means that the element or attribute is optional, while a second numeric value or 'n' indicates the element or attribute can repeat (where n = no limit)"

| **Element**                                                                                                            | **Attribute**    | **Number** | **Description**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OTA\_HotelResNotifRS                                                                                                   |                  | 1          | <p><strong>Mandatory</strong><br>Root element of the message.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|                                                                                                                        | @EchoToken       | 1          | As per OpenTravel Alliance Specifications.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|                                                                                                                        | @Version         | 1          | Version is a mandatory attribute in OTA; therefore, it must remain Mandatory in HTNG in order to be able to use the same message.                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|                                                                                                                        | @TimeStamp       | 1          | ISO 8601 encoded timestamp indicating the creation date and time of the message. Format like `yyyy-MM-dd'T'HH:mm:ssZZ` i.e `2012-03-09T20:05:52+08:00`                                                                                                                                                                                                                                                                                                                                                                                                                          |
|                                                                                                                        | @ResResponseType | 0..1       | <p>Given that the OTA_HotelResNotifRQ message is used for additions, modifications and cancellations, this attribute is used to replicate whether the original message was an addition, a modification or a cancellation and does not refer to the status of the transaction itself but rather to the nature of the original message. The only three enumerations allowed will therefore be:</p><ul><li>Committed</li><li>Modified</li><li>Cancelled</li></ul>                                                                                                                  |
| OTA\_HotelResNotifRS / Errors / Error                                                                                  |                  | 1..99      | Mandatory ONLY if Success element is not sent. Only needed if RQ message was unsuccessful. More information can be found [here](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling#Recommended-OTA-Error-Codes).                                                                                                                                                                                                                                                                                                                              |
|                                                                                                                        | @Type            | 1          | Mandatory in OTA. Refers to OpenTravel Alliance [EWT](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling#Error-Warning-Type-\(EWT\)) list (Error Warning Type).                                                                                                                                                                                                                                                                                                                                                                               |
|                                                                                                                        | @Code            | 0..1       | Refers to OpenTravel Alliance [ERR](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling#Error-Codes-\(ERR\)) list (Error Codes). Should be used wherever possible.                                                                                                                                                                                                                                                                                                                                                                             |
|                                                                                                                        | @RecordID        | 0..1       | If the receiving system is able to identify within a batch of reservations which reservation failed, the uniqueID of the rejected reservation should be reported here.                                                                                                                                                                                                                                                                                                                                                                                                          |
| OTA\_HotelResNotifRS / Success                                                                                         |                  | 1          | Mandatory if no Errors were sent. This is the annotation that the reservation batch was received successfully. It could be combined with warning messages if some of the reservations in the batch had issues.                                                                                                                                                                                                                                                                                                                                                                  |
| OTA\_HotelResNotifRS / Warnings / Warning                                                                              |                  | 0..99      | Can be used in conjunction with Success message.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|                                                                                                                        | @Type            | 1          | Refers to OpenTravel Alliance [EWT](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling#Error-Warning-Type-\(EWT\)) list (Error Warning Type).                                                                                                                                                                                                                                                                                                                                                                                                 |
|                                                                                                                        | @Code            | 0..1       | Refers to OpenTravel Alliance [ERR](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling#Error-Codes-\(ERR\)) list (Error Codes). Should be used wherever possible.                                                                                                                                                                                                                                                                                                                                                                             |
|                                                                                                                        | @RecordID        | 0..1       | If the receiving system is able to identify within a batch of reservations which reservation has a warning, the uniqueID of that reservation should be reported here.                                                                                                                                                                                                                                                                                                                                                                                                           |
| OTA\_HotelResNotifRS / HotelReservations / HotelReservation                                                            |                  | 1          | <p><strong>Mandatory</strong><br>Must be sent for the message to have a meaning.<br>Mandatory only if 'Success' element is sent.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|                                                                                                                        | @ResStatus       | 0..1       | <p>Indicates the current status of the reservation.<br>Valid values are dependant on the roles:</p><ul><li>Reserved</li><li>Waitlisted</li><li>In-house</li><li>Checked-Out</li></ul>                                                                                                                                                                                                                                                                                                                                                                                           |
| OTA\_HotelResNotifRS / HotelReservations / HotelReservation / UniqueID                                                 |                  | 1          | <p><strong>Mandatory</strong><br>This is the confirmation number for the reservation assigned by the immediate originator of the booking (i.e., the system that sent the OTA_HotelResNotifRQ message for which the OTA_HotelresNotifRS message is sent).</p>                                                                                                                                                                                                                                                                                                                    |
|                                                                                                                        | @Type            | 0..1       | <p>Type is assigned values from the <a href="https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383301614/OTA+Code+List#Unique-ID-Type-(UIT)">UIT</a> code list. If the original system was a CRS:<br>Type = 14 – Reservation<br>ID is the actual confirmation number<br>If it was a PMS: Type = 10 - Hotel</p>                                                                                                                                                                                                                                                        |
|                                                                                                                        | @ID              | 1          | ID is the CRS confirmation number (or PMS number if the reservation was originated in the PMS).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| OTA\_HotelResNotifRS / HotelReservations / HotelReservation / ResGlobalInfo / HotelReservationIDs / HotelReservationID |                  | 1          | <p><strong>Mandatory</strong><br>This is the confirmation number associated by the system that received the booking.</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|                                                                                                                        | @ResID\_Type     | 1          | <p>ResID_Type is assigned values from the <a href="https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383301614/OTA+Code+List#Unique-ID-Type-(UIT)">UIT</a> code list. Some common uses:<br>18 - Other<br>10 – Hotel<br>13 – Internet Broker<br>14 – Reservation Broker<br>24 – Travel Agent PNR<br>For any other type of system the implementing partners should agree on the appropriate code from the OpenTravel Alliance <a href="https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383301614/OTA+Code+List#Unique-ID-Type-(UIT)">UIT</a> code list.</p> |
|                                                                                                                        | @ResID\_Value    | 1          | ResID\_Value is the actual confirmation number.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|                                                                                                                        | @ResID\_Source   | 0..1       | A unique identifier to indicate the source system that generated the ResID\_Value.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|                                                                                                                        | @ForGuest        | 0..1       | When 1 the confirmation number given to the guest. This number should be searchable by the destination.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

***

#### Response Samples <a href="#ota_hotelresnotifrs-responsesamples" id="ota_hotelresnotifrs-responsesamples"></a>

OTA\_HotelResNotifRS must be wrapped in a Soap Envelope with Content-Type: `application/xml; charset=utf-8`.

**Success**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
		<OTA_HotelResNotifRS
			xmlns="http://www.opentravel.org/OTA/2003/05" EchoToken="cdcd51f2-769a-5a1d-841c-e6204d811f5c" TimeStamp="2019-05-08T00:56:53Z" Version="1.0">
			<Success/>
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

**Success and Warning**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
		<OTA_HotelResNotifRS
			xmlns="http://www.opentravel.org/OTA/2003/05" EchoToken="cdcd51f2-769a-5a1d-841c-e6204d811f5c" TimeStamp="2019-05-08T00:56:53Z" Version="1.0">
			<Success/>
			<Warnings>
				<Warning Type="10" Code="310">Missing last name</Warning>
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

**Failure**

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
		<OTA_HotelResNotifRS
			xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" TimeStamp="2005-08-01T09:30:47+08:00" EchoToken="cdcd51f2-769a-5a1d-841c-e6204d811f5c">
			<Errors>
				<Error Type="6" Code="375">Hotel not active</Error>
			</Errors>
		</OTA_HotelResNotifRS>
	</soap-env:Body>
</soap-env:Envelope>
```
