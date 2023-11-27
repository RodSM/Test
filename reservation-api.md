# Reservation API

* Introduction
* Communications
* Supported Functions
* OTA
* Endpoint Requirements
* Security
* SSL/TLS
* Content-Type
* Response Time
* Reservations Historical Data
* Process Flow

**Intended Audience**

This document is intended for developers and assumes the reader has working knowledge of `XML` and `SOAP`.

#### Introduction <a href="#reservationapi-introduction" id="reservationapi-introduction"></a>

SiteMinder will push reservations to SiteMinder Exchange (SMX) Partner Applications based on the partner's subscription set-up. New reservations, reservation modifications and cancellations will be sent to partner applications using an `OTA_HotelResNotifRQ`.

The request will be sent as a SOAP message as per the SMX SOAP Envelope sample provided [here](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383366749).

***

#### Communications <a href="#reservationapi-communications" id="reservationapi-communications"></a>

Communications between both systems is via the exchange of SOAP messages over secure HTTP (`HTTPS`). Operations are synchronous request/response pairs. A message is considered to be atomic and is either processed entirely or not at all by the Web Service.

***

#### Supported Functions <a href="#reservationapi-supportedfunctions" id="reservationapi-supportedfunctions"></a>

`OTA_HotelResNotifRQ` - Used to PUSH reservation notifications to the SMX Partner Application.

`OTA_HotelResNotifRS` - Returned by the SMX Partner Application to confirm receipt or failure to process the reservation message.

***

#### OTA <a href="#reservationapi-ota" id="reservationapi-ota"></a>

The SMX For Applications Reservation API is based on the Open Travel Alliance (OTA) specifications for 2017A. Although this document attempts to be technically comprehensive it is expected that the connecting system’s developers be somewhat familiar with the OTA specifications found [here](http://www.opentravel.org).

***

#### Endpoint Requirements <a href="#reservationapi-endpointrequirements" id="reservationapi-endpointrequirements"></a>

Partners will need to provide SMX with a single web service endpoint to be used for message delivery. This endpoint **must** be global for all hotels using the connection, not for each individual hotel.

The endpoint must also accept incoming SMX requests with header 'Accept' with value `application/xml`.

***

#### Security <a href="#reservationapi-security" id="reservationapi-security"></a>

Encryption is provided by the transport layer via HTTPS. Each message contains a WS-Security (WSSE) UsernameToken SOAP header for authentication/authorization purposes. Each connecting SMX Partner Application will need to provide a webservice endpoint to receive the reservation notifications.

***

#### SSL/TLS <a href="#reservationapi-ssl-tls" id="reservationapi-ssl-tls"></a>

SMX supports TLSv1.2 and above.

SiteMinder does not support self-signed SSL certificates.

***

#### Content-Type <a href="#reservationapi-content-type" id="reservationapi-content-type"></a>

The ‘Content-Type’ for all `SOAP` XML messages must be `application/xml; charset=utf-8`.

***

#### Response Time <a href="#reservationapi-responsetime" id="reservationapi-responsetime"></a>

Response time should not exceed 1000ms.

***

#### Reservations Historical Data <a href="#reservationapi-reservationshistoricaldata" id="reservationapi-reservationshistoricaldata"></a>

SiteMinder Exchange is able to send a flush of historical reservations data for a selected time period: 3 months, 6 months, 1 year etc. The time period is **only** based on the creation date (booked-on date) of the reservation so the flush might include future reservations that were created (booked) in the selected time frame. All ResStatus values are expected to be sent in the flush.

***

#### Process Flow <a href="#reservationapi-processflow" id="reservationapi-processflow"></a>

When a reservation is created, modified or cancelled in the partner PMS application (Reservation Uploader/Data Publisher) and is pushed to SiteMinder’s SMX platform, SiteMinder will generate a notification for each reservation event and PUSH reservation notifications to subscribing SMX partner applications. Partner applications will need to provide a webservice endpoint to receive the reservation notifications. The subscribing SMX partner applications can then use these reservations to offer value added solutions for the hospitality and travel industry.

Scenarios for Reservation delivery to subscribing SMX partner applications:

* If the `OTA_HotelResNotifRQ` message is delivered successfully by SiteMinder to the SMX partner application, the partner application's web service endpoint will need to respond with an `OTA_HotelResNotifRS` success message.
* If the `OTA_HotelResNotifRQ` message delivery flags an error in the SMX partner application, the partner application's web service endpoint will need to respond with an `OTA_HotelResNotifRS` error message, which should include an error string. The reservation will be retained in SMX's retry cycle and resent once the error is resolved. The message resend process may need to be done manually upon expiry of retry cycle time period.
* If the `OTA_HotelResNotifRQ` message is unable to be delivered to SMX partner application due to a network outage or similar connectivity issues, the reservation will be retained in SMX's retry cycle and resent once the error is resolved. The message resend process may need to be done manually upon expiry of retry cycle time period.

The SMX Partner Application should be able to accept all ResStatus values and respond with Success (200 OK status).

* Reserved
* Waitlisted
* Cancelled
* No-show
* In-house
* Checked-Out
* Redacted
