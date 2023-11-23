# SOAP Message Structure

* Overview
* SOAP Security Header
* Credential Requirements
* Error Handling
* SOAP Faults

#### Overview <a href="#soapmessagestructure-overview" id="soapmessagestructure-overview"></a>

All messages exchanged with SMX are SOAP messages. They include a SOAP Security header for authentication purposes and contain the SOAP Body contains the OTA message. The following example is a complete SOAP message with the SOAP Security header.

```
<soap-env:Envelope
	xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
	<soap-env:Header
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
		<wsse:Security
			xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
			xmlns:wsse="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-wssecurity-secext-1.0.xsd" soap:mustunderstand="1">
			<wsse:UsernameToken>
				<wsse:Username>username</wsse:Username>
				<wsse:Password type="http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#passwordtext">secret</wsse:Password>
			</wsse:UsernameToken>
		</wsse:Security>
	</soap-env:Header>
	<soap-env:Body
		xmlns:soap-env="http://schemas.xmlsoap.org/soap/envelope/">
		<OTA_HotelResNotifRQ
			xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" EchoToken="4528545b-f875-5c77-9205-22631b68f15a" ResStatus="Commit" TimeStamp="2018-07-31T01:16:16Z">
            ...
		</OTA_HotelResNotifRQ>
	</soap-env:Body>
</soap-env:Envelope>
```

***

#### SOAP Security Header <a href="#soapmessagestructure-soapsecurityheader" id="soapmessagestructure-soapsecurityheader"></a>

The Security Header structure conveys authentication information. It is mandatory and both the `/wsse:UsernameToken/wsse:Username` and `/wsse:UsernameToken/wsse:Password` elements are mandatory. The only acceptable value for the Password/@Type attribute is `http://docs.oasis-open.org/wss/2004/01/oasis-200401-wss-username-token-profile-1.0#PasswordText`, indicating a plain text password. Plain text password are acceptable as all communication is done over encrypted `HTTPS`.

***

#### Credential Requirements <a href="#soapmessagestructure-credentialrequirements" id="soapmessagestructure-credentialrequirements"></a>

Partners will need to provide SMX with a single username and password to be used authentication. These details **must** be global for all hotels using the connection, not for each individual hotel.

***

#### Error Handling <a href="#soapmessagestructure-errorhandling" id="soapmessagestructure-errorhandling"></a>

It is expected that your application has a robust error handling process in place. Please refer to the [Error Handling](https://siteminder.atlassian.net/wiki/spaces/SMXAPPS/pages/1383596141/Error+Handling) section of the Reservation API documentation for more information.

***

#### SOAP Faults <a href="#soapmessagestructure-soapfaults" id="soapmessagestructure-soapfaults"></a>

Generally OTA messages transmit "business logic" failures in the `<Errors>` element structure. However a SOAP fault can be returned in case of an unexpected error caused by for example a SOAP message where the `xml` cannot be parsed. The SOAP Fault will identify the party at fault (CLIENT/SERVER).

```
<SOAP-ENV:Envelope
	xmlns:SOAP-ENV="http://schemas.xmlsoap.org/soap/envelope/">
	<SOAP-ENV:Header/>
	<SOAP-ENV:Body>
		<SOAP-ENV:Fault>
			<faultcode>SOAP-ENV:Client</faultcode>
			<faultstring xml:lang="en">Authentication failed - Invalid username</faultstring>
		</SOAP-ENV:Fault>
	</SOAP-ENV:Body>
</SOAP-ENV:Envelope>
```
