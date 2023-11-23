# Minimum Content Sample

* Minimum Content XML
* Minimum Content XML - Reservation Cancellation

#### Minimum Content XML <a href="#minimumcontentsample-minimumcontentxml" id="minimumcontentsample-minimumcontentxml"></a>

The minimum content XML sample is for reference purposes only and it is an example of the minimum amount of data that your system could receive from SMX.

| <pre><code>&#x3C;OTA_HotelResNotifRQ xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" EchoToken="abc-123" TimeStamp="2018-05-04T19:40:04Z">
    &#x3C;HotelReservations>
        &#x3C;HotelReservation ResStatus="Reserved" CreateDateTime="2018-05-04T19:32:04Z">
            &#x3C;POS>
                &#x3C;Source>
                    &#x3C;RequestorID ID="PMSPUBLISHER"/>
                &#x3C;/Source>
            &#x3C;/POS>
            &#x3C;UniqueID ID="123456789"/>
            &#x3C;RoomStays>
                &#x3C;RoomStay>
                    &#x3C;TimeSpan Start="2017-09-05" End="2017-09-06"/>
                &#x3C;/RoomStay>
            &#x3C;/RoomStays>
            &#x3C;ResGlobalInfo>
                &#x3C;TimeSpan Start="2017-09-05" End="2017-09-06"/>
                &#x3C;Total AmountAfterTax="200.00"/>
                &#x3C;!-- May be AmountBeforeTax -->
                &#x3C;BasicPropertyInfo HotelCode="10107"/>
            &#x3C;/ResGlobalInfo>
        &#x3C;/HotelReservation>
    &#x3C;/HotelReservations>
&#x3C;/OTA_HotelResNotifRQ>
</code></pre> |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |

***

#### Minimum Content XML - Reservation Cancellation <a href="#minimumcontentsample-minimumcontentxml-reservationcancellation" id="minimumcontentsample-minimumcontentxml-reservationcancellation"></a>

In scenarios where the original reservation message was not processed by the reservation publisher, it is possible to receive the following as an "initial cancellation" message.

| <pre><code>&#x3C;OTA_HotelResNotifRQ xmlns="http://www.opentravel.org/OTA/2003/05" Version="1" EchoToken="abc-123" TimeStamp="2018-09-20T07:55:07Z">
    &#x3C;HotelReservations>
        &#x3C;HotelReservation ResStatus="Cancelled" CreateDateTime="2018-05-04T19:32:04Z" LastModifyDateTime="2018-09-20T07:55:04Z">
            &#x3C;POS>
                &#x3C;Source>
                    &#x3C;RequestorID ID="PMSPUBLISHER"/>
                &#x3C;/Source>
            &#x3C;/POS>
            &#x3C;UniqueID ID="123456789"/>
            &#x3C;ResGlobalInfo>
                 &#x3C;BasicPropertyInfo HotelCode="10107"/>
            &#x3C;/ResGlobalInfo>
        &#x3C;/HotelReservation>
    &#x3C;/HotelReservations>
&#x3C;/OTA_HotelResNotifRQ>
</code></pre> |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
