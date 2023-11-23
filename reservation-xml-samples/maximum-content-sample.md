# Maximum Content Sample

The maximum content XML sample is for reference purposes only and it is an example of the maximum amount of data that your system could received from SMX.

{% code overflow="wrap" fullWidth="true" %}
```xml
<OTA_HotelResNotifRQ xmlns="http://www.opentravel.org/OTA/2003/05" Version="1.0" EchoToken="cc3048b5-55ca-4d77-b316-cb8e769c1381" TimeStamp="2017-09-19T18:13:53+00:00">
<HotelReservations>
<HotelReservation ResStatus="Reserved" CreateDateTime="2017-09-19T18:02:44+00:00" CreatorID="LINDA-RESAGENT" LastModifyDateTime="2017-09-19T18:13:51+00:00" LastModifierID="651651651651">
<POS>
<Source>
<RequestorID ID="TESTPMS"/>
</Source>
<Source>
<BookingChannel Type="4" Primary="true">
<CompanyName Code="Code1">CompanyName0</CompanyName>
</BookingChannel>
</Source>
</POS>
<UniqueID ID="BDC-3685569477"/>
<RoomStays>
<RoomStay MarketCode="Corporate" SourceOfBusiness="Radio" PromotionCode="STAYNSAVE15">
<RoomTypes>
<RoomType RoomType="Deluxe" RoomTypeCode="DLX" RoomCategory="4" RoomID="1501" NonSmoking="true" Configuration="King Split + Single Bed">
<RoomDescription>
<Text>Deluxe Room with a lovely view over the harbour and a seperate lounge with 50" LED TV</Text>
</RoomDescription>
<AdditionalDetails>
<AdditionalDetail Type="4" Code="CORNERROOM">
<DetailDescription>
<Text>This room is a Deluxe Corner Room</Text>
</DetailDescription>
</AdditionalDetail>
</AdditionalDetails>
</RoomType>
</RoomTypes>
<RatePlans>
<RatePlan RatePlanCode="WKGPKG" EffectiveDate="2017-12-01" ExpireDate="2017-12-03" RatePlanName="Weekend Package">
<RatePlanDescription>
<Text>Weekend Package includes wine, chocolates, champagne on arrival and late checkout at 3PM</Text>
</RatePlanDescription>
<RatePlanInclusions TaxInclusive="true" ServiceFeeInclusive="false">
<RatePlanInclusionDescription>
<Text>Champagne on arrival, English Breakfast, Chocolates and 3PM Checkout </Text>
</RatePlanInclusionDescription>
</RatePlanInclusions>
<MealsIncluded MealPlanIndicator="true" MealPlanCodes="7"/>
<AdditionalDetails>
<AdditionalDetail Type="12" Code="WKDNDPKGINFO">
<DetailDescription>
<Text>Some parts of this package (such as wine selection) will need to be arranged with guest prior to check-in</Text>
</DetailDescription>
</AdditionalDetail>
</AdditionalDetails>
</RatePlan>
</RatePlans>
<RoomRates>
<RoomRate InvBlockCode="HIGHROLL" NumberOfUnits="1" RoomID="1501" RoomTypeCode="DLX" RatePlanCode="WKGPKG" RatePlanCategory="Consumer Packages" EffectiveDate="2017-12-01" ExpireDate="2017-12-03">
<Rates>
<Rate EffectiveDate="2017-12-01" ExpireDate="2017-12-02" UnitMultiplier="1">
<Base AmountBeforeTax="100.00" AmountAfterTax="110.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="10.00">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
</Base>
<Total AmountBeforeTax="120.00" AmountAfterTax="132.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="12.00">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
</Rate>
<Rate EffectiveDate="2017-12-02" ExpireDate="2017-12-03" UnitMultiplier="1">
<Base AmountBeforeTax="80.00" AmountAfterTax="88.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="8.00">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
</Base>
<Total AmountBeforeTax="100.00" AmountAfterTax="110.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="10.00">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
</Rate>
</Rates>
<ServiceRPHs>
<ServiceRPH RPH="1"/>
</ServiceRPHs>
</RoomRate>
</RoomRates>
<GuestCounts>
<GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
<GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
</GuestCounts>
<TimeSpan Start="2017-12-01" End="2017-12-03"/>
<Guarantee GuaranteeCode="COMBINED_GUARANTEE" GuaranteeType="DepositRequired">
<GuaranteesAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
<CardHolderName>Leonard Woolf</CardHolderName>
<CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
</CardNumber>
</PaymentCard>
</GuaranteeAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<Voucher SeriesCode="4555"/>
</GuaranteeAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<DirectBill DirectBill_ID="4981003"/>
</GuaranteeAccepted>
</GuaranteesAccepted>
<GuaranteeDescription>
<Text>Combined Guarantees Accepted (Platinum Membership)</Text>
</GuaranteeDescription>
</Guarantee>
<DepositPayments>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
<CardHolderName>Leonard Woolf</CardHolderName>
<CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
</CardNumber>
</PaymentCard>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="30" CurrencyCode="AUD" Amount="64.52" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="1.29">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="2">
<TaxDescription>
<Text>Credit Card surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>30% deposit (of the total cost of the stay) will be charged to card holder's account 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="1">
<AddressLine>12 Pine Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2095</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<Voucher SeriesCode="4555"/>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="10" CurrencyCode="AUD" Amount="21.51" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="1.08">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Payment surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>10% deposit (of the total cost of the stay) will be charged using provided Voucher code 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="1">
<AddressLine>12 Pine Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2095</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<DirectBill DirectBill_ID="4981003"/>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="20" CurrencyCode="AUD" Amount="43.01" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="2.15">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Payment surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>20% deposit (of the total cost of the stay) will be charged using Direct Bill ID provided 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="2">
<AddressLine>125 Pitt Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2000</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
</DepositPayments>
<Discount TaxInclusive="true" Percent="15" DiscountCode="STAYNSAVE15" AmountBeforeTax="33.00" AmountAfterTax="36.30" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="3.30">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
<DiscountReason>
<Text>Stay 2 nights and get 15% off.</Text>
</DiscountReason>
</Discount>
<Total AmountBeforeTax="187.00" AmountAfterTax="215.05" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="28.05">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
<Tax Code="21" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Insurance Premium Tax</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
<ResGuestRPHs>
<ResGuestRPH RPH="1"/>
<ResGuestRPH RPH="2"/>
</ResGuestRPHs>
<Memberships>
<Membership ProgramCode="Platinum" AccountID="8943112"/>
<Membership ProgramCode="Platinum" AccountID="8943966"/>
</Memberships>
<Comments>
<Comment GuestViewable="true">
<Text>Platinum Members are offered a free spa entry for the whole length of stay.</Text>
</Comment>
</Comments>
<SpecialRequests>
<SpecialRequest RequestCode="Bedding Configuration" CodeContext="GUEST_DIRECT">
<Text>King Split + Single Bed.</Text>
</SpecialRequest>
<SpecialRequest RequestCode="Smoking" CodeContext="CHANNEL">
<Text>Non-smoking room.</Text>
</SpecialRequest>
</SpecialRequests>
</RoomStay>
</RoomStays>
<Services>
<Service ServicePricingType="Per night" ServiceCategoryCode="PARKING" ServiceInventoryCode="ACAR_PARK" Inclusive="true" Quantity="1" ServiceRPH="1" Type="10" ID="01120212A3" ID_Context="HOTEL">
<Price>
<Total AmountBeforeTax="20.00" AmountAfterTax="22.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="2.00">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
</Price>
<ServiceDetails>
<GuestCounts>
<GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
</GuestCounts>
<TimeSpan Start="2017-12-01" End="2017-12-03"/>
<Comments>
<Comment GuestViewable="false">
<Text>Car space needs to be released before 3PM check-out day. No exceptions allowed.</Text>
</Comment>
</Comments>
<ServiceDescription>
<Text>Accessible, covered and secured vehicle storage space.</Text>
</ServiceDescription>
</ServiceDetails>
</Service>
<Service ServicePricingType="Per person" ServiceCategoryCode="GUEST" ServiceInventoryCode="CLIENT" Inclusive="false" Quantity="1" ServiceRPH="2" Type="1" ID="CLI8569" ID_Context="GUEST_DIRECT">
<Price>
<Total AmountBeforeTax="30.00" AmountAfterTax="36.00" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="6.00">
<Tax Code="14" Amount="0" CurrencyCode="AUD" Percent="20">
<TaxDescription>
<Text>Service charge</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
</Price>
<ServiceDetails>
<GuestCounts>
<GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
</GuestCounts>
<TimeSpan Start="2017-12-01" End="2017-12-02"/>
<Comments>
<Comment GuestViewable="true">
<Text>French manicure - Platinum Members are offered a free pedicure.</Text>
</Comment>
</Comments>
<ServiceDescription>
<Text>Manicure and pedicure set.</Text>
</ServiceDescription>
</ServiceDetails>
</Service>
<ServiceCategory ServiceCategoryCode="PARKING"/>
<ServiceCategory ServiceCategoryCode="GUEST"/>
</Services>
<BillingInstructionCode BillingCode="385H45991" AccountNumber="WOOLF05301300" Start="2017-12-01" End="2017-12-03" AuthorizationCode="7985" Description="Please follow billing instructions for Platinum Membership.">
<ResGuestRPH RPH="1"/>
</BillingInstructionCode>
<ResGuests>
<ResGuest ResGuestRPH="1" AgeQualifyingCode="10" ArrivalTime="13:30:00" PrimaryIndicator="true" Age="51">
<Profiles>
<ProfileInfo>
<UniqueID Type="1" ID="8943112" ID_Context="PROPERTY"/>
<Profile ProfileType="1" ShareAllOptOutInd="true" ShareAllMarketInd="false">
<Customer VIP_Indicator="true" CustomerValue="Platinum" BirthDate="1966-07-16">
<PersonName NameType="2" Language="en">
<NamePrefix>Mrs.</NamePrefix>
<GivenName>Ginny</GivenName>
<MiddleName>Adeline</MiddleName>
<Surname>Woolf</Surname>
<NameSuffix>Jr.</NameSuffix>
<NameTitle>Ph.D.</NameTitle>
</PersonName>
<Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="13855956" Remark="Active" FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="1">Virginia.Woolf@hotmail.com</Email>
<Address Type="2">
<AddressLine>125 Pitt Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2000</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
<CompanyName Code="DLW">Dalloway</CompanyName>
<AddresseeName NameType="2" Language="en">
<NamePrefix>Mrs.</NamePrefix>
<GivenName>Ginny</GivenName>
<MiddleName>Adeline</MiddleName>
<Surname>Woolf</Surname>
<NameSuffix>Jr.</NameSuffix>
<NameTitle>Ph.D.</NameTitle>
</AddresseeName>
</Address>
<RelatedTraveler Relation="Security" BirthDate="1958-12-01">
<UniqueID Type="1" ID="8943125" ID_Context="Platinum_Member"/>
<PersonName NameType="2" Language="en">
<NamePrefix>Mr.</NamePrefix>
<GivenName>Charles</GivenName>
<MiddleName>Hank</MiddleName>
<Surname>Bukowski</Surname>
<NameSuffix>Sr.</NameSuffix>
<NameTitle>D.Lett.</NameTitle>
</PersonName>
</RelatedTraveler>
<CustLoyalty ProgramID="PLATINUM5+5" MembershipID="8943112" LoyalLevel="VIP" LoyalLevelCode="10" SignupDate="2014-08-08" EffectiveDate="2014-08-08" ExpireDate="2024-08-08" Remark="5+5 DEAL (Sign up for 5 years of Platinum membership, get another 5 years for free)"/>
</Customer>
<CompanyInfo>
<CompanyName Code="DLW">Dalloway</CompanyName>
<AddressInfo Type="2">
<AddressLine>88 Pall Mall</AddressLine>
<CityName>London</CityName>
<PostalCode>SW1Y 5ER</PostalCode>
<StateProv StateCode="ENG">England</StateProv>
<CountryName Code="UK">United Kingdom</CountryName>
</AddressInfo>
<TelephoneInfo PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="44" AreaCityCode="20" PhoneNumber="23983039" Remark="Only active during business hours: 8AM-8PM BST" FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="2">info@dalloway.co.uk</Email>
<ContactPerson>
<PersonName NameType="3" Language="en-UK">
<NamePrefix>Mr.</NamePrefix>
<GivenName>Warren</GivenName>
<MiddleName>Glass</MiddleName>
<Surname>Smith</Surname>
<NameSuffix>II</NameSuffix>
<NameTitle>M.D.</NameTitle>
</PersonName>
<Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="44" AreaCityCode="20" PhoneNumber="28596654" Remark="Active" FormattedInd="false" DefaultInd="true"/>
<Address Type="2">
<AddressLine>88 Pall Mall</AddressLine>
<CityName>London</CityName>
<PostalCode>SW1Y 5ER</PostalCode>
<StateProv StateCode="ENG">England</StateProv>
<CountryName Code="UK">United Kingdom</CountryName>
</Address>
<Email DefaultInd="true" EmailType="2">Phillip.Glass-Smith@dalloway.co.uk</Email>
</ContactPerson>
</CompanyInfo>
</Profile>
</ProfileInfo>
</Profiles>
<SpecialRequests>
<SpecialRequest RequestCode="Room features" CodeContext="GUEST_DIRECT">
<Text>Aircon off</Text>
</SpecialRequest>
</SpecialRequests>
<Comments>
<Comment GuestViewable="false">
<Text>No flowers - pollen allergy.</Text>
</Comment>
</Comments>
<ServiceRPHs>
<ServiceRPH RPH="2"/>
</ServiceRPHs>
<ArrivalTransport>
<TransportInfo Type="Rail" ID="80D-AAE" Time="2017-12-01T09:25:00"/>
</ArrivalTransport>
<DepartureTransport>
<TransportInfo Type="Rail" ID="77D-ABB" Time="2017-12-03T20:05:00"/>
</DepartureTransport>
</ResGuest>
<ResGuest ResGuestRPH="2" AgeQualifyingCode="10" ArrivalTime="15:30:00" PrimaryIndicator="false" Age="44">
<Profiles>
<ProfileInfo>
<UniqueID Type="1" ID="8943966" ID_Context="PROPERTY"/>
<Profile ProfileType="1" ShareAllOptOutInd="true" ShareAllMarketInd="false">
<Customer VIP_Indicator="true" CustomerValue="Platinum" BirthDate="1973-04-12">
<PersonName NameType="2" Language="en">
<NamePrefix>Mr.</NamePrefix>
<GivenName>Willy</GivenName>
<Surname>Bradshaw</Surname>
</PersonName>
<Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="138564216" Remark="Active" FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="2">WBradshaw@orlando.com.au</Email>
<Address Type="1">
<AddressLine>3 Hunter Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2017</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
<AddresseeName Language="en">
<NamePrefix>Mr.</NamePrefix>
<GivenName>William</GivenName>
<Surname>Bradshaw</Surname>
<NameSuffix>Sr.</NameSuffix>
</AddresseeName>
</Address>
<CustLoyalty ProgramID="PLAT" MembershipID="8943966" LoyalLevel="VIP" LoyalLevelCode="10" SignupDate="2016-04-18" EffectiveDate="2016-06-25" ExpireDate="2021-06-25" Remark="Standard 5 year membership."/>
</Customer>
<CompanyInfo>
<CompanyName Code="ORL">Orlando</CompanyName>
<AddressInfo Type="2">
<AddressLine>175B George Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2000</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</AddressInfo>
<TelephoneInfo PhoneLocationType="7" PhoneTechType="1" CountryAccessCode="61" AreaCityCode="2" PhoneNumber="45665039" Remark="All phone calls are recorded." FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="2">info@orlando.com.au</Email>
</CompanyInfo>
</Profile>
</ProfileInfo>
</Profiles>
<Comments>
<Comment GuestViewable="false">
<Text>Disability - accessible room and parking space necessary.</Text>
</Comment>
</Comments>
<ArrivalTransport>
<TransportInfo Type="Air" ID="QR199" Time="2017-12-01T12:30:00"/>
</ArrivalTransport>
<DepartureTransport>
<TransportInfo Type="Rail" ID="77D-ABB" Time="2017-12-03T20:05:00"/>
</DepartureTransport>
</ResGuest>
</ResGuests>
<ResGlobalInfo>
<GuestCounts>
<GuestCount AgeQualifyingCode="10" Age="51" Count="1" AgeBucket="AdultOver50"/>
<GuestCount AgeQualifyingCode="10" Age="44" Count="1" AgeBucket="AdultOver40"/>
</GuestCounts>
<TimeSpan Start="2017-12-01" End="2017-12-03"/>
<Memberships>
<Membership ProgramCode="Platinum" AccountID="8943112"/>
<Membership ProgramCode="Platinum" AccountID="8943966"/>
</Memberships>
<Comments>
<Comment GuestViewable="true">
<Text>Business trip</Text>
</Comment>
</Comments>
<SpecialRequests>
<SpecialRequest RequestCode="Staff" CodeContext="GUEST_DIRECT">
<Text>Please make sure your chef Leonard is on duty during our stay, thanks.</Text>
</SpecialRequest>
</SpecialRequests>
<Guarantee GuaranteeCode="COMBINED_GUARANTEE" GuaranteeType="DepositRequired">
<GuaranteesAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
<CardHolderName>Leonard Woolf</CardHolderName>
<CardNumber Mask="4021XXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
</CardNumber>
</PaymentCard>
</GuaranteeAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<Voucher SeriesCode="4555"/>
</GuaranteeAccepted>
<GuaranteeAccepted PaymentTransactionTypeCode="charge">
<DirectBill DirectBill_ID="4981003"/>
</GuaranteeAccepted>
</GuaranteesAccepted>
<GuaranteeDescription>
<Text>Combined Guarantees Accepted (Platinum Membership)</Text>
</GuaranteeDescription>
</Guarantee>
<DepositPayments>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<PaymentCard CardCode="VI" EffectiveDate="0717" ExpireDate="0720">
<CardHolderName>Leonard Woolf</CardHolderName>
<CardNumber Mask="4021XXXXXXXXX8995" Token="0087254835699221" TokenProviderID="VTS">
</CardNumber>
</PaymentCard>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="30" CurrencyCode="AUD" Amount="76.67" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="1.53">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="2">
<TaxDescription>
<Text>Credit Card surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>30% deposit (of the total reservation cost) will be charged to card holder's account 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="1">
<AddressLine>12 Pine Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2095</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<Voucher SeriesCode="4555"/>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="10" CurrencyCode="AUD" Amount="25.56" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="1.28">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Payment surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>10% deposit (of the total reservation cost) will be charged using provided Voucher code 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="1">
<AddressLine>12 Pine Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2095</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
<GuaranteePayment>
<AcceptedPayments>
<AcceptedPayment PaymentTransactionTypeCode="charge">
<DirectBill DirectBill_ID="4981003"/>
</AcceptedPayment>
</AcceptedPayments>
<AmountPercent Percent="20" CurrencyCode="AUD" Amount="51.11" NmbrOfNights="2">
<Taxes CurrencyCode="AUD" Amount="2.56">
<Tax Code="16" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Payment surcharge.</Text>
</TaxDescription>
</Tax>
</Taxes>
</AmountPercent>
<Deadline AbsoluteDeadline="2017-11-21T12:00:00+00:00" OffsetTimeUnit="Day" OffsetUnitMultiplier="10" OffsetDropTime="BeforeArrival"/>
<Description>
<Text>20% deposit (of the total reservation cost) will be charged using Direct Bill ID provided 10 days before the date of arrival at the latest.</Text>
</Description>
<Address Type="2">
<AddressLine>125 Pitt Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2000</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
</GuaranteePayment>
</DepositPayments>
<Total AmountBeforeTax="217.00" AmountAfterTax="255.55" CurrencyCode="AUD">
<Taxes CurrencyCode="AUD" Amount="38.55">
<Tax Code="19" Amount="0" CurrencyCode="AUD" Percent="10">
<TaxDescription>
<Text>GST</Text>
</TaxDescription>
</Tax>
<Tax Code="21" Amount="0" CurrencyCode="AUD" Percent="5">
<TaxDescription>
<Text>Insurance Premium Tax</Text>
</TaxDescription>
</Tax>
<Tax Code="14" Amount="6.00" CurrencyCode="AUD" Percent="0">
<TaxDescription>
<Text>Service charge - manicure</Text>
</TaxDescription>
</Tax>
</Taxes>
</Total>
<HotelReservationIDs>
<HotelReservationID ResID_Type="10" ResID_Value="BDC3685170919" ResID_Source="TESTPMS_GRHP6597"/>
</HotelReservationIDs>
<Profiles>
<ProfileInfo>
<UniqueID Type="1" ID="8942213" ID_Context="PROPERTY"/>
<Profile ShareAllMarketInd="true" ShareAllOptOutInd="false" ProfileType="1">
<Customer VIP_Indicator="true" CustomerValue="5" BirthDate="1959-12-12">
<PersonName NameType="2" Language="en">
<NamePrefix>Mr.</NamePrefix>
<GivenName>Leo</GivenName>
<MiddleName>Darcy</MiddleName>
<Surname>Woolf</Surname>
<NameSuffix>Ret.</NameSuffix>
<NameTitle>BA</NameTitle>
</PersonName>
<Telephone PhoneLocationType="10" PhoneTechType="5" CountryAccessCode="61" AreaCityCode="4" PhoneNumber="23865911" Remark="Active" FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="1">LeonardoWoolf59@gmail.com</Email>
<Address Type="1">
<AddressLine>12 Pine Street</AddressLine>
<CityName>Sydney</CityName>
<PostalCode>2095</PostalCode>
<StateProv StateCode="NSW">New South Wales</StateProv>
<CountryName Code="AU">Australia</CountryName>
</Address>
<CustLoyalty ProgramID="GOLD" MembershipID="8974358" LoyalLevel="VIP" LoyalLevelCode="2" SignupDate="2002-01-06" EffectiveDate="2002-01-06" ExpireDate="2032-01-06" Remark="30 years + Membership"/>
</Customer>
</Profile>
</ProfileInfo>
<ProfileInfo>
<Profile ProfileType="5">
<CompanyInfo>
<CompanyName Code="ASTERIX">Asterix</CompanyName>
<AddressInfo Type="2">
<AddressLine>360C Bergen Street</AddressLine>
<CityName>New York - Brooklyn</CityName>
<PostalCode>11238</PostalCode>
<StateProv StateCode="NY">New York</StateProv>
<CountryName Code="US">United States</CountryName>
</AddressInfo>
<TelephoneInfo  PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="1" AreaCityCode="212" PhoneNumber="44458561" Remark="Voicemail only" FormattedInd="false" DefaultInd="true"/>
<Email DefaultInd="true" EmailType="2">support@asterix.com</Email>
<ContactPerson>
<PersonName NameType="2" Language="en-US">
<NamePrefix>Ms.</NamePrefix>
<GivenName>Elle</GivenName>
<MiddleName>Maria</MiddleName>
<Surname>VanHoff</Surname>
<NameSuffix>Jr.</NameSuffix>
<NameTitle>M.D.</NameTitle>
</PersonName>
<Telephone PhoneLocationType="9" PhoneTechType="1" CountryAccessCode="1" AreaCityCode="212" PhoneNumber="44458562" Remark="Helpdesk" FormattedInd="false" DefaultInd="true"/>
<Address Type="0">
<AddressLine>360C Bergen Street</AddressLine>
<CityName>New York - Brooklyn</CityName>
<PostalCode>11238</PostalCode>
<StateProv StateCode="NY">New York</StateProv>
<CountryName Code="US">United States</CountryName>
</Address>
<Email DefaultInd="true" EmailType="2">Elle.VanHoff@asterix.com</Email>
</ContactPerson>
</CompanyInfo>
</Profile>
</ProfileInfo>
</Profiles>
<TotalCommissions>
<UniqueID Type="5" ID="11395LYN"/>
<CommissionPayableAmount CurrencyCode="AUD" Amount="25.00"/>
<Comment>
<Text>Booking agent reservation commission - flat rate.</Text>
</Comment>
</TotalCommissions>
<BasicPropertyInfo ChainCode="GLDNRIV" BrandCode="GRH-P" HotelCode="GRHP6597" HotelName="Golden River Hotel - Perth"/>
</ResGlobalInfo>
</HotelReservation>
</HotelReservations>
</OTA_HotelResNotifRQ>
```
{% endcode %}

