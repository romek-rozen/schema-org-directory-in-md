Title: AggregateOffer - Schema.org Type

URL Source: https://schema.org/AggregateOffer

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

When a single product is associated with multiple offers (for example, the same pair of shoes is offered by different merchants), then AggregateOffer can be used.

Note: AggregateOffers are normally expected to associate multiple offers that all share the same defined [businessFunction](https://schema.org/businessFunction) value, or default to http://purl.org/goodrelations/v1#Sell if businessFunction is not explicitly defined.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [AggregateOffer](https://schema.org/AggregateOffer "AggregateOffer") |
| ``` highPrice ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The highest price of all offers available. Usage guidelines: * Use values from 0123456789 (Unicode 'DIGIT ZERO' (U+0030) to 'DIGIT NINE' (U+0039)) rather than superficially similar Unicode symbols. * Use '.' (Unicode 'FULL STOP' (U+002E)) rather than ',' to indicate a decimal point. Avoid using these symbols as a readability separator. |
| ``` lowPrice ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The lowest price of all offers available. Usage guidelines: * Use values from 0123456789 (Unicode 'DIGIT ZERO' (U+0030) to 'DIGIT NINE' (U+0039)) rather than superficially similar Unicode symbols. * Use '.' (Unicode 'FULL STOP' (U+002E)) rather than ',' to indicate a decimal point. Avoid using these symbols as a readability separator. |
| ``` offerCount ``` | [Integer](https://schema.org/Integer "Integer") | The number of offers for the product. |
| ``` offers ``` | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](https://schema.org/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](https://schema.org/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [itemOffered](https://schema.org/itemOffered "itemOffered") |
| Properties from [Offer](https://schema.org/Offer "Offer") |
| ``` acceptedPaymentMethod ``` | [LoanOrCredit](https://schema.org/LoanOrCredit "LoanOrCredit") or [PaymentMethod](https://schema.org/PaymentMethod "PaymentMethod") or [Text](https://schema.org/Text "Text") | The payment method(s) that are accepted in general by an organization, or for some specific demand or offer. |
| ``` addOn ``` | [Offer](https://schema.org/Offer "Offer") | An additional offer that can only be obtained in combination with the first base offer (e.g. supplements and extensions that are available for a surcharge). |
| ``` additionalProperty ``` | [PropertyValue](https://schema.org/PropertyValue "PropertyValue") | A property-value pair representing an additional characteristic of the entity, e.g. a product feature or another characteristic for which there is no matching property in schema.org. Note: Publishers should be aware that applications designed to use specific schema.org properties (e.g. https://schema.org/width, https://schema.org/color, https://schema.org/gtin13, ...) will typically expect such data to be provided using those properties, rather than using the generic property/value mechanism. |
| ``` advanceBookingRequirement ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The amount of time that is required between accepting the offer and the actual usage of the resource or service. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` areaServed ``` | [AdministrativeArea](https://schema.org/AdministrativeArea "AdministrativeArea") or [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](https://schema.org/serviceArea "serviceArea"). |
| ``` asin ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | An Amazon Standard Identification Number (ASIN) is a 10-character alphanumeric unique identifier assigned by Amazon.com and its partners for product identification within the Amazon organization (summary from [Wikipedia](https://en.wikipedia.org/wiki/Amazon_Standard_Identification_Number)'s article). Note also that this is a definition for how to include ASINs in Schema.org data, and not a definition of ASINs in general - see documentation from Amazon for authoritative details. ASINs are most commonly encoded as text strings, but the [asin] property supports URL/URI as potential values too. |
| ``` availability ``` | [ItemAvailability](https://schema.org/ItemAvailability "ItemAvailability") | The availability of this item—for example In stock, Out of stock, Pre-order, etc. |
| ``` availabilityEnds ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") or [Time](https://schema.org/Time "Time") | The end of the availability of the product or service included in the offer. |
| ``` availabilityStarts ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") or [Time](https://schema.org/Time "Time") | The beginning of the availability of the product or service included in the offer. |
| ``` availableAtOrFrom ``` | [Place](https://schema.org/Place "Place") | The place(s) from which the offer can be obtained (e.g. store locations). |
| ``` availableDeliveryMethod ``` | [DeliveryMethod](https://schema.org/DeliveryMethod "DeliveryMethod") | The delivery method(s) available for this offer. |
| ``` businessFunction ``` | [BusinessFunction](https://schema.org/BusinessFunction "BusinessFunction") | The business function (e.g. sell, lease, repair, dispose) of the offer or component of a bundle (TypeAndQuantityNode). The default is http://purl.org/goodrelations/v1#Sell. |
| ``` category ``` | [CategoryCode](https://schema.org/CategoryCode "CategoryCode") or [PhysicalActivityCategory](https://schema.org/PhysicalActivityCategory "PhysicalActivityCategory") or [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | A category for the item. Greater signs or slashes can be used to informally indicate a category hierarchy. |
| ``` checkoutPageURLTemplate ``` | [Text](https://schema.org/Text "Text") | A URL template (RFC 6570) for a checkout page for an offer. This approach allows merchants to specify a URL for online checkout of the offered product, by interpolating parameters such as the logged in user ID, product ID, quantity, discount code etc. Parameter naming and standardization are not specified here. |
| ``` deliveryLeadTime ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The typical delay between the receipt of the order and the goods either leaving the warehouse or being prepared for pickup, in case the delivery method is on site pickup. |
| ``` eligibleCustomerType ``` | [BusinessEntityType](https://schema.org/BusinessEntityType "BusinessEntityType") | The type(s) of customers for which the given offer is valid. |
| ``` eligibleDuration ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The duration for which the given offer is valid. |
| ``` eligibleQuantity ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The interval and unit of measurement of ordering quantities for which the offer or price specification is valid. This allows e.g. specifying that a certain freight charge is valid only for a certain quantity. |
| ``` eligibleRegion ``` | [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code, the place, or the GeoShape for the geo-political region(s) for which the offer or delivery charge specification is valid. See also [ineligibleRegion](https://schema.org/ineligibleRegion). |
| ``` eligibleTransactionVolume ``` | [PriceSpecification](https://schema.org/PriceSpecification "PriceSpecification") | The transaction volume, in a monetary unit, for which the offer or price specification is valid, e.g. for indicating a minimal purchasing volume, to express free shipping above a certain order volume, or to limit the acceptance of credit cards to purchases to a certain minimal amount. |
| ``` gtin ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | A Global Trade Item Number ([GTIN](https://www.gs1.org/standards/id-keys/gtin)). GTINs identify trade items, including products and services, using numeric identification codes. A correct [gtin](https://schema.org/gtin) value should be a valid GTIN, which means that it should be an all-numeric string of either 8, 12, 13 or 14 digits, or a "GS1 Digital Link" URL based on such a string. The numeric component should also have a [valid GS1 check digit](https://www.gs1.org/services/check-digit-calculator) and meet the other rules for valid GTINs. See also [GS1's GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) and [Wikipedia](https://en.wikipedia.org/wiki/Global_Trade_Item_Number) for more details. Left-padding of the gtin values is not required or encouraged. The [gtin](https://schema.org/gtin) property generalizes the earlier [gtin8](https://schema.org/gtin8), [gtin12](https://schema.org/gtin12), [gtin13](https://schema.org/gtin13), and [gtin14](https://schema.org/gtin14) properties. The GS1 [digital link specifications](https://www.gs1.org/standards/Digital-Link/) expresses GTINs as URLs (URIs, IRIs, etc.). Digital Links should be populated into the [hasGS1DigitalLink](https://schema.org/hasGS1DigitalLink) attribute. Note also that this is a definition for how to include GTINs in Schema.org data, and not a definition of GTINs in general - see the GS1 documentation for authoritative details. |
| ``` gtin12 ``` | [Text](https://schema.org/Text "Text") | The GTIN-12 code of the product, or the product to which the offer refers. The GTIN-12 is the 12-digit GS1 Identification Key composed of a U.P.C. Company Prefix, Item Reference, and Check Digit used to identify trade items. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin13 ``` | [Text](https://schema.org/Text "Text") | The GTIN-13 code of the product, or the product to which the offer refers. This is equivalent to 13-digit ISBN codes and EAN UCC-13. Former 12-digit UPC codes can be converted into a GTIN-13 code by simply adding a preceding zero. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin14 ``` | [Text](https://schema.org/Text "Text") | The GTIN-14 code of the product, or the product to which the offer refers. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin8 ``` | [Text](https://schema.org/Text "Text") | The GTIN-8 code of the product, or the product to which the offer refers. This code is also known as EAN/UCC-8 or 8-digit EAN. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` hasAdultConsideration ``` | [AdultOrientedEnumeration](https://schema.org/AdultOrientedEnumeration "AdultOrientedEnumeration") | Used to tag an item to be intended or suitable for consumption or use by adults only. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMeasurement ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | A measurement of an item, For example, the inseam of pants, the wheel size of a bicycle, the gauge of a screw, or the carbon footprint measured for certification by an authority. Usually an exact measurement, but can also be a range of measurements for adjustable products, for example belts and ski bindings. |
| ``` hasMerchantReturnPolicy ``` | [MerchantReturnPolicy](https://schema.org/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](https://schema.org/hasProductReturnPolicy "hasProductReturnPolicy"). |
| ``` includesObject ``` | [TypeAndQuantityNode](https://schema.org/TypeAndQuantityNode "TypeAndQuantityNode") | This links to a node or nodes indicating the exact quantity of the products included in an [Offer](https://schema.org/Offer) or [ProductCollection](https://schema.org/ProductCollection). |
| ``` ineligibleRegion ``` | [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The ISO 3166-1 (ISO 3166-1 alpha-2) or ISO 3166-2 code, the place, or the GeoShape for the geo-political region(s) for which the offer or delivery charge specification is not valid, e.g. a region where the transaction is not allowed. See also [eligibleRegion](https://schema.org/eligibleRegion). |
| ``` inventoryLevel ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The current approximate inventory level for the item or items. |
| ``` isFamilyFriendly ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether this content is family friendly. |
| ``` itemCondition ``` | [OfferItemCondition](https://schema.org/OfferItemCondition "OfferItemCondition") | A predefined value from OfferItemCondition specifying the condition of the product or service, or the products or services included in the offer. Also used for product return policies to specify the condition of products accepted for returns. |
| ``` itemOffered ``` | [AggregateOffer](https://schema.org/AggregateOffer "AggregateOffer") or [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") or [MenuItem](https://schema.org/MenuItem "MenuItem") or [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") or [Trip](https://schema.org/Trip "Trip") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](https://schema.org/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [offers](https://schema.org/offers "offers") |
| ``` leaseLength ``` | [Duration](https://schema.org/Duration "Duration") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | Length of the lease for some [Accommodation](https://schema.org/Accommodation), either particular to some [Offer](https://schema.org/Offer) or in some cases intrinsic to the property. |
| ``` mobileUrl ``` | [Text](https://schema.org/Text "Text") | The [mobileUrl](https://schema.org/mobileUrl) property is provided for specific situations in which data consumers need to determine whether one of several provided URLs is a dedicated 'mobile site'. To discourage over-use, and reflecting intial usecases, the property is expected only on [Product](https://schema.org/Product) and [Offer](https://schema.org/Offer), rather than [Thing](https://schema.org/Thing). The general trend in web technology is towards [responsive design](https://en.wikipedia.org/wiki/Responsive_web_design) in which content can be flexibly adapted to a wide range of browsing environments. Pages and sites referenced with the long-established [url](https://schema.org/url) property should ideally also be usable on a wide variety of devices, including mobile phones. In most cases, it would be pointless and counter productive to attempt to update all [url](https://schema.org/url) markup to use [mobileUrl](https://schema.org/mobileUrl) for more mobile-oriented pages. The property is intended for the case when items (primarily [Product](https://schema.org/Product) and [Offer](https://schema.org/Offer)) have extra URLs hosted on an additional "mobile site" alongside the main one. It should not be taken as an endorsement of this publication style. |
| ``` mpn ``` | [Text](https://schema.org/Text "Text") | The Manufacturer Part Number (MPN) of the product, or the product to which the offer refers. |
| ``` offeredBy ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A pointer to the organization or person making the offer. Inverse property: [makesOffer](https://schema.org/makesOffer "makesOffer") |
| ``` price ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The offer price of a product, or of a price component when attached to PriceSpecification and its subtypes. Usage guidelines: * Use the [priceCurrency](https://schema.org/priceCurrency) property (with standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR") instead of including [ambiguous symbols](http://en.wikipedia.org/wiki/Dollar_sign#Currencies_that_use_the_dollar_or_peso_sign) such as '$' in the value. * Use '.' (Unicode 'FULL STOP' (U+002E)) rather than ',' to indicate a decimal point. Avoid using these symbols as a readability separator. * Note that both [RDFa](http://www.w3.org/TR/xhtml-rdfa-primer/#using-the-content-attribute) and Microdata syntax allow the use of a "content=" attribute for publishing simple machine-readable values alongside more human-friendly formatting. * Use values from 0123456789 (Unicode 'DIGIT ZERO' (U+0030) to 'DIGIT NINE' (U+0039)) rather than superficially similar Unicode symbols. |
| ``` priceCurrency ``` | [Text](https://schema.org/Text "Text") | The currency of the price, or a price component when attached to [PriceSpecification](https://schema.org/PriceSpecification) and its subtypes. Use standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR". |
| ``` priceSpecification ``` | [PriceSpecification](https://schema.org/PriceSpecification "PriceSpecification") | One or more detailed price specifications, indicating the unit price and delivery or payment charges. |
| ``` priceValidUntil ``` | [Date](https://schema.org/Date "Date") | The date after which the price is no longer available. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` seller ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | An entity which offers (sells / leases / lends / loans) the services / goods. A seller may also be a provider. Supersedes [merchant](https://schema.org/merchant "merchant"), [vendor](https://schema.org/vendor "vendor"). |
| ``` serialNumber ``` | [Text](https://schema.org/Text "Text") | The serial number or any alphanumeric identifier of a particular product. When attached to an offer, it is a shortcut for the serial number of the product included in the offer. |
| ``` shippingDetails ``` | [OfferShippingDetails](https://schema.org/OfferShippingDetails "OfferShippingDetails") | Indicates information about the shipping policies and options associated with an [Offer](https://schema.org/Offer). |
| ``` sku ``` | [Text](https://schema.org/Text "Text") | The Stock Keeping Unit (SKU), i.e. a merchant-specific identifier for a product or service, or the product to which the offer refers. |
| ``` validForMemberTier ``` | [MemberProgramTier](https://schema.org/MemberProgramTier "MemberProgramTier") | The membership program tier an Offer (or a PriceSpecification, OfferShippingDetails, or MerchantReturnPolicy under an Offer) is valid for. |
| ``` validFrom ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date when the item becomes valid. |
| ``` validThrough ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date after when the item is not valid. For example the end of an offer, salary period, or a period of opening hours. |
| ``` warranty ``` | [WarrantyPromise](https://schema.org/WarrantyPromise "WarrantyPromise") | The warranty promise(s) included in the offer. Supersedes [warrantyPromise](https://schema.org/warrantyPromise "warrantyPromise"). |
| Properties from [Thing](https://schema.org/Thing "Thing") |
| ``` additionalType ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. Typically the value is a URI-identified RDF class, and in this case corresponds to the use of rdf:type in RDF. Text values can be used sparingly, for cases where useful information can be added without their being an appropriate schema to reference. In the case of text values, the class label should follow the schema.org [style guide](https://schema.org/docs/styleguide.html). |
| ``` alternateName ``` | [Text](https://schema.org/Text "Text") | An alias for the item. |
| ``` description ``` | [Text](https://schema.org/Text "Text") or [TextObject](https://schema.org/TextObject "TextObject") | A description of the item. |
| ``` disambiguatingDescription ``` | [Text](https://schema.org/Text "Text") | A sub property of description. A short description of the item used to disambiguate from other, similar items. Information from other properties (in particular, name) may be necessary for the description to be useful for disambiguation. |
| ``` identifier ``` | [PropertyValue](https://schema.org/PropertyValue "PropertyValue") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | The identifier property represents any kind of identifier for any kind of [Thing](https://schema.org/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](https://schema.org/docs/datamodel.html#identifierBg) for more details. |
| ``` image ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An image of the item. This can be a [URL](https://schema.org/URL) or a fully described [ImageObject](https://schema.org/ImageObject). |
| ``` mainEntityOfPage ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See [background notes](https://schema.org/docs/datamodel.html#mainEntityBackground) for details. Inverse property: [mainEntity](https://schema.org/mainEntity "mainEntity") |
| ``` name ``` | [Text](https://schema.org/Text "Text") | The name of the item. |
| ``` potentialAction ``` | [Action](https://schema.org/Action "Action") | Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role. |
| ``` sameAs ``` | [URL](https://schema.org/URL "URL") | URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website. |
| ``` subjectOf ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") | A CreativeWork or Event about this Thing. Inverse property: [about](https://schema.org/about "about") |
| ``` url ``` | [URL](https://schema.org/URL "URL") | URL of the item. |

Instances of [AggregateOffer](https://schema.org/AggregateOffer "AggregateOffer") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [itemOffered](https://schema.org/itemOffered "itemOffered") | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](https://schema.org/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |

### Examples
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
      "name": "Miami Heat at Philadelphia 76ers - Game 3 (Home Game 1)",
      "location": {
        "@type": "Place",
        "address": {
          "@type": "PostalAddress",
          "addressLocality": "Philadelphia",
          "addressRegion": "PA"
        },
        "url": "wells-fargo-center.html"
      },
      "offers": {
        "@type": "AggregateOffer",
        "priceCurrency": "USD",
        "lowPrice": "35",
        "offerCount": "1938"
      },
      "startDate": "2016-04-21T20:00",
      "url": "nba-miami-philidelphia-game3.html"
    }
    </script>
```