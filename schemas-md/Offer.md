Title: Offer - Schema.org Type

URL Source: https://schema.org/Offer

Markdown Content:
# Offer

A Schema.org Type

  [Thing](/Thing "Thing") \> [Intangible](/Intangible "Intangible") \>   [Offer](/Offer "Offer")  

**\[more...\]**

*   Canonical URL: https://schema.org/Offer
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+Offer)

An offer to transfer some rights to an item or to provide a service — for example, an offer to sell tickets to an event, to rent the DVD of a movie, to stream a TV show over the internet, to repair a motorcycle, or to loan a book.  
  
Note: As the [businessFunction](/businessFunction) property, which identifies the form of offer (e.g. sell, lease, repair, dispose), defaults to http://purl.org/goodrelations/v1#Sell; an Offer without a defined businessFunction value can be assumed to be an offer to sell.  
  
For [GTIN](http://www.gs1.org/barcodes/technical/idkeys/gtin)\-related fields, see [Check Digit calculator](http://www.gs1.org/barcodes/support/check_digit_calculator) and [validation guide](http://www.gs1us.org/resources/standards/gtin-validation-guide) from [GS1](http://www.gs1.org/).

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Offer](/Offer "Offer") |     |     |
| `[acceptedPaymentMethod](/acceptedPaymentMethod "acceptedPaymentMethod")` | [LoanOrCredit](/LoanOrCredit "LoanOrCredit")  or  <br>[PaymentMethod](/PaymentMethod "PaymentMethod")  or  <br>[Text](/Text "Text") | The payment method(s) that are accepted in general by an organization, or for some specific demand or offer. |
| `[addOn](/addOn "addOn")` | [Offer](/Offer "Offer") | An additional offer that can only be obtained in combination with the first base offer (e.g. supplements and extensions that are available for a surcharge). |
| `[additionalProperty](/additionalProperty "additionalProperty")` | [PropertyValue](/PropertyValue "PropertyValue") | A property-value pair representing an additional characteristic of the entity, e.g. a product feature or another characteristic for which there is no matching property in schema.org.  <br>  <br>Note: Publishers should be aware that applications designed to use specific schema.org properties (e.g. https://schema.org/width, https://schema.org/color, https://schema.org/gtin13, ...) will typically expect such data to be provided using those properties, rather than using the generic property/value mechanism. |
| `[advanceBookingRequirement](/advanceBookingRequirement "advanceBookingRequirement")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The amount of time that is required between accepting the offer and the actual usage of the resource or service. |
| `[aggregateRating](/aggregateRating "aggregateRating")` | [AggregateRating](/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| `[areaServed](/areaServed "areaServed")` | [AdministrativeArea](/AdministrativeArea "AdministrativeArea")  or  <br>[GeoShape](/GeoShape "GeoShape")  or  <br>[Place](/Place "Place")  or  <br>[Text](/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](/serviceArea "serviceArea"). |
| `[asin](/asin "asin")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | An Amazon Standard Identification Number (ASIN) is a 10-character alphanumeric unique identifier assigned by Amazon.com and its partners for product identification within the Amazon organization (summary from [Wikipedia](https://en.wikipedia.org/wiki/Amazon_Standard_Identification_Number)'s article).  <br>  <br>Note also that this is a definition for how to include ASINs in Schema.org data, and not a definition of ASINs in general - see documentation from Amazon for authoritative details. ASINs are most commonly encoded as text strings, but the \[asin\] property supports URL/URI as potential values too. |
| `[availability](/availability "availability")` | [ItemAvailability](/ItemAvailability "ItemAvailability") | The availability of this item—for example In stock, Out of stock, Pre-order, etc. |
| `[availabilityEnds](/availabilityEnds "availabilityEnds")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")  or  <br>[Time](/Time "Time") | The end of the availability of the product or service included in the offer. |
| `[availabilityStarts](/availabilityStarts "availabilityStarts")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime")  or  <br>[Time](/Time "Time") | The beginning of the availability of the product or service included in the offer. |
| `[availableAtOrFrom](/availableAtOrFrom "availableAtOrFrom")` | [Place](/Place "Place") | The place(s) from which the offer can be obtained (e.g. store locations). |
| `[availableDeliveryMethod](/availableDeliveryMethod "availableDeliveryMethod")` | [DeliveryMethod](/DeliveryMethod "DeliveryMethod") | The delivery method(s) available for this offer. |
| `[businessFunction](/businessFunction "businessFunction")` | [BusinessFunction](/BusinessFunction "BusinessFunction") | The business function (e.g. sell, lease, repair, dispose) of the offer or component of a bundle (TypeAndQuantityNode). The default is http://purl.org/goodrelations/v1#Sell. |
| `[category](/category "category")` | [CategoryCode](/CategoryCode "CategoryCode")  or  <br>[PhysicalActivityCategory](/PhysicalActivityCategory "PhysicalActivityCategory")  or  <br>[Text](/Text "Text")  or  <br>[Thing](/Thing "Thing")  or  <br>[URL](/URL "URL") | A category for the item. Greater signs or slashes can be used to informally indicate a category hierarchy. |
| `[checkoutPageURLTemplate](/checkoutPageURLTemplate "checkoutPageURLTemplate")` | [Text](/Text "Text") | A URL template (RFC 6570) for a checkout page for an offer. This approach allows merchants to specify a URL for online checkout of the offered product, by interpolating parameters such as the logged in user ID, product ID, quantity, discount code etc. Parameter naming and standardization are not specified here. |
| `[deliveryLeadTime](/deliveryLeadTime "deliveryLeadTime")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The typical delay between the receipt of the order and the goods either leaving the warehouse or being prepared for pickup, in case the delivery method is on site pickup. |
| `[eligibleCustomerType](/eligibleCustomerType "eligibleCustomerType")` | [BusinessEntityType](/BusinessEntityType "BusinessEntityType") | The type(s) of customers for which the given offer is valid. |
| `[eligibleDuration](/eligibleDuration "eligibleDuration")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The duration for which the given offer is valid. |
| `[eligibleQuantity](/eligibleQuantity "eligibleQuantity")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The interval and unit of measurement of ordering quantities for which the offer or price specification is valid. This allows e.g. specifying that a certain freight charge is valid only for a certain quantity. |
| `[eligibleRegion](/eligibleRegion "eligibleRegion")` | [GeoShape](/GeoShape "GeoShape")  or  <br>[Place](/Place "Place")  or  <br>[Text](/Text "Text") | The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code, the place, or the GeoShape for the geo-political region(s) for which the offer or delivery charge specification is valid.  <br>  <br>See also [ineligibleRegion](/ineligibleRegion). |
| `[eligibleTransactionVolume](/eligibleTransactionVolume "eligibleTransactionVolume")` | [PriceSpecification](/PriceSpecification "PriceSpecification") | The transaction volume, in a monetary unit, for which the offer or price specification is valid, e.g. for indicating a minimal purchasing volume, to express free shipping above a certain order volume, or to limit the acceptance of credit cards to purchases to a certain minimal amount. |
| `[gtin](/gtin "gtin")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | A Global Trade Item Number ([GTIN](https://www.gs1.org/standards/id-keys/gtin)). GTINs identify trade items, including products and services, using numeric identification codes.  <br>  <br>A correct [gtin](/gtin) value should be a valid GTIN, which means that it should be an all-numeric string of either 8, 12, 13 or 14 digits, or a "GS1 Digital Link" URL based on such a string. The numeric component should also have a [valid GS1 check digit](https://www.gs1.org/services/check-digit-calculator) and meet the other rules for valid GTINs. See also [GS1's GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) and [Wikipedia](https://en.wikipedia.org/wiki/Global_Trade_Item_Number) for more details. Left-padding of the gtin values is not required or encouraged. The [gtin](/gtin) property generalizes the earlier [gtin8](/gtin8), [gtin12](/gtin12), [gtin13](/gtin13), and [gtin14](/gtin14) properties.  <br>  <br>The GS1 [digital link specifications](https://www.gs1.org/standards/Digital-Link/) expresses GTINs as URLs (URIs, IRIs, etc.). Digital Links should be populated into the [hasGS1DigitalLink](/hasGS1DigitalLink) attribute.  <br>  <br>Note also that this is a definition for how to include GTINs in Schema.org data, and not a definition of GTINs in general - see the GS1 documentation for authoritative details. |
| `[gtin12](/gtin12 "gtin12")` | [Text](/Text "Text") | The GTIN-12 code of the product, or the product to which the offer refers. The GTIN-12 is the 12-digit GS1 Identification Key composed of a U.P.C. Company Prefix, Item Reference, and Check Digit used to identify trade items. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| `[gtin13](/gtin13 "gtin13")` | [Text](/Text "Text") | The GTIN-13 code of the product, or the product to which the offer refers. This is equivalent to 13-digit ISBN codes and EAN UCC-13. Former 12-digit UPC codes can be converted into a GTIN-13 code by simply adding a preceding zero. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| `[gtin14](/gtin14 "gtin14")` | [Text](/Text "Text") | The GTIN-14 code of the product, or the product to which the offer refers. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| `[gtin8](/gtin8 "gtin8")` | [Text](/Text "Text") | The GTIN-8 code of the product, or the product to which the offer refers. This code is also known as EAN/UCC-8 or 8-digit EAN. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| `[hasAdultConsideration](/hasAdultConsideration "hasAdultConsideration")` | [AdultOrientedEnumeration](/AdultOrientedEnumeration "AdultOrientedEnumeration") | Used to tag an item to be intended or suitable for consumption or use by adults only. |
| `[hasGS1DigitalLink](/hasGS1DigitalLink "hasGS1DigitalLink")` | [URL](/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](/Product) or an [Organization](/Organization), and for the correct granularity. In particular, for products:<br><br>*   A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](/IndividualProduct)<br>*   A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](/SomeProduct) if only products from that lot are sold, or [IndividualProduct](/IndividualProduct) if there is only a specific product.<br>*   A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](/Product) or a [ProductModel](/ProductModel).<br><br>Other item types should be adapted similarly. |
| `[hasMeasurement](/hasMeasurement "hasMeasurement")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | A measurement of an item, For example, the inseam of pants, the wheel size of a bicycle, the gauge of a screw, or the carbon footprint measured for certification by an authority. Usually an exact measurement, but can also be a range of measurements for adjustable products, for example belts and ski bindings. |
| `[hasMerchantReturnPolicy](/hasMerchantReturnPolicy "hasMerchantReturnPolicy")` | [MerchantReturnPolicy](/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](/hasProductReturnPolicy "hasProductReturnPolicy"). |
| `[includesObject](/includesObject "includesObject")` | [TypeAndQuantityNode](/TypeAndQuantityNode "TypeAndQuantityNode") | This links to a node or nodes indicating the exact quantity of the products included in an [Offer](/Offer) or [ProductCollection](/ProductCollection). |
| `[ineligibleRegion](/ineligibleRegion "ineligibleRegion")` | [GeoShape](/GeoShape "GeoShape")  or  <br>[Place](/Place "Place")  or  <br>[Text](/Text "Text") | The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code, the place, or the GeoShape for the geo-political region(s) for which the offer or delivery charge specification is not valid, e.g. a region where the transaction is not allowed.  <br>  <br>See also [eligibleRegion](/eligibleRegion). |
| `[inventoryLevel](/inventoryLevel "inventoryLevel")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The current approximate inventory level for the item or items. |
| `[isFamilyFriendly](/isFamilyFriendly "isFamilyFriendly")` | [Boolean](/Boolean "Boolean") | Indicates whether this content is family friendly. |
| `[itemCondition](/itemCondition "itemCondition")` | [OfferItemCondition](/OfferItemCondition "OfferItemCondition") | A predefined value from OfferItemCondition specifying the condition of the product or service, or the products or services included in the offer. Also used for product return policies to specify the condition of products accepted for returns. |
| `[itemOffered](/itemOffered "itemOffered")` | [AggregateOffer](/AggregateOffer "AggregateOffer")  or  <br>[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event")  or  <br>[MenuItem](/MenuItem "MenuItem")  or  <br>[Product](/Product "Product")  or  <br>[Service](/Service "Service")  or  <br>[Trip](/Trip "Trip") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer.  <br>Inverse property: [offers](/offers "offers") |
| `[leaseLength](/leaseLength "leaseLength")` | [Duration](/Duration "Duration")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue") | Length of the lease for some [Accommodation](/Accommodation), either particular to some [Offer](/Offer) or in some cases intrinsic to the property. |
| `[mobileUrl](/mobileUrl "mobileUrl")` | [Text](/Text "Text") | The [mobileUrl](/mobileUrl) property is provided for specific situations in which data consumers need to determine whether one of several provided URLs is a dedicated 'mobile site'.  <br>  <br>To discourage over-use, and reflecting intial usecases, the property is expected only on [Product](/Product) and [Offer](/Offer), rather than [Thing](/Thing). The general trend in web technology is towards [responsive design](https://en.wikipedia.org/wiki/Responsive_web_design) in which content can be flexibly adapted to a wide range of browsing environments. Pages and sites referenced with the long-established [url](/url) property should ideally also be usable on a wide variety of devices, including mobile phones. In most cases, it would be pointless and counter productive to attempt to update all [url](/url) markup to use [mobileUrl](/mobileUrl) for more mobile-oriented pages. The property is intended for the case when items (primarily [Product](/Product) and [Offer](/Offer)) have extra URLs hosted on an additional "mobile site" alongside the main one. It should not be taken as an endorsement of this publication style. |
| `[mpn](/mpn "mpn")` | [Text](/Text "Text") | The Manufacturer Part Number (MPN) of the product, or the product to which the offer refers. |
| `[offeredBy](/offeredBy "offeredBy")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A pointer to the organization or person making the offer.  <br>Inverse property: [makesOffer](/makesOffer "makesOffer") |
| `[price](/price "price")` | [Number](/Number "Number")  or  <br>[Text](/Text "Text") | The offer price of a product, or of a price component when attached to PriceSpecification and its subtypes.  <br>  <br>Usage guidelines:  <br>  <br><br>*   Use the [priceCurrency](/priceCurrency) property (with standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR") instead of including [ambiguous symbols](http://en.wikipedia.org/wiki/Dollar_sign#Currencies_that_use_the_dollar_or_peso_sign) such as '$' in the value.<br>*   Use '.' (Unicode 'FULL STOP' (U+002E)) rather than ',' to indicate a decimal point. Avoid using these symbols as a readability separator.<br>*   Note that both [RDFa](http://www.w3.org/TR/xhtml-rdfa-primer/#using-the-content-attribute) and Microdata syntax allow the use of a "content=" attribute for publishing simple machine-readable values alongside more human-friendly formatting.<br>*   Use values from 0123456789 (Unicode 'DIGIT ZERO' (U+0030) to 'DIGIT NINE' (U+0039)) rather than superficially similar Unicode symbols. |
| `[priceCurrency](/priceCurrency "priceCurrency")` | [Text](/Text "Text") | The currency of the price, or a price component when attached to [PriceSpecification](/PriceSpecification) and its subtypes.  <br>  <br>Use standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR". |
| `[priceSpecification](/priceSpecification "priceSpecification")` | [PriceSpecification](/PriceSpecification "PriceSpecification") | One or more detailed price specifications, indicating the unit price and delivery or payment charges. |
| `[priceValidUntil](/priceValidUntil "priceValidUntil")` | [Date](/Date "Date") | The date after which the price is no longer available. |
| `[review](/review "review")` | [Review](/Review "Review") | A review of the item. Supersedes [reviews](/reviews "reviews"). |
| `[seller](/seller "seller")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | An entity which offers (sells / leases / lends / loans) the services / goods. A seller may also be a provider. Supersedes [merchant](/merchant "merchant"), [vendor](/vendor "vendor"). |
| `[serialNumber](/serialNumber "serialNumber")` | [Text](/Text "Text") | The serial number or any alphanumeric identifier of a particular product. When attached to an offer, it is a shortcut for the serial number of the product included in the offer. |
| `[shippingDetails](/shippingDetails "shippingDetails")` | [OfferShippingDetails](/OfferShippingDetails "OfferShippingDetails") | Indicates information about the shipping policies and options associated with an [Offer](/Offer). |
| `[sku](/sku "sku")` | [Text](/Text "Text") | The Stock Keeping Unit (SKU), i.e. a merchant-specific identifier for a product or service, or the product to which the offer refers. |
| `[validForMemberTier](/validForMemberTier "validForMemberTier")` | [MemberProgramTier](/MemberProgramTier "MemberProgramTier") | The membership program tier an Offer (or a PriceSpecification, OfferShippingDetails, or MerchantReturnPolicy under an Offer) is valid for. |
| `[validFrom](/validFrom "validFrom")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The date when the item becomes valid. |
| `[validThrough](/validThrough "validThrough")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The date after when the item is not valid. For example the end of an offer, salary period, or a period of opening hours. |
| `[warranty](/warranty "warranty")` | [WarrantyPromise](/WarrantyPromise "WarrantyPromise") | The warranty promise(s) included in the offer. Supersedes [warrantyPromise](/warrantyPromise "warrantyPromise"). |
| Properties from [Thing](/Thing "Thing") |     |     |
| `[additionalType](/additionalType "additionalType")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. Typically the value is a URI-identified RDF class, and in this case corresponds to the use of rdf:type in RDF. Text values can be used sparingly, for cases where useful information can be added without their being an appropriate schema to reference. In the case of text values, the class label should follow the schema.org [style guide](https://schema.org/docs/styleguide.html). |
| `[alternateName](/alternateName "alternateName")` | [Text](/Text "Text") | An alias for the item. |
| `[description](/description "description")` | [Text](/Text "Text")  or  <br>[TextObject](/TextObject "TextObject") | A description of the item. |
| `[disambiguatingDescription](/disambiguatingDescription "disambiguatingDescription")` | [Text](/Text "Text") | A sub property of description. A short description of the item used to disambiguate from other, similar items. Information from other properties (in particular, name) may be necessary for the description to be useful for disambiguation. |
| `[identifier](/identifier "identifier")` | [PropertyValue](/PropertyValue "PropertyValue")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | The identifier property represents any kind of identifier for any kind of [Thing](/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](/docs/datamodel.html#identifierBg) for more details. |
| `[image](/image "image")` | [ImageObject](/ImageObject "ImageObject")  or  <br>[URL](/URL "URL") | An image of the item. This can be a [URL](/URL) or a fully described [ImageObject](/ImageObject). |
| `[mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See [background notes](/docs/datamodel.html#mainEntityBackground) for details.  <br>Inverse property: [mainEntity](/mainEntity "mainEntity") |
| `[name](/name "name")` | [Text](/Text "Text") | The name of the item. |
| `[potentialAction](/potentialAction "potentialAction")` | [Action](/Action "Action") | Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role. |
| `[sameAs](/sameAs "sameAs")` | [URL](/URL "URL") | URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website. |
| `[subjectOf](/subjectOf "subjectOf")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event") | A CreativeWork or Event about this Thing.  <br>Inverse property: [about](/about "about") |
| `[url](/url "url")` | [URL](/URL "URL") | URL of the item. |

  

Instances of [Offer](/Offer "Offer") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [acceptedOffer](/acceptedOffer "acceptedOffer") | [Order](/Order "Order") | The offer(s) -- e.g., product, quantity and price combinations -- included in the order. |
| [addOn](/addOn "addOn") | [Offer](/Offer "Offer") | An additional offer that can only be obtained in combination with the first base offer (e.g. supplements and extensions that are available for a surcharge). |
| [expectsAcceptanceOf](/expectsAcceptanceOf "expectsAcceptanceOf") | [ActionAccessSpecification](/ActionAccessSpecification "ActionAccessSpecification")  or  <br>[ConsumeAction](/ConsumeAction "ConsumeAction")  or  <br>[MediaSubscription](/MediaSubscription "MediaSubscription") | An Offer which must be accepted before the user can perform the Action. For example, the user may need to buy a movie before being able to watch it. |
| [makesOffer](/makesOffer "makesOffer") | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A pointer to products or services offered by the organization or person. |
| [offers](/offers "offers") | [AggregateOffer](/AggregateOffer "AggregateOffer")  or  <br>[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[EducationalOccupationalProgram](/EducationalOccupationalProgram "EducationalOccupationalProgram")  or  <br>[Event](/Event "Event")  or  <br>[MenuItem](/MenuItem "MenuItem")  or  <br>[Product](/Product "Product")  or  <br>[Service](/Service "Service")  or  <br>[Trip](/Trip "Trip") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |

  

#### More specific Types

*   [AggregateOffer](/AggregateOffer "AggregateOffer")
*   [OfferForLease](/OfferForLease "OfferForLease")
*   [OfferForPurchase](/OfferForPurchase "OfferForPurchase")

### Acknowledgements

GoodRelations Vocabulary Terms

This term [uses](http://blog.schema.org/2012/11/good-relations-and-schemaorg.html) terminology from the GoodRelations Vocabulary for E-Commerce, created by Martin Hepp. GoodRelations is a data model for sharing e-commerce data on the Web. More information about GoodRelations can be found at [http://purl.org/goodrelations/](http://purl.org/goodrelations/).

### Examples
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Product",
      "aggregateRating": {
        "@type": "AggregateRating",
        "ratingValue": "3.5",
        "reviewCount": "11"
      },
      "description": "0.7 cubic feet countertop microwave. Has six preset cooking categories and convenience features like Add-A-Minute and Child Lock.",
      "name": "Kenmore White 17\" Microwave",
      "image": "kenmore-microwave-17in.jpg",
      "offers": {
        "@type": "Offer",
        "availability": "https://schema.org/InStock",
        "price": "55.00",
        "priceCurrency": "USD"
      },
      "review": [
        {
          "@type": "Review",
          "author": "Ellie",
          "datePublished": "2011-04-01",
          "reviewBody": "The lamp burned out and now I have to replace it.",
          "name": "Not a happy camper",
          "reviewRating": {
            "@type": "Rating",
            "bestRating": "5",
            "ratingValue": "1",
            "worstRating": "1"
          }
        },
        {
          "@type": "Review",
          "author": "Lucas",
          "datePublished": "2011-03-25",
          "reviewBody": "Great microwave for the price. It is small and fits in my apartment.",
          "name": "Value purchase",
          "reviewRating": {
            "@type": "Rating",
            "bestRating": "5",
            "ratingValue": "4",
            "worstRating": "1"
          }
        }
      ]
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Product",
      "aggregateRating": {
        "@type": "AggregateRating",
        "bestRating": "100",
        "ratingCount": "24",
        "ratingValue": "87"
      },
      "image": "dell-30in-lcd.jpg",
      "name": "Dell UltraSharp 30\" LCD Monitor",
      "offers": {
        "@type": "AggregateOffer",
        "priceCurrency": "USD",
        "highPrice": "1495",
        "lowPrice": "1250",
        "offerCount": "8",
        "offers": [
          {
            "@type": "Offer",
            "url": "save-a-lot-monitors.com/dell-30.html"
          },
          {
            "@type": "Offer",
            "url": "jondoe-gadgets.com/dell-30.html"
          }
        ]
      }
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Event",
      "location": {
        "@type": "Place",
        "address": {
          "@type": "PostalAddress",
          "addressLocality": "Denver",
          "addressRegion": "CO",
          "postalCode": "80209",
          "streetAddress": "7 S. Broadway"
        },
        "name": "The Hi-Dive"
      },
      "name": "Typhoon with Radiation City",
      "offers": {
        "@type": "Offer",
        "price": "13.00",
        "priceCurrency": "USD",
        "url": "http://www.ticketfly.com/purchase/309433"
      },
      "startDate": "2013-09-14T21:30"
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context":"https://schema.org",
      "@id":"http://example.com/explosive-tennis-balls",
      "@type":"ItemPage",
      "copyrightYear":"2015",
      "copyrightHolder":{"@id":"#Organization"},
      "publisher":{"@id":"#Organization"},
      "mainEntity":{
        "@id":"#Product",
        "@type":"Product",
        "name":"Explosive tennis balls",
        "description":"Tickle your friends! Surprise your opponent!",
        "image":"http://example.com/explosive-tennis-balls.jpg",
        "url":"http://example.com/explosive-tennis-balls",
        "offers":{
          "@id":"#Offer",
          "@type":"Offer",
          "priceCurrency":"USD",
          "price":"1000.00",
          "availability":"https://schema.org/InStock",
          "itemOffered":{"@id":"#Product"},
            "offeredBy":{
              "@id":"#Organization",
              "@type":"Organization",
              "name":"Acme Inc",
              "logo":"http://example.commple.com/acme-inc-logo.jpg",
              "url":"http://example.com/",
              "sameAs":["https://twitter.com/AcmeInc","https://www.facebook.com/AcmeInc","https://plus.google.com/u/0/+AcmeInc/"]
            }
        }
      }
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Service",
      "serviceType": "Weekly home cleaning",
      "provider": {
        "@type": "LocalBusiness",
        "name": "ACME Home Cleaning"
      },
      "areaServed": {
        "@type": "State",
        "name": "Massachusetts"
      },
      "hasOfferCatalog": {
        "@type": "OfferCatalog",
        "name": "Cleaning services",
        "itemListElement": [
          {
            "@type": "OfferCatalog",
            "name": "House Cleaning",
            "itemListElement": [
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "Apartment light cleaning"
                }
              },
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "House light cleaning up to 2 bedrooms"
                }
              },
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "House light cleaning 3+ bedrooms"
                }
              }
            ]
          },
          {
            "@type": "OfferCatalog",
            "name": "One-time services",
            "itemListElement": [
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "Window washing"
                }
              },
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "Carpet cleaning"
                }
              },
              {
                "@type": "Offer",
                "itemOffered": {
                  "@type": "Service",
                  "name": "Move in/out cleaning"
                }
              }
            ]
          }
        ]
      }
    }
    </script>
```