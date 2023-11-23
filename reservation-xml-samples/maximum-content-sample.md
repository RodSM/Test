# Maximum Content Sample

The maximum content XML sample is for reference purposes only and it is an example of the maximum amount of data that your system could received from SMX.

| <pre><code>&#x3C;OTA_HotelResNotifRQ xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" EchoToken="cc3048b5-55ca-4d77-b316-cb8e769c1381" TimeStamp="2017-09-19T18:13:53+00:00">
    &#x3C;HotelReservations>
        &#x3C;HotelReservation ResStatus="Reserved" CreateDateTime="2017-09-19T18:02:44+00:00" CreatorID="LINDA-RESAGENT" LastModifyDateTime="2017-09-19T18:13:51+00:00" LastModifierID="651651651651">
            &#x3C;POS>
                &#x3C;Source>
                    &#x3C;RequestorID ID="TESTPMS"/>
                &#x3C;/Source>
                &#x3C;Source>
                    &#x3C;BookingChannel Type="4" Primary="true">
                        &#x3C;CompanyName Code="Code1">CompanyName0&#x3C;/CompanyName>
                    &#x3C;/BookingChannel>
                &#x3C;/Source>
            &#x3C;/POS>
            &#x3C;UniqueID ID="BDC-3685569477"/>
            &#x3C;RoomStays>
                &#x3C;RoomStay MarketCode="Corporate" SourceOfBusiness="Radio" PromotionCode="STAYNSAVE15">
                    &#x3C;RoomTypes>
                        &#x3C;RoomType RoomType="Deluxe" RoomTypeCode="DLX" RoomCategory="4" RoomID="1501" NonSmoking="true" Configuration="King Split + Single Bed">
                            &#x3C;RoomDescription>
                                &#x3C;Text>Deluxe Room with a lovely view over the harbour and a seperate lounge with 50" LED TV&#x3C;/Text>
                            &#x3C;/RoomDescription>
                            &#x3C;AdditionalDetails>
                                &#x3C;AdditionalDetail Type="4" Code="CORNERROOM">
                                    &#x3C;DetailDescription>
                                        &#x3C;Text>This room is a Deluxe Corner Room&#x3C;/Text>
                                    &#x3C;/DetailDescription>
                                &#x3C;/AdditionalDetail>
                            &#x3C;/AdditionalDetails>
                        &#x3C;/RoomType>
                    &#x3C;/RoomTypes>
                    &#x3C;RatePlans>
                        &#x3C;RatePlan RatePlanCode="WKGPKG" EffectiveDate="2017-12-01" ExpireDate="2017-12-03" RatePlanName="Weekend Package">
                            &#x3C;RatePlanDescription>
                                &#x3C;Text>Weekend Package includes wine, chocolates, champagne on arrival and late checkout at 3PM&#x3C;/Text>
                            &#x3C;/RatePlanDescription>
                            &#x3C;RatePlanInclusions TaxInclusive="true" ServiceFeeInclusive="false">
                                &#x3C;RatePlanInclusionDescription>
                                    &#x3C;Text>Champagne on arrival, English Breakfast, Chocolates and 3PM Checkout &#x3C;/Text>
                                &#x3C;/RatePlanInclusionDescription>
                            &#x3C;/RatePlanInclusions>
                            &#x3C;MealsIncluded MealPlanIndicator="true" MealPlanCodes="7"/>
                            &#x3C;AdditionalDetails>
                                &#x3C;AdditionalDetail Type="12" Code="WKDNDPKGINFO">
                                    &#x3C;DetailDescription>
                                        &#x3C;Text>Some parts of this package (such as wine selection) will need to be arranged with guest prior to check-in&#x3C;/Text>
                                    &#x3C;/DetailDescription>
                                &#x3C;/AdditionalDetail>
                            &#x3C;/AdditionalDetails>
                        &#x3C;/RatePlan>
                    &#x3C;/RatePlans>
                    &#x3C;RoomRates>
                        &#x3C;RoomRate InvBlockCode="HIGHROLL" NumberOfUnits="1" RoomID="1501" RoomTypeCode="DLX" RatePlanCode="WKGPKG" RatePlanCategory="Consumer Packages" EffectiveDate="2017-12-01" ExpireDate="2017-12-03">
                            &#x3C;Rates>
                                &#x3C;Rate EffectiveDate="2017-12-01" ExpireDate="2017-12-02" UnitMultiplier="1">
                                    &#x3C;Base AmountBeforeTax="100.00" AmountAfterTax="110.00" CurrencyCode="AUD">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="10.00">
                                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>GST&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/Base>
                                    &#x3C;Total AmountBeforeTax="120.00" AmountAfterTax="132.00" CurrencyCode="AUD">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="12.00">
                                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>GST&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/Total>
                                &#x3C;/Rate>
                                &#x3C;Rate EffectiveDate="2017-12-02" ExpireDate="2017-12-03" UnitMultiplier="1">
                                    &#x3C;Base AmountBeforeTax="80.00" AmountAfterTax="88.00" CurrencyCode="AUD">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="8.00">
                                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>GST&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/Base>
                                    &#x3C;Total AmountBeforeTax="100.00" AmountAfterTax="110.00" CurrencyCode="AUD">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="10.00">
                                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>GST&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/Total>
                                &#x3C;/Rate>
                            &#x3C;/Rates>
                            &#x3C;ServiceRPHs>
                                &#x3C;ServiceRPH RPH="1"/>
                            &#x3C;/ServiceRPHs>
                        &#x3C;/RoomRate>
                    &#x3C;/RoomRates>
                    &#x3C;GuestCounts>
                        &#x3C;GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
                        &#x3C;GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
                    &#x3C;/GuestCounts>
                    &#x3C;TimeSpan Start="2017-12-01" End="2017-12-03"/>
                    &#x3C;Guarantee GuaranteeCode="COMBINED_GUARANTEE" GuaranteeType="DepositRequired">
                                &#x3C;GuaranteesAccepted>
                                    &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                        &#x3C;PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
                                            &#x3C;CardHolderName>Leonard Woolf&#x3C;/CardHolderName>
                                            &#x3C;CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
                                            &#x3C;/CardNumber>
                                        &#x3C;/PaymentCard>
                                    &#x3C;/GuaranteeAccepted>
                                    &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                        &#x3C;Voucher SeriesCode="4555"/>
                                    &#x3C;/GuaranteeAccepted>
                                    &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                        &#x3C;DirectBill DirectBill_ID="4981003"/>
                                    &#x3C;/GuaranteeAccepted>
                                &#x3C;/GuaranteesAccepted>
                                &#x3C;GuaranteeDescription>
                                    &#x3C;Text>Combined Guarantees Accepted (Platinum Membership)&#x3C;/Text>
                                &#x3C;/GuaranteeDescription>
                            &#x3C;/Guarantee>
                            &#x3C;DepositPayments>
                                &#x3C;GuaranteePayment>
                                    &#x3C;AcceptedPayments>
                                        &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                            &#x3C;PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
                                                &#x3C;CardHolderName>Leonard Woolf&#x3C;/CardHolderName>
                                                &#x3C;CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
                                                &#x3C;/CardNumber>
                                            &#x3C;/PaymentCard>
                                        &#x3C;/AcceptedPayment>
                                    &#x3C;/AcceptedPayments>
                                    &#x3C;AmountPercent Percent="30" CurrencyCode="AUD" Amount="64.52" NmbrOfNights="2">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="1.29">
                                            &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="2">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>Credit Card surcharge.&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/AmountPercent>
                                    &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                    &#x3C;Description>
                                        &#x3C;Text>30% deposit (of the total cost of the stay) will be charged to card holder's account 10 days before the date of arrival at the latest.&#x3C;/Text>
                                    &#x3C;/Description>
                                    &#x3C;Address Type="1">
                                        &#x3C;AddressLine>12 Pine Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2095&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                    &#x3C;/Address>
                                &#x3C;/GuaranteePayment>
                                &#x3C;GuaranteePayment>
                                    &#x3C;AcceptedPayments>
                                        &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                            &#x3C;Voucher SeriesCode="4555"/>
                                        &#x3C;/AcceptedPayment>
                                    &#x3C;/AcceptedPayments>
                                    &#x3C;AmountPercent Percent="10" CurrencyCode="AUD" Amount="21.51" NmbrOfNights="2">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="1.08">
                                            &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>Payment surcharge.&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/AmountPercent>
                                    &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                    &#x3C;Description>
                                        &#x3C;Text>10% deposit (of the total cost of the stay) will be charged using provided Voucher code 10 days before the date of arrival at the latest.&#x3C;/Text>
                                    &#x3C;/Description>
                                    &#x3C;Address Type="1">
                                        &#x3C;AddressLine>12 Pine Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2095&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                    &#x3C;/Address>
                                &#x3C;/GuaranteePayment>
                                &#x3C;GuaranteePayment>
                                    &#x3C;AcceptedPayments>
                                        &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                            &#x3C;DirectBill DirectBill_ID="4981003"/>
                                        &#x3C;/AcceptedPayment>
                                    &#x3C;/AcceptedPayments>
                                    &#x3C;AmountPercent Percent="20" CurrencyCode="AUD" Amount="43.01" NmbrOfNights="2">
                                        &#x3C;Taxes CurrencyCode="AUD" Amount="2.15">
                                            &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
                                                &#x3C;TaxDescription>
                                                    &#x3C;Text>Payment surcharge.&#x3C;/Text>
                                                &#x3C;/TaxDescription>
                                            &#x3C;/Tax>
                                        &#x3C;/Taxes>
                                    &#x3C;/AmountPercent>
                                    &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                    &#x3C;Description>
                                        &#x3C;Text>20% deposit (of the total cost of the stay) will be charged using Direct Bill ID provided 10 days before the date of arrival at the latest.&#x3C;/Text>
                                    &#x3C;/Description>
                                    &#x3C;Address Type="2">
                                        &#x3C;AddressLine>125 Pitt Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2000&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                    &#x3C;/Address>
                                &#x3C;/GuaranteePayment>
                            &#x3C;/DepositPayments>
                    &#x3C;Discount TaxInclusive="true" Percent="15" DiscountCode="STAYNSAVE15" AmountBeforeTax="33.00" AmountAfterTax="36.30" CurrencyCode="AUD">
                        &#x3C;Taxes CurrencyCode="AUD" Amount="3.30">
                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                &#x3C;TaxDescription>
                                    &#x3C;Text>GST&#x3C;/Text>
                                &#x3C;/TaxDescription>
                            &#x3C;/Tax>
                        &#x3C;/Taxes>
                        &#x3C;DiscountReason>
                            &#x3C;Text>Stay 2 nights and get 15% off.&#x3C;/Text>
                        &#x3C;/DiscountReason>
                    &#x3C;/Discount>
                    &#x3C;Total AmountBeforeTax="187.00" AmountAfterTax="215.05" CurrencyCode="AUD">
                        &#x3C;Taxes CurrencyCode="AUD" Amount="28.05">
                            &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                &#x3C;TaxDescription>
                                    &#x3C;Text>GST&#x3C;/Text>
                                &#x3C;/TaxDescription>
                            &#x3C;/Tax>
                            &#x3C;Tax Code="21" Amount="0" CurrencyCode="AUD" Percent="5">
                                &#x3C;TaxDescription>
                                    &#x3C;Text>Insurance Premium Tax&#x3C;/Text>
                                &#x3C;/TaxDescription>
                            &#x3C;/Tax>
                        &#x3C;/Taxes>
                    &#x3C;/Total>
                    &#x3C;ResGuestRPHs>
                        &#x3C;ResGuestRPH RPH="1"/>
                        &#x3C;ResGuestRPH RPH="2"/>
                    &#x3C;/ResGuestRPHs>
                    &#x3C;Memberships>
                        &#x3C;Membership ProgramCode="Platinum" AccountID="8943112"/>
                        &#x3C;Membership ProgramCode="Platinum" AccountID="8943966"/>
                    &#x3C;/Memberships>
                    &#x3C;Comments>
                        &#x3C;Comment GuestViewable="true">
                            &#x3C;Text>Platinum Members are offered a free spa entry for the whole length of stay.&#x3C;/Text>
                        &#x3C;/Comment>
                    &#x3C;/Comments>
                    &#x3C;SpecialRequests>
                        &#x3C;SpecialRequest RequestCode="Bedding Configuration" CodeContext="GUEST_DIRECT">
                            &#x3C;Text>King Split + Single Bed.&#x3C;/Text>
                        &#x3C;/SpecialRequest>
                        &#x3C;SpecialRequest RequestCode="Smoking" CodeContext="CHANNEL">
                            &#x3C;Text>Non-smoking room.&#x3C;/Text>
                        &#x3C;/SpecialRequest>
                    &#x3C;/SpecialRequests>
                &#x3C;/RoomStay>
            &#x3C;/RoomStays>
            &#x3C;Services>
                &#x3C;Service ServicePricingType="Per night" ServiceCategoryCode="PARKING" ServiceInventoryCode="ACAR_PARK" Inclusive="true" Quantity="1" ServiceRPH="1" Type="10" ID="01120212A3" ID_Context="HOTEL">
                    &#x3C;Price>
                        &#x3C;Total AmountBeforeTax="20.00" AmountAfterTax="22.00" CurrencyCode="AUD">
                            &#x3C;Taxes CurrencyCode="AUD" Amount="2.00">
                                &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                                    &#x3C;TaxDescription>
                                        &#x3C;Text>GST&#x3C;/Text>
                                    &#x3C;/TaxDescription>
                                &#x3C;/Tax>
                            &#x3C;/Taxes>
                        &#x3C;/Total>
                    &#x3C;/Price>
                    &#x3C;ServiceDetails>
                        &#x3C;GuestCounts>
                            &#x3C;GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
                        &#x3C;/GuestCounts>
                        &#x3C;TimeSpan Start="2017-12-01" End="2017-12-03"/>
                        &#x3C;Comments>
                            &#x3C;Comment GuestViewable="false">
                                &#x3C;Text>Car space needs to be released before 3PM check-out day. No exceptions allowed.&#x3C;/Text>
                            &#x3C;/Comment>
                        &#x3C;/Comments>
                        &#x3C;ServiceDescription>
                            &#x3C;Text>Accessible, covered and secured vehicle storage space.&#x3C;/Text>
                        &#x3C;/ServiceDescription>
                    &#x3C;/ServiceDetails>
                &#x3C;/Service>             
                &#x3C;Service ServicePricingType="Per person" ServiceCategoryCode="GUEST" ServiceInventoryCode="CLIENT" Inclusive="false" Quantity="1" ServiceRPH="2" Type="1" ID="CLI8569" ID_Context="GUEST_DIRECT">
                    &#x3C;Price>
                        &#x3C;Total AmountBeforeTax="30.00" AmountAfterTax="36.00" CurrencyCode="AUD">
                            &#x3C;Taxes CurrencyCode="AUD" Amount="6.00">
                                &#x3C;Tax Code="14" Amount="0" CurrencyCode="AUD" Percent="20">
                                    &#x3C;TaxDescription>
                                        &#x3C;Text>Service charge&#x3C;/Text>
                                    &#x3C;/TaxDescription>
                                &#x3C;/Tax>
                            &#x3C;/Taxes>
                        &#x3C;/Total>
                    &#x3C;/Price>
                    &#x3C;ServiceDetails>
                        &#x3C;GuestCounts>
                            &#x3C;GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
                        &#x3C;/GuestCounts>
                        &#x3C;TimeSpan Start="2017-12-01" End="2017-12-02"/>
                        &#x3C;Comments>
                            &#x3C;Comment GuestViewable="true">
                                &#x3C;Text>French manicure - Platinum Members are offered a free pedicure.&#x3C;/Text>
                            &#x3C;/Comment>
                        &#x3C;/Comments>
                        &#x3C;ServiceDescription>
                            &#x3C;Text>Manicure and pedicure set.&#x3C;/Text>
                        &#x3C;/ServiceDescription>
                    &#x3C;/ServiceDetails>
                &#x3C;/Service>
                &#x3C;ServiceCategory ServiceCategoryCode="PARKING"/>
                &#x3C;ServiceCategory ServiceCategoryCode="GUEST"/>
            &#x3C;/Services>
            &#x3C;BillingInstructionCode BillingCode="385H45991" AccountNumber="WOOLF05301300" Start="2017-12-01" End="2017-12-03" AuthorizationCode="7985" Description="Please follow billing instructions for Platinum Membership.">
                &#x3C;ResGuestRPH RPH="1"/>
            &#x3C;/BillingInstructionCode>
            &#x3C;ResGuests>
                &#x3C;ResGuest ResGuestRPH="1" AgeQualifyingCode="10" ArrivalTime="13:30:00" PrimaryIndicator="true" Age="51">
                    &#x3C;Profiles>
                        &#x3C;ProfileInfo>
                            &#x3C;UniqueID Type="1" ID="8943112" ID_Context="PROPERTY"/>
                            &#x3C;Profile ProfileType="1" ShareAllOptOutInd="true" ShareAllMarketInd="false">
                                &#x3C;Customer VIP_Indicator="true" CustomerValue="Platinum" BirthDate="1966-07-16">
                                    &#x3C;PersonName NameType="2" Language="en">
                                        &#x3C;NamePrefix>Mrs.&#x3C;/NamePrefix>
                                        &#x3C;GivenName>Ginny&#x3C;/GivenName>
                                        &#x3C;MiddleName>Adeline&#x3C;/MiddleName>
                                        &#x3C;Surname>Woolf&#x3C;/Surname>
                                        &#x3C;NameSuffix>Jr.&#x3C;/NameSuffix>
                                        &#x3C;NameTitle>Ph.D.&#x3C;/NameTitle>
                                    &#x3C;/PersonName>
                                    &#x3C;Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="13855956" Remark="Active" FormattedInd="false" DefaultInd="true"/>
                                    &#x3C;Email DefaultInd="true" EmailType="1">Virginia.Woolf@hotmail.com&#x3C;/Email>
                                    &#x3C;Address Type="2">
                                        &#x3C;AddressLine>125 Pitt Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2000&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                        &#x3C;CompanyName Code="DLW">Dalloway&#x3C;/CompanyName>
                                        &#x3C;AddresseeName NameType="2" Language="en">
                                            &#x3C;NamePrefix>Mrs.&#x3C;/NamePrefix>
                                            &#x3C;GivenName>Ginny&#x3C;/GivenName>
                                            &#x3C;MiddleName>Adeline&#x3C;/MiddleName>
                                            &#x3C;Surname>Woolf&#x3C;/Surname>
                                            &#x3C;NameSuffix>Jr.&#x3C;/NameSuffix>
                                            &#x3C;NameTitle>Ph.D.&#x3C;/NameTitle>
                                        &#x3C;/AddresseeName>
                                    &#x3C;/Address>
                                    &#x3C;RelatedTraveler Relation="Security" BirthDate="1958-12-01">
                                        &#x3C;UniqueID Type="1" ID="8943125" ID_Context="Platinum_Member"/>
                                        &#x3C;PersonName NameType="2" Language="en">
                                            &#x3C;NamePrefix>Mr.&#x3C;/NamePrefix>
                                            &#x3C;GivenName>Charles&#x3C;/GivenName>
                                            &#x3C;MiddleName>Hank&#x3C;/MiddleName>
                                            &#x3C;Surname>Bukowski&#x3C;/Surname>
                                            &#x3C;NameSuffix>Sr.&#x3C;/NameSuffix>
                                            &#x3C;NameTitle>D.Lett.&#x3C;/NameTitle>
                                        &#x3C;/PersonName>
                                    &#x3C;/RelatedTraveler>
                                    &#x3C;CustLoyalty ProgramID="PLATINUM5+5" MembershipID="8943112" LoyalLevel="VIP" LoyalLevelCode="10" SignupDate="2014-08-08" EffectiveDate="2014-08-08" ExpireDate="2024-08-08" Remark="5+5 DEAL (Sign up for 5 years of Platinum membership, get another 5 years for free)"/>
                                &#x3C;/Customer>
                                &#x3C;CompanyInfo>
                                    &#x3C;CompanyName Code="DLW">Dalloway&#x3C;/CompanyName>
                                    &#x3C;AddressInfo Type="2">
                                        &#x3C;AddressLine>88 Pall Mall&#x3C;/AddressLine>
                                        &#x3C;CityName>London&#x3C;/CityName>
                                        &#x3C;PostalCode>SW1Y 5ER&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="ENG">England&#x3C;/StateProv>
                                        &#x3C;CountryName Code="UK">United Kingdom&#x3C;/CountryName>
                                    &#x3C;/AddressInfo>
                                    &#x3C;TelephoneInfo PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="44" AreaCityCode="20" PhoneNumber="23983039" Remark="Only active during business hours: 8AM-8PM BST" FormattedInd="false" DefaultInd="true"/>
                                    &#x3C;Email DefaultInd="true" EmailType="2">info@dalloway.co.uk&#x3C;/Email>
                                    &#x3C;ContactPerson>
                                        &#x3C;PersonName NameType="3" Language="en-UK">
                                            &#x3C;NamePrefix>Mr.&#x3C;/NamePrefix>
                                            &#x3C;GivenName>Warren&#x3C;/GivenName>
                                            &#x3C;MiddleName>Glass&#x3C;/MiddleName>
                                            &#x3C;Surname>Smith&#x3C;/Surname>
                                            &#x3C;NameSuffix>II&#x3C;/NameSuffix>
                                            &#x3C;NameTitle>M.D.&#x3C;/NameTitle>
                                        &#x3C;/PersonName>
                                        &#x3C;Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="44" AreaCityCode="20" PhoneNumber="28596654" Remark="Active" FormattedInd="false" DefaultInd="true"/>
                                        &#x3C;Address Type="2">
                                            &#x3C;AddressLine>88 Pall Mall&#x3C;/AddressLine>
                                            &#x3C;CityName>London&#x3C;/CityName>
                                            &#x3C;PostalCode>SW1Y 5ER&#x3C;/PostalCode>
                                            &#x3C;StateProv StateCode="ENG">England&#x3C;/StateProv>
                                            &#x3C;CountryName Code="UK">United Kingdom&#x3C;/CountryName>
                                        &#x3C;/Address>
                                        &#x3C;Email DefaultInd="true" EmailType="2">Phillip.Glass-Smith@dalloway.co.uk&#x3C;/Email>
                                    &#x3C;/ContactPerson>
                                &#x3C;/CompanyInfo>
                            &#x3C;/Profile>
                        &#x3C;/ProfileInfo>
                    &#x3C;/Profiles>
                    &#x3C;SpecialRequests>
                        &#x3C;SpecialRequest RequestCode="Room features" CodeContext="GUEST_DIRECT">
                            &#x3C;Text>Aircon off&#x3C;/Text>
                        &#x3C;/SpecialRequest>
                    &#x3C;/SpecialRequests>
                    &#x3C;Comments>
                        &#x3C;Comment GuestViewable="false">
                            &#x3C;Text>No flowers - pollen allergy.&#x3C;/Text>
                        &#x3C;/Comment>
                    &#x3C;/Comments>
                    &#x3C;ServiceRPHs>
                        &#x3C;ServiceRPH RPH="2"/>
                    &#x3C;/ServiceRPHs>
                    &#x3C;ArrivalTransport>
                        &#x3C;TransportInfo Type="Rail" ID="80D-AAE" Time="2017-12-01T09:25:00"/>
                    &#x3C;/ArrivalTransport>
                    &#x3C;DepartureTransport>
                        &#x3C;TransportInfo Type="Rail" ID="77D-ABB" Time="2017-12-03T20:05:00"/>
                    &#x3C;/DepartureTransport>
                &#x3C;/ResGuest>
                &#x3C;ResGuest ResGuestRPH="2" AgeQualifyingCode="10" ArrivalTime="15:30:00" PrimaryIndicator="false" Age="44">
                    &#x3C;Profiles>
                        &#x3C;ProfileInfo>
                            &#x3C;UniqueID Type="1" ID="8943966" ID_Context="PROPERTY"/>
                            &#x3C;Profile ProfileType="1" ShareAllOptOutInd="true" ShareAllMarketInd="false">
                                &#x3C;Customer VIP_Indicator="true" CustomerValue="Platinum" BirthDate="1973-04-12">
                                    &#x3C;PersonName NameType="2" Language="en">
                                        &#x3C;NamePrefix>Mr.&#x3C;/NamePrefix>
                                        &#x3C;GivenName>Willy&#x3C;/GivenName>
                                        &#x3C;Surname>Bradshaw&#x3C;/Surname>
                                    &#x3C;/PersonName>
                                    &#x3C;Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="138564216" Remark="Active" FormattedInd="false" DefaultInd="true"/>
                                    &#x3C;Email DefaultInd="true" EmailType="2">WBradshaw@orlando.com.au&#x3C;/Email>
                                    &#x3C;Address Type="1">
                                        &#x3C;AddressLine>3 Hunter Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2017&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                        &#x3C;AddresseeName Language="en">
                                            &#x3C;NamePrefix>Mr.&#x3C;/NamePrefix>
                                            &#x3C;GivenName>William&#x3C;/GivenName>
                                            &#x3C;Surname>Bradshaw&#x3C;/Surname>
                                            &#x3C;NameSuffix>Sr.&#x3C;/NameSuffix>
                                        &#x3C;/AddresseeName>
                                    &#x3C;/Address>
                                    &#x3C;CustLoyalty ProgramID="PLAT" MembershipID="8943966" LoyalLevel="VIP" LoyalLevelCode="10" SignupDate="2016-04-18" EffectiveDate="2016-06-25" ExpireDate="2021-06-25" Remark="Standard 5 year membership."/>
                                &#x3C;/Customer>
                                &#x3C;CompanyInfo>
                                    &#x3C;CompanyName Code="ORL">Orlando&#x3C;/CompanyName>
                                    &#x3C;AddressInfo Type="2">
                                        &#x3C;AddressLine>175B George Street&#x3C;/AddressLine>
                                        &#x3C;CityName>Sydney&#x3C;/CityName>
                                        &#x3C;PostalCode>2000&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                        &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                    &#x3C;/AddressInfo>
                                    &#x3C;TelephoneInfo PhoneLocationType="7" PhoneTechType="1" CountryAccessCode="61" AreaCityCode="2" PhoneNumber="45665039" Remark="All phone calls are recorded." FormattedInd="false" DefaultInd="true"/>
                                    &#x3C;Email DefaultInd="true" EmailType="2">info@orlando.com.au&#x3C;/Email>
                                &#x3C;/CompanyInfo>
                            &#x3C;/Profile>
                        &#x3C;/ProfileInfo>
                    &#x3C;/Profiles>
                    &#x3C;Comments>
                        &#x3C;Comment GuestViewable="false">
                            &#x3C;Text>Disability - accessible room and parking space necessary.&#x3C;/Text>
                        &#x3C;/Comment>
                    &#x3C;/Comments>
                    &#x3C;ArrivalTransport>
                        &#x3C;TransportInfo Type="Air" ID="QR199" Time="2017-12-01T12:30:00"/>
                    &#x3C;/ArrivalTransport>
                    &#x3C;DepartureTransport>
                        &#x3C;TransportInfo Type="Rail" ID="77D-ABB" Time="2017-12-03T20:05:00"/>
                    &#x3C;/DepartureTransport>
                &#x3C;/ResGuest>
            &#x3C;/ResGuests>
            &#x3C;ResGlobalInfo>
                &#x3C;GuestCounts>
                    &#x3C;GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
                    &#x3C;GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
                &#x3C;/GuestCounts>
                &#x3C;TimeSpan Start="2017-12-01" End="2017-12-03"/>
                &#x3C;Memberships>
                    &#x3C;Membership ProgramCode="Platinum" AccountID="8943112"/>
                    &#x3C;Membership ProgramCode="Platinum" AccountID="8943966"/>
                &#x3C;/Memberships>
                &#x3C;Comments>
                    &#x3C;Comment GuestViewable="true">
                        &#x3C;Text>Business trip&#x3C;/Text>
                    &#x3C;/Comment>
                &#x3C;/Comments>
                &#x3C;SpecialRequests>
                    &#x3C;SpecialRequest RequestCode="Staff" CodeContext="GUEST_DIRECT">
                        &#x3C;Text>Please make sure your chef Leonard is on duty during our stay, thanks.&#x3C;/Text>
                    &#x3C;/SpecialRequest>
                &#x3C;/SpecialRequests>
                &#x3C;Guarantee GuaranteeCode="COMBINED_GUARANTEE" GuaranteeType="DepositRequired">
                            &#x3C;GuaranteesAccepted>
                                &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                    &#x3C;PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
                                        &#x3C;CardHolderName>Leonard Woolf&#x3C;/CardHolderName>
                                        &#x3C;CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
                                        &#x3C;/CardNumber>
                                    &#x3C;/PaymentCard>
                                &#x3C;/GuaranteeAccepted>
                                &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                    &#x3C;Voucher SeriesCode="4555"/>
                                &#x3C;/GuaranteeAccepted>
                                &#x3C;GuaranteeAccepted PaymentTransactionTypeCode="charge">
                                    &#x3C;DirectBill DirectBill_ID="4981003"/>
                                &#x3C;/GuaranteeAccepted>
                            &#x3C;/GuaranteesAccepted>
                            &#x3C;GuaranteeDescription>
                                &#x3C;Text>Combined Guarantees Accepted (Platinum Membership)&#x3C;/Text>
                            &#x3C;/GuaranteeDescription>
                        &#x3C;/Guarantee>
                        &#x3C;DepositPayments>
                            &#x3C;GuaranteePayment>
                                &#x3C;AcceptedPayments>
                                    &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                        &#x3C;PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
                                            &#x3C;CardHolderName>Leonard Woolf&#x3C;/CardHolderName>
                                            &#x3C;CardNumber Mask="4021XXXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
                                            &#x3C;/CardNumber>
                                        &#x3C;/PaymentCard>
                                    &#x3C;/AcceptedPayment>
                                &#x3C;/AcceptedPayments>
                                &#x3C;AmountPercent Percent="30" CurrencyCode="AUD" Amount="76.67" NmbrOfNights="2">
                                    &#x3C;Taxes CurrencyCode="AUD" Amount="1.53">
                                        &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="2">
                                            &#x3C;TaxDescription>
                                                &#x3C;Text>Credit Card surcharge.&#x3C;/Text>
                                            &#x3C;/TaxDescription>
                                        &#x3C;/Tax>
                                    &#x3C;/Taxes>
                                &#x3C;/AmountPercent>
                                &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                &#x3C;Description>
                                    &#x3C;Text>30% deposit (of the total reservation cost) will be charged to card holder's account 10 days before the date of arrival at the latest.&#x3C;/Text>
                                &#x3C;/Description>
                                &#x3C;Address Type="1">
                                    &#x3C;AddressLine>12 Pine Street&#x3C;/AddressLine>
                                    &#x3C;CityName>Sydney&#x3C;/CityName>
                                    &#x3C;PostalCode>2095&#x3C;/PostalCode>
                                    &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                    &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                &#x3C;/Address>
                            &#x3C;/GuaranteePayment>
                            &#x3C;GuaranteePayment>
                                &#x3C;AcceptedPayments>
                                    &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                        &#x3C;Voucher SeriesCode="4555"/>
                                    &#x3C;/AcceptedPayment>
                                &#x3C;/AcceptedPayments>
                                &#x3C;AmountPercent Percent="10" CurrencyCode="AUD" Amount="25.56" NmbrOfNights="2">
                                    &#x3C;Taxes CurrencyCode="AUD" Amount="1.28">
                                        &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
                                            &#x3C;TaxDescription>
                                                &#x3C;Text>Payment surcharge.&#x3C;/Text>
                                            &#x3C;/TaxDescription>
                                        &#x3C;/Tax>
                                    &#x3C;/Taxes>
                                &#x3C;/AmountPercent>
                                &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                &#x3C;Description>
                                    &#x3C;Text>10% deposit (of the total reservation cost) will be charged using provided Voucher code 10 days before the date of arrival at the latest.&#x3C;/Text>
                                &#x3C;/Description>
                                &#x3C;Address Type="1">
                                    &#x3C;AddressLine>12 Pine Street&#x3C;/AddressLine>
                                    &#x3C;CityName>Sydney&#x3C;/CityName>
                                    &#x3C;PostalCode>2095&#x3C;/PostalCode>
                                    &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                    &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                &#x3C;/Address>
                            &#x3C;/GuaranteePayment>
                            &#x3C;GuaranteePayment>
                                &#x3C;AcceptedPayments>
                                    &#x3C;AcceptedPayment PaymentTransactionTypeCode="charge">
                                        &#x3C;DirectBill DirectBill_ID="4981003"/>
                                    &#x3C;/AcceptedPayment>
                                &#x3C;/AcceptedPayments>
                                &#x3C;AmountPercent Percent="20" CurrencyCode="AUD" Amount="51.11" NmbrOfNights="2">
                                    &#x3C;Taxes CurrencyCode="AUD" Amount="2.56">
                                        &#x3C;Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
                                            &#x3C;TaxDescription>
                                                &#x3C;Text>Payment surcharge.&#x3C;/Text>
                                            &#x3C;/TaxDescription>
                                        &#x3C;/Tax>
                                    &#x3C;/Taxes>
                                &#x3C;/AmountPercent>
                                &#x3C;Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
                                &#x3C;Description>
                                    &#x3C;Text>20% deposit (of the total reservation cost) will be charged using Direct Bill ID provided 10 days before the date of arrival at the latest.&#x3C;/Text>
                                &#x3C;/Description>
                                &#x3C;Address Type="2">
                                    &#x3C;AddressLine>125 Pitt Street&#x3C;/AddressLine>
                                    &#x3C;CityName>Sydney&#x3C;/CityName>
                                    &#x3C;PostalCode>2000&#x3C;/PostalCode>
                                    &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                    &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                &#x3C;/Address>
                            &#x3C;/GuaranteePayment>
                        &#x3C;/DepositPayments>
                &#x3C;Total AmountBeforeTax="217.00" AmountAfterTax="255.55" CurrencyCode="AUD">
                    &#x3C;Taxes CurrencyCode="AUD" Amount="38.55">
                        &#x3C;Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
                            &#x3C;TaxDescription>
                                &#x3C;Text>GST&#x3C;/Text>
                            &#x3C;/TaxDescription>
                        &#x3C;/Tax>
                        &#x3C;Tax Code="21" Amount="0" CurrencyCode="AUD" Percent="5">
                            &#x3C;TaxDescription>
                                &#x3C;Text>Insurance Premium Tax&#x3C;/Text>
                            &#x3C;/TaxDescription>
                        &#x3C;/Tax>
                        &#x3C;Tax Code="14" Amount="6.00" CurrencyCode="AUD" Percent="0">
                            &#x3C;TaxDescription>
                                &#x3C;Text>Service charge - manicure&#x3C;/Text>
                            &#x3C;/TaxDescription>
                        &#x3C;/Tax>
                    &#x3C;/Taxes>
                &#x3C;/Total>
                &#x3C;HotelReservationIDs>
                    &#x3C;HotelReservationID ResID_Type="10" ResID_Value="BDC3685170919" ResID_Source="TESTPMS_GRHP6597"/>
                &#x3C;/HotelReservationIDs>
                &#x3C;Profiles>
                    &#x3C;ProfileInfo>
                        &#x3C;UniqueID Type="1" ID="8942213" ID_Context="PROPERTY"/>
                        &#x3C;Profile ShareAllMarketInd="true" ShareAllOptOutInd="false" ProfileType="1">
                            &#x3C;Customer VIP_Indicator="true" CustomerValue="5" BirthDate="1959-12-12">
                                &#x3C;PersonName NameType="2" Language="en">
                                    &#x3C;NamePrefix>Mr.&#x3C;/NamePrefix>
                                    &#x3C;GivenName>Leo&#x3C;/GivenName>
                                    &#x3C;MiddleName>Darcy&#x3C;/MiddleName>
                                    &#x3C;Surname>Woolf&#x3C;/Surname>
                                    &#x3C;NameSuffix>Ret.&#x3C;/NameSuffix>
                                    &#x3C;NameTitle>BA&#x3C;/NameTitle>
                                &#x3C;/PersonName>
                                &#x3C;Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="23865911" Remark="Active" FormattedInd="false" DefaultInd="true"/>
                                &#x3C;Email DefaultInd="true" EmailType="1">LeonardoWoolf59@gmail.com&#x3C;/Email>
                                &#x3C;Address Type="1">
                                    &#x3C;AddressLine>12 Pine Street&#x3C;/AddressLine>
                                    &#x3C;CityName>Sydney&#x3C;/CityName>
                                    &#x3C;PostalCode>2095&#x3C;/PostalCode>
                                    &#x3C;StateProv StateCode="NSW">New South Wales&#x3C;/StateProv>
                                    &#x3C;CountryName Code="AU">Australia&#x3C;/CountryName>
                                &#x3C;/Address>
                                &#x3C;CustLoyalty ProgramID="GOLD" MembershipID="8974358" LoyalLevel="VIP" LoyalLevelCode="2" SignupDate="2002-01-06" EffectiveDate="2002-01-06" ExpireDate="2032-01-06" Remark="30 years + Membership"/>
                            &#x3C;/Customer>
                        &#x3C;/Profile>
                    &#x3C;/ProfileInfo>
                    &#x3C;ProfileInfo>
                        &#x3C;Profile ProfileType="5">
                            &#x3C;CompanyInfo>
                                &#x3C;CompanyName Code="ASTERIX">Asterix&#x3C;/CompanyName>
                                &#x3C;AddressInfo Type="2">
                                    &#x3C;AddressLine>360C Bergen Street&#x3C;/AddressLine>
                                    &#x3C;CityName>New York - Brooklyn&#x3C;/CityName>
                                    &#x3C;PostalCode>11238&#x3C;/PostalCode>
                                    &#x3C;StateProv StateCode="NY">New York&#x3C;/StateProv>
                                    &#x3C;CountryName Code="US">United States&#x3C;/CountryName>
                                &#x3C;/AddressInfo>
                                &#x3C;TelephoneInfo  PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="1" AreaCityCode="212" PhoneNumber="44458561" Remark="Voicemail only" FormattedInd="false" DefaultInd="true"/>
                                &#x3C;Email DefaultInd="true" EmailType="2">support@asterix.com&#x3C;/Email>
                                &#x3C;ContactPerson>
                                    &#x3C;PersonName NameType="2" Language="en-US">
                                        &#x3C;NamePrefix>Ms.&#x3C;/NamePrefix>
                                        &#x3C;GivenName>Elle&#x3C;/GivenName>
                                        &#x3C;MiddleName>Maria&#x3C;/MiddleName>
                                        &#x3C;Surname>VanHoff&#x3C;/Surname>
                                        &#x3C;NameSuffix>Jr.&#x3C;/NameSuffix>
                                        &#x3C;NameTitle>M.D.&#x3C;/NameTitle>
                                    &#x3C;/PersonName>
                                    &#x3C;Telephone PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="1" AreaCityCode="212" PhoneNumber="44458562" Remark="Helpdesk" FormattedInd="false" DefaultInd="true"/>
                                    &#x3C;Address Type="0">
                                        &#x3C;AddressLine>360C Bergen Street&#x3C;/AddressLine>
                                        &#x3C;CityName>New York - Brooklyn&#x3C;/CityName>
                                        &#x3C;PostalCode>11238&#x3C;/PostalCode>
                                        &#x3C;StateProv StateCode="NY">New York&#x3C;/StateProv>
                                        &#x3C;CountryName Code="US">United States&#x3C;/CountryName>
                                    &#x3C;/Address>
                                    &#x3C;Email DefaultInd="true" EmailType="2">Elle.VanHoff@asterix.com&#x3C;/Email>
                                &#x3C;/ContactPerson>
                            &#x3C;/CompanyInfo>
                        &#x3C;/Profile>
                    &#x3C;/ProfileInfo>
                &#x3C;/Profiles>
                &#x3C;TotalCommissions>
                    &#x3C;UniqueID Type="5" ID="11395LYN"/>
                    &#x3C;CommissionPayableAmount CurrencyCode="AUD" Amount="25.00"/>
                    &#x3C;Comment>
                        &#x3C;Text>Booking agent reservation commission - flat rate.&#x3C;/Text>
                    &#x3C;/Comment>
                &#x3C;/TotalCommissions>
                &#x3C;BasicPropertyInfo ChainCode="GLDNRIV" BrandCode="GRH-P" HotelCode="GRHP6597" HotelName="Golden River Hotel - Perth"/>
            &#x3C;/ResGlobalInfo>
        &#x3C;/HotelReservation>
    &#x3C;/HotelReservations>
&#x3C;/OTA_HotelResNotifRQ>
</code></pre> |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
