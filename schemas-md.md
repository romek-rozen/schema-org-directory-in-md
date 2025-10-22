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
```Title: Brand - Schema.org Type

URL Source: https://schema.org/Brand

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

A brand is a name used by an organization or business person for labeling a product, product group, or similar.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Brand](https://schema.org/Brand "Brand") |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
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

Instances of [Brand](https://schema.org/Brand "Brand") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [brand](https://schema.org/brand "brand") | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") or [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |

### Acknowledgements

GoodRelations Vocabulary Classes

This class is derived from the GoodRelations Vocabulary for E-Commerce, created by Martin Hepp. GoodRelations is a data model for sharing e-commerce data on the Web that can be expressed in a variety of syntaxes, including RDFa and HTML5 Microdata. More information about GoodRelations can be found at [http://purl.org/goodrelations/](http://purl.org/goodrelations/).
Title: CreativeWork - Schema.org Type

URL Source: https://schema.org/CreativeWork

Markdown Content:
# CreativeWork

A Schema.org Type

  [Thing](/Thing "Thing") \>   [CreativeWork](/CreativeWork "CreativeWork")  


*   Canonical URL: https://schema.org/CreativeWork
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+CreativeWork)

The most generic kind of creative work, including books, movies, photographs, software programs, etc.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [CreativeWork](/CreativeWork "CreativeWork") |     |     |
| `[about](/about "about")` | [Thing](/Thing "Thing") | The subject matter of the content.  <br>Inverse property: [subjectOf](/subjectOf "subjectOf") |
| `[abstract](/abstract "abstract")` | [Text](/Text "Text") | An abstract is a short description that summarizes a [CreativeWork](/CreativeWork). |
| `[accessMode](/accessMode "accessMode")` | [Text](/Text "Text") | The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessMode-vocabulary). |
| `[accessModeSufficient](/accessModeSufficient "accessModeSufficient")` | [ItemList](/ItemList "ItemList") | A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessModeSufficient-vocabulary). |
| `[accessibilityAPI](/accessibilityAPI "accessibilityAPI")` | [Text](/Text "Text") | Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityAPI-vocabulary). |
| `[accessibilityControl](/accessibilityControl "accessibilityControl")` | [Text](/Text "Text") | Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityControl-vocabulary). |
| `[accessibilityFeature](/accessibilityFeature "accessibilityFeature")` | [Text](/Text "Text") | Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityFeature-vocabulary). |
| `[accessibilityHazard](/accessibilityHazard "accessibilityHazard")` | [Text](/Text "Text") | A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityHazard-vocabulary). |
| `[accessibilitySummary](/accessibilitySummary "accessibilitySummary")` | [Text](/Text "Text") | A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed". |
| `[accountablePerson](/accountablePerson "accountablePerson")` | [Person](/Person "Person") | Specifies the Person that is legally accountable for the CreativeWork. |
| `[acquireLicensePage](/acquireLicensePage "acquireLicensePage")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item. |
| `[aggregateRating](/aggregateRating "aggregateRating")` | [AggregateRating](/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| `[alternativeHeadline](/alternativeHeadline "alternativeHeadline")` | [Text](/Text "Text") | A secondary title of the CreativeWork. |
| `[archivedAt](/archivedAt "archivedAt")` | [URL](/URL "URL")  or  <br>[WebPage](/WebPage "WebPage") | Indicates a page or other link involved in archival of a [CreativeWork](/CreativeWork). In the case of [MediaReview](/MediaReview), the items in a [MediaReviewItem](/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content. |
| `[assesses](/assesses "assesses")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The item being described is intended to assess the competency or learning outcome defined by the referenced term. |
| `[associatedMedia](/associatedMedia "associatedMedia")` | [MediaObject](/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for encoding. |
| `[audience](/audience "audience")` | [Audience](/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](/serviceAudience "serviceAudience"). |
| `[audio](/audio "audio")` | [AudioObject](/AudioObject "AudioObject")  or  <br>[Clip](/Clip "Clip")  or  <br>[MusicRecording](/MusicRecording "MusicRecording") | An embedded audio object. |
| `[author](/author "author")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| `[award](/award "award")` | [Text](/Text "Text") | An award won by or for this item. Supersedes [awards](/awards "awards"). |
| `[character](/character "character")` | [Person](/Person "Person") | Fictional person connected with a creative work. |
| `[citation](/citation "citation")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Text](/Text "Text") | A citation or reference to another creative work, such as another publication, web page, scholarly article, etc. |
| `[comment](/comment "comment")` | [Comment](/Comment "Comment") | Comments, typically from users. |
| `[commentCount](/commentCount "commentCount")` | [Integer](/Integer "Integer") | The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere. |
| `[conditionsOfAccess](/conditionsOfAccess "conditionsOfAccess")` | [Text](/Text "Text") | Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an [ArchiveComponent](/ArchiveComponent) held by an [ArchiveOrganization](/ArchiveOrganization). This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language.  <br>  <br>For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts ". |
| `[contentLocation](/contentLocation "contentLocation")` | [Place](/Place "Place") | The location depicted or described in the content. For example, the location in a photograph or painting. |
| `[contentRating](/contentRating "contentRating")` | [Rating](/Rating "Rating")  or  <br>[Text](/Text "Text") | Official rating of a piece of content—for example, 'MPAA PG-13'. |
| `[contentReferenceTime](/contentReferenceTime "contentReferenceTime")` | [DateTime](/DateTime "DateTime") | The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event. |
| `[contributor](/contributor "contributor")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A secondary contributor to the CreativeWork or Event. |
| `[copyrightHolder](/copyrightHolder "copyrightHolder")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The party holding the legal copyright to the CreativeWork. |
| `[copyrightNotice](/copyrightNotice "copyrightNotice")` | [Text](/Text "Text") | Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work. |
| `[copyrightYear](/copyrightYear "copyrightYear")` | [Number](/Number "Number") | The year during which the claimed copyright for the CreativeWork was first asserted. |
| `[correction](/correction "correction")` | [CorrectionComment](/CorrectionComment "CorrectionComment")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | Indicates a correction to a [CreativeWork](/CreativeWork), either via a [CorrectionComment](/CorrectionComment), textually or in another document. |
| `[countryOfOrigin](/countryOfOrigin "countryOfOrigin")` | [Country](/Country "Country") | The country of origin of something, including products as well as creative works such as movie and TV content.  <br>  <br>In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](/contentLocation) and [locationCreated](/locationCreated) may be more applicable.  <br>  <br>In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here. |
| `[creativeWorkStatus](/creativeWorkStatus "creativeWorkStatus")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle. |
| `[creator](/creator "creator")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| `[creditText](/creditText "creditText")` | [Text](/Text "Text") | Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work. |
| `[dateCreated](/dateCreated "dateCreated")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The date on which the CreativeWork was created or the item was added to a DataFeed. |
| `[dateModified](/dateModified "dateModified")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed. |
| `[datePublished](/datePublished "datePublished")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | Date of first publication or broadcast. For example the date a [CreativeWork](/CreativeWork) was broadcast or a [Certification](/Certification) was issued. |
| `[digitalSourceType](/digitalSourceType "digitalSourceType")` | [IPTCDigitalSourceEnumeration](/IPTCDigitalSourceEnumeration "IPTCDigitalSourceEnumeration") | Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some [CreativeWork](/CreativeWork). |
| `[discussionUrl](/discussionUrl "discussionUrl")` | [URL](/URL "URL") | A link to the page containing the comments of the CreativeWork. |
| `[editEIDR](/editEIDR "editEIDR")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | An [EIDR](https://eidr.org/) (Entertainment Identifier Registry) [identifier](/identifier) representing a specific edit / edition for a work of film or television.  <br>  <br>For example, the motion picture known as "Ghostbusters" whose [titleEIDR](/titleEIDR) is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3".  <br>  <br>Since schema.org types like [Movie](/Movie) and [TVEpisode](/TVEpisode) can be used for both works and their multiple expressions, it is possible to use [titleEIDR](/titleEIDR) alone (for a general description), or alongside [editEIDR](/editEIDR) for a more edit-specific description. |
| `[editor](/editor "editor")` | [Person](/Person "Person") | Specifies the Person who edited the CreativeWork. |
| `[educationalAlignment](/educationalAlignment "educationalAlignment")` | [AlignmentObject](/AlignmentObject "AlignmentObject") | An alignment to an established educational framework.  <br>  <br>This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource [teaches](/teaches) or [assesses](/assesses) a competency. |
| `[educationalLevel](/educationalLevel "educationalLevel")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators. |
| `[educationalUse](/educationalUse "educationalUse")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The purpose of a work in the context of education; for example, 'assignment', 'group work'. |
| `[encoding](/encoding "encoding")` | [MediaObject](/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes [encodings](/encodings "encodings").  <br>Inverse property: [encodesCreativeWork](/encodesCreativeWork "encodesCreativeWork") |
| `[encodingFormat](/encodingFormat "encodingFormat")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | Media type typically expressed using a MIME format (see [IANA site](http://www.iana.org/assignments/media-types/media-types.xhtml) and [MDN reference](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc.  <br>  <br>In cases where a [CreativeWork](/CreativeWork) has several media type representations, [encoding](/encoding) can be used to indicate each [MediaObject](/MediaObject) alongside particular [encodingFormat](/encodingFormat) information.  <br>  <br>Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes [fileFormat](/fileFormat "fileFormat"). |
| `[exampleOfWork](/exampleOfWork "exampleOfWork")` | [CreativeWork](/CreativeWork "CreativeWork") | A creative work that this work is an example/instance/realization/derivation of.  <br>Inverse property: [workExample](/workExample "workExample") |
| `[expires](/expires "expires")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | Date the content expires and is no longer useful or available. For example a [VideoObject](/VideoObject) or [NewsArticle](/NewsArticle) whose availability or relevance is time-limited, a [ClaimReview](/ClaimReview) fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a [Certification](/Certification) the validity has expired. |
| `[funder](/funder "funder")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| `[funding](/funding "funding")` | [Grant](/Grant "Grant") | A [Grant](/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](/ownershipFundingInfo).  <br>Inverse property: [fundedItem](/fundedItem "fundedItem") |
| `[genre](/genre "genre")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | Genre of the creative work, broadcast channel or group. |
| `[hasPart](/hasPart "hasPart")` | [CreativeWork](/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).  <br>Inverse property: [isPartOf](/isPartOf "isPartOf") |
| `[headline](/headline "headline")` | [Text](/Text "Text") | Headline of the article. |
| `[inLanguage](/inLanguage "inLanguage")` | [Language](/Language "Language")  or  <br>[Text](/Text "Text") | The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](/availableLanguage). Supersedes [language](/language "language"). |
| `[interactionStatistic](/interactionStatistic "interactionStatistic")` | [InteractionCounter](/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](/interactionCount "interactionCount"). |
| `[interactivityType](/interactivityType "interactivityType")` | [Text](/Text "Text") | The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'. |
| `[interpretedAsClaim](/interpretedAsClaim "interpretedAsClaim")` | [Claim](/Claim "Claim") | Used to indicate a specific claim contained, implied, translated or refined from the content of a [MediaObject](/MediaObject) or other [CreativeWork](/CreativeWork). The interpreting party can be indicated using [claimInterpreter](/claimInterpreter). |
| `[isAccessibleForFree](/isAccessibleForFree "isAccessibleForFree")` | [Boolean](/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](/free "free"). |
| `[isBasedOn](/isBasedOn "isBasedOn")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Product](/Product "Product")  or  <br>[URL](/URL "URL") | A resource from which this work is derived or from which it is a modification or adaptation. Supersedes [isBasedOnUrl](/isBasedOnUrl "isBasedOnUrl"). |
| `[isFamilyFriendly](/isFamilyFriendly "isFamilyFriendly")` | [Boolean](/Boolean "Boolean") | Indicates whether this content is family friendly. |
| `[isPartOf](/isPartOf "isPartOf")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.  <br>Inverse property: [hasPart](/hasPart "hasPart") |
| `[keywords](/keywords "keywords")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| `[learningResourceType](/learningResourceType "learningResourceType")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'. |
| `[license](/license "license")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | A license document that applies to this content, typically indicated by URL. |
| `[locationCreated](/locationCreated "locationCreated")` | [Place](/Place "Place") | The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork. |
| `[mainEntity](/mainEntity "mainEntity")` | [Thing](/Thing "Thing") | Indicates the primary entity described in some page or other CreativeWork.  <br>Inverse property: [mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage") |
| `[maintainer](/maintainer "maintainer")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A maintainer of a [Dataset](/Dataset), software package ([SoftwareApplication](/SoftwareApplication)), or other [Project](/Project). A maintainer is a [Person](/Person) or [Organization](/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| `[material](/material "material")` | [Product](/Product "Product")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| `[materialExtent](/materialExtent "materialExtent")` | [QuantitativeValue](/QuantitativeValue "QuantitativeValue")  or  <br>[Text](/Text "Text") | The quantity of the materials being described or an expression of the physical space they occupy. |
| `[mentions](/mentions "mentions")` | [Thing](/Thing "Thing") | Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept. |
| `[offers](/offers "offers")` | [Demand](/Demand "Demand")  or  <br>[Offer](/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer.  <br>Inverse property: [itemOffered](/itemOffered "itemOffered") |
| `[pattern](/pattern "pattern")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported. |
| `[position](/position "position")` | [Integer](/Integer "Integer")  or  <br>[Text](/Text "Text") | The position of an item in a series or sequence of items. |
| `[producer](/producer "producer")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| `[provider](/provider "provider")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](/carrier "carrier"). |
| `[publication](/publication "publication")` | [PublicationEvent](/PublicationEvent "PublicationEvent") | A publication event associated with the item. |
| `[publisher](/publisher "publisher")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The publisher of the article in question. |
| `[publisherImprint](/publisherImprint "publisherImprint")` | [Organization](/Organization "Organization") | The publishing division which published the comic. |
| `[publishingPrinciples](/publishingPrinciples "publishingPrinciples")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | The publishingPrinciples property indicates (typically via [URL](/URL)) a document describing the editorial principles of an [Organization](/Organization) (or individual, e.g. a [Person](/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](/CreativeWork) (e.g. [NewsArticle](/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](/CreativeWork).  <br>  <br>While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](/funder)) can be expressed using schema.org terminology. |
| `[recordedAt](/recordedAt "recordedAt")` | [Event](/Event "Event") | The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event.  <br>Inverse property: [recordedIn](/recordedIn "recordedIn") |
| `[releasedEvent](/releasedEvent "releasedEvent")` | [PublicationEvent](/PublicationEvent "PublicationEvent") | The place and time the release was issued, expressed as a PublicationEvent. |
| `[review](/review "review")` | [Review](/Review "Review") | A review of the item. Supersedes [reviews](/reviews "reviews"). |
| `[schemaVersion](/schemaVersion "schemaVersion")` | [Text](/Text "Text")  or  <br>[URL](/URL "URL") | Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. `10.0` as a simple string, or more explicitly via URL, `https://schema.org/docs/releases.html#v10.0`. There may be situations in which other schemas might usefully be referenced this way, e.g. `http://dublincore.org/specifications/dublin-core/dces/1999-07-02/` but this has not been carefully explored in the community. |
| `[sdDatePublished](/sdDatePublished "sdDatePublished")` | [Date](/Date "Date") | Indicates the date on which the current structured data was generated / published. Typically used alongside [sdPublisher](/sdPublisher). |
| `[sdLicense](/sdLicense "sdLicense")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | A license document that applies to this structured data, typically indicated by URL. |
| `[sdPublisher](/sdPublisher "sdPublisher")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](/sdPublisher) property helps make such practices more explicit. |
| `[size](/size "size")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue")  or  <br>[SizeSpecification](/SizeSpecification "SizeSpecification")  or  <br>[Text](/Text "Text") | A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](/SizeSpecification); in other cases, the [width](/width), [height](/height), [depth](/depth) and [weight](/weight) properties may be more applicable. |
| `[sourceOrganization](/sourceOrganization "sourceOrganization")` | [Organization](/Organization "Organization") | The Organization on whose behalf the creator was working. |
| `[spatial](/spatial "spatial")` | [Place](/Place "Place") | The "spatial" property can be used in cases when more specific properties (e.g. [locationCreated](/locationCreated), [spatialCoverage](/spatialCoverage), [contentLocation](/contentLocation)) are not known to be appropriate. |
| `[spatialCoverage](/spatialCoverage "spatialCoverage")` | [Place](/Place "Place") | The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York. |
| `[sponsor](/sponsor "sponsor")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| `[teaches](/teaches "teaches")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term. |
| `[temporal](/temporal "temporal")` | [DateTime](/DateTime "DateTime")  or  <br>[Text](/Text "Text") | The "temporal" property can be used in cases where more specific properties (e.g. [temporalCoverage](/temporalCoverage), [dateCreated](/dateCreated), [dateModified](/dateModified), [datePublished](/datePublished)) are not known to be appropriate. |
| `[temporalCoverage](/temporalCoverage "temporalCoverage")` | [DateTime](/DateTime "DateTime")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in [ISO 8601 time interval format](https://en.wikipedia.org/wiki/ISO_8601#Time_intervals). In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945".  <br>  <br>Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes [datasetTimeInterval](/datasetTimeInterval "datasetTimeInterval"). |
| `[text](/text "text")` | [Text](/Text "Text") | The textual content of this CreativeWork. |
| `[thumbnail](/thumbnail "thumbnail")` | [ImageObject](/ImageObject "ImageObject") | Thumbnail image for an image or video. |
| `[thumbnailUrl](/thumbnailUrl "thumbnailUrl")` | [URL](/URL "URL") | A thumbnail image relevant to the Thing. |
| `[timeRequired](/timeRequired "timeRequired")` | [Duration](/Duration "Duration") | Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience. |
| `[translationOfWork](/translationOfWork "translationOfWork")` | [CreativeWork](/CreativeWork "CreativeWork") | The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”.  <br>Inverse property: [workTranslation](/workTranslation "workTranslation") |
| `[translator](/translator "translator")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| `[typicalAgeRange](/typicalAgeRange "typicalAgeRange")` | [Text](/Text "Text") | The typical expected age range, e.g. '7-9', '11-'. |
| `[usageInfo](/usageInfo "usageInfo")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | The schema.org [usageInfo](/usageInfo) property indicates further information about a [CreativeWork](/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options.  <br>  <br>This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses. |
| `[version](/version "version")` | [Number](/Number "Number")  or  <br>[Text](/Text "Text") | The version of the CreativeWork embodied by a specified resource. |
| `[video](/video "video")` | [Clip](/Clip "Clip")  or  <br>[VideoObject](/VideoObject "VideoObject") | An embedded video object. |
| `[wordCount](/wordCount "wordCount")` | [Integer](/Integer "Integer") | The number of words in the text of the CreativeWork such as an Article, Book, etc. |
| `[workExample](/workExample "workExample")` | [CreativeWork](/CreativeWork "CreativeWork") | Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book.  <br>Inverse property: [exampleOfWork](/exampleOfWork "exampleOfWork") |
| `[workTranslation](/workTranslation "workTranslation")` | [CreativeWork](/CreativeWork "CreativeWork") | A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo.  <br>Inverse property: [translationOfWork](/translationOfWork "translationOfWork") |
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

  

Instances of [CreativeWork](/CreativeWork "CreativeWork") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [acquireLicensePage](/acquireLicensePage "acquireLicensePage") | [CreativeWork](/CreativeWork "CreativeWork") | Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item. |
| [actionableFeedbackPolicy](/actionableFeedbackPolicy "actionableFeedbackPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | For a [NewsMediaOrganization](/NewsMediaOrganization) or other news-related [Organization](/Organization), a statement about public engagement activities (for news media, the newsroom’s), including involving the public - digitally or otherwise -- in coverage decisions, reporting and activities after publication. |
| [appearance](/appearance "appearance") | [Claim](/Claim "Claim") | Indicates an occurrence of a [Claim](/Claim) in some [CreativeWork](/CreativeWork). |
| [backstory](/backstory "backstory") | [Article](/Article "Article") | For an [Article](/Article), typically a [NewsArticle](/NewsArticle), the backstory property provides a textual summary giving a brief explanation of why and how an article was created. In a journalistic setting this could include information about reporting process, methods, interviews, data sources, etc. |
| [cheatCode](/cheatCode "cheatCode") | [VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries") | Cheat codes to the game. |
| [citation](/citation "citation") | [CreativeWork](/CreativeWork "CreativeWork") | A citation or reference to another creative work, such as another publication, web page, scholarly article, etc. |
| [correctionsPolicy](/correctionsPolicy "correctionsPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | For an [Organization](/Organization) (e.g. [NewsMediaOrganization](/NewsMediaOrganization)), a statement describing (in news media, the newsroom’s) disclosure and correction policy for errors. |
| [discusses](/discusses "discusses") | [UserComments](/UserComments "UserComments") | Specifies the CreativeWork associated with the UserComment. |
| [diversityPolicy](/diversityPolicy "diversityPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | Statement on diversity policy by an [Organization](/Organization) e.g. a [NewsMediaOrganization](/NewsMediaOrganization). For a [NewsMediaOrganization](/NewsMediaOrganization), a statement describing the newsroom’s diversity policy on both staffing and sources, typically providing staffing data. |
| [documentation](/documentation "documentation") | [WebAPI](/WebAPI "WebAPI") | Further documentation describing the Web API in more detail. |
| [encodesCreativeWork](/encodesCreativeWork "encodesCreativeWork") | [MediaObject](/MediaObject "MediaObject") | The CreativeWork encoded by this media object. |
| [ethicsPolicy](/ethicsPolicy "ethicsPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | Statement about ethics policy, e.g. of a [NewsMediaOrganization](/NewsMediaOrganization) regarding journalistic and publishing practices, or of a [Restaurant](/Restaurant), a page describing food source policies. In the case of a [NewsMediaOrganization](/NewsMediaOrganization), an ethicsPolicy is typically a statement describing the personal, organizational, and corporate standards of behavior expected by the organization. |
| [exampleOfWork](/exampleOfWork "exampleOfWork") | [CreativeWork](/CreativeWork "CreativeWork") | A creative work that this work is an example/instance/realization/derivation of. |
| [firstAppearance](/firstAppearance "firstAppearance") | [Claim](/Claim "Claim") | Indicates the first known occurrence of a [Claim](/Claim) in some [CreativeWork](/CreativeWork). |
| [fundedItem](/fundedItem "fundedItem") | [Grant](/Grant "Grant") | Indicates something directly or indirectly funded or sponsored through a [Grant](/Grant). See also [ownershipFundingInfo](/ownershipFundingInfo). |
| [gameTip](/gameTip "gameTip") | [VideoGame](/VideoGame "VideoGame") | Links to tips, tactics, etc. |
| [hasPart](/hasPart "hasPart") | [CreativeWork](/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense). |
| [isBasedOn](/isBasedOn "isBasedOn") | [CreativeWork](/CreativeWork "CreativeWork") | A resource from which this work is derived or from which it is a modification or adaptation. |
| [isBasedOnUrl](/isBasedOnUrl "isBasedOnUrl") | [CreativeWork](/CreativeWork "CreativeWork") | A resource that was used in the creation of this resource. This term can be repeated for multiple sources. For example, http://example.com/great-multiplication-intro.html. |
| [isPartOf](/isPartOf "isPartOf") | [CreativeWork](/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of. |
| [itemOffered](/itemOffered "itemOffered") | [Demand](/Demand "Demand")  or  <br>[Offer](/Offer "Offer") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |
| [license](/license "license") | [CreativeWork](/CreativeWork "CreativeWork") | A license document that applies to this content, typically indicated by URL. |
| [lyrics](/lyrics "lyrics") | [MusicComposition](/MusicComposition "MusicComposition") | The words in the song. |
| [mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage") | [Thing](/Thing "Thing") | Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See [background notes](/docs/datamodel.html#mainEntityBackground) for details. |
| [masthead](/masthead "masthead") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization") | For a [NewsMediaOrganization](/NewsMediaOrganization), a link to the masthead page or a page listing top editorial management. |
| [messageAttachment](/messageAttachment "messageAttachment") | [Message](/Message "Message") | A CreativeWork attached to the message. |
| [missionCoveragePrioritiesPolicy](/missionCoveragePrioritiesPolicy "missionCoveragePrioritiesPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization") | For a [NewsMediaOrganization](/NewsMediaOrganization), a statement on coverage priorities, including any public agenda or stance on issues. |
| [noBylinesPolicy](/noBylinesPolicy "noBylinesPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization") | For a [NewsMediaOrganization](/NewsMediaOrganization) or other news-related [Organization](/Organization), a statement explaining when authors of articles are not named in bylines. |
| [ownershipFundingInfo](/ownershipFundingInfo "ownershipFundingInfo") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | For an [Organization](/Organization) (often but not necessarily a [NewsMediaOrganization](/NewsMediaOrganization)), a description of organizational ownership structure; funding and grants. In a news/media setting, this is with particular reference to editorial independence. Note that the [funder](/funder) is also available and can be used to make basic funder information machine-readable. |
| [parentItem](/parentItem "parentItem") | [Answer](/Answer "Answer")  or  <br>[Comment](/Comment "Comment")  or  <br>[Question](/Question "Question") | The parent of a question, answer or item in general. Typically used for Q/A discussion threads e.g. a chain of comments with the first comment being an [Article](/Article) or other [CreativeWork](/CreativeWork). See also [comment](/comment) which points from something to a comment about it. |
| [publishingPrinciples](/publishingPrinciples "publishingPrinciples") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The publishingPrinciples property indicates (typically via [URL](/URL)) a document describing the editorial principles of an [Organization](/Organization) (or individual, e.g. a [Person](/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](/CreativeWork) (e.g. [NewsArticle](/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](/CreativeWork).  <br>  <br>While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](/funder)) can be expressed using schema.org terminology. |
| [recipeInstructions](/recipeInstructions "recipeInstructions") | [Recipe](/Recipe "Recipe") | A step in making the recipe, in the form of a single item (document, video, etc.) or an ordered list with HowToStep and/or HowToSection items. |
| [recordedIn](/recordedIn "recordedIn") | [Event](/Event "Event") | The CreativeWork that captured all or part of this Event. |
| [sdLicense](/sdLicense "sdLicense") | [CreativeWork](/CreativeWork "CreativeWork") | A license document that applies to this structured data, typically indicated by URL. |
| [sharedContent](/sharedContent "sharedContent") | [Comment](/Comment "Comment")  or  <br>[SocialMediaPosting](/SocialMediaPosting "SocialMediaPosting") | A CreativeWork such as an image, video, or audio clip shared as part of this posting. |
| [softwareHelp](/softwareHelp "softwareHelp") | [SoftwareApplication](/SoftwareApplication "SoftwareApplication") | Software application help. |
| [step](/step "step") | [HowTo](/HowTo "HowTo") | A single step item (as HowToStep, text, document, video, etc.) or a HowToSection. |
| [steps](/steps "steps") | [HowTo](/HowTo "HowTo")  or  <br>[HowToSection](/HowToSection "HowToSection") | A single step item (as HowToStep, text, document, video, etc.) or a HowToSection (originally misnamed 'steps'; 'step' is preferred). |
| [subjectOf](/subjectOf "subjectOf") | [Thing](/Thing "Thing") | A CreativeWork or Event about this Thing. |
| [translationOfWork](/translationOfWork "translationOfWork") | [CreativeWork](/CreativeWork "CreativeWork") | The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”. |
| [unnamedSourcesPolicy](/unnamedSourcesPolicy "unnamedSourcesPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization")  or  <br>[Organization](/Organization "Organization") | For an [Organization](/Organization) (typically a [NewsMediaOrganization](/NewsMediaOrganization)), a statement about policy on use of unnamed sources and the decision process required. |
| [usageInfo](/usageInfo "usageInfo") | [CreativeWork](/CreativeWork "CreativeWork") | The schema.org [usageInfo](/usageInfo) property indicates further information about a [CreativeWork](/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options.  <br>  <br>This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses. |
| [verificationFactCheckingPolicy](/verificationFactCheckingPolicy "verificationFactCheckingPolicy") | [NewsMediaOrganization](/NewsMediaOrganization "NewsMediaOrganization") | Disclosure about verification and fact-checking processes for a [NewsMediaOrganization](/NewsMediaOrganization) or other fact-checking [Organization](/Organization). |
| [workExample](/workExample "workExample") | [CreativeWork](/CreativeWork "CreativeWork") | Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book. |
| [workFeatured](/workFeatured "workFeatured") | [Event](/Event "Event") | A work featured in some event, e.g. exhibited in an ExhibitionEvent. Specific subproperties are available for workPerformed (e.g. a play), or a workPresented (a Movie at a ScreeningEvent). |
| [workPerformed](/workPerformed "workPerformed") | [Event](/Event "Event") | A work performed in some event, for example a play performed in a TheaterEvent. |
| [workTranslation](/workTranslation "workTranslation") | [CreativeWork](/CreativeWork "CreativeWork") | A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo. |

  

#### More specific Types

*   [AmpStory](/AmpStory "AmpStory")
*   [ArchiveComponent](/ArchiveComponent "ArchiveComponent")
*   [Article](/Article "Article")
*   [Atlas](/Atlas "Atlas")
*   [Blog](/Blog "Blog")
*   [Book](/Book "Book")
*   [Certification](/Certification "Certification")
*   [Chapter](/Chapter "Chapter")
*   [Claim](/Claim "Claim")
*   [Clip](/Clip "Clip")
*   [Collection](/Collection "Collection")
*   [ComicStory](/ComicStory "ComicStory")
*   [Comment](/Comment "Comment")
*   [Conversation](/Conversation "Conversation")
*   [Course](/Course "Course")
*   [CreativeWorkSeason](/CreativeWorkSeason "CreativeWorkSeason")
*   [CreativeWorkSeries](/CreativeWorkSeries "CreativeWorkSeries")
*   [DataCatalog](/DataCatalog "DataCatalog")
*   [Dataset](/Dataset "Dataset")
*   [DefinedTermSet](/DefinedTermSet "DefinedTermSet")
*   [Diet](/Diet "Diet")
*   [DigitalDocument](/DigitalDocument "DigitalDocument")
*   [Drawing](/Drawing "Drawing")
*   [EducationalOccupationalCredential](/EducationalOccupationalCredential "EducationalOccupationalCredential")
*   [Episode](/Episode "Episode")
*   [ExercisePlan](/ExercisePlan "ExercisePlan")
*   [Game](/Game "Game")
*   [Guide](/Guide "Guide")
*   [HowTo](/HowTo "HowTo")
*   [HowToDirection](/HowToDirection "HowToDirection")
*   [HowToSection](/HowToSection "HowToSection")
*   [HowToStep](/HowToStep "HowToStep")
*   [HowToTip](/HowToTip "HowToTip")
*   [HyperToc](/HyperToc "HyperToc")
*   [HyperTocEntry](/HyperTocEntry "HyperTocEntry")
*   [LearningResource](/LearningResource "LearningResource")
*   [Legislation](/Legislation "Legislation")
*   [Manuscript](/Manuscript "Manuscript")
*   [Map](/Map "Map")
*   [MathSolver](/MathSolver "MathSolver")
*   [MediaObject](/MediaObject "MediaObject")
*   [MediaReviewItem](/MediaReviewItem "MediaReviewItem")
*   [Menu](/Menu "Menu")
*   [MenuSection](/MenuSection "MenuSection")
*   [Message](/Message "Message")
*   [Movie](/Movie "Movie")
*   [MusicComposition](/MusicComposition "MusicComposition")
*   [MusicPlaylist](/MusicPlaylist "MusicPlaylist")
*   [MusicRecording](/MusicRecording "MusicRecording")
*   [Painting](/Painting "Painting")
*   [Photograph](/Photograph "Photograph")
*   [Play](/Play "Play")
*   [Poster](/Poster "Poster")
*   [PublicationIssue](/PublicationIssue "PublicationIssue")
*   [PublicationVolume](/PublicationVolume "PublicationVolume")
*   [Quotation](/Quotation "Quotation")
*   [Review](/Review "Review")
*   [Sculpture](/Sculpture "Sculpture")
*   [SheetMusic](/SheetMusic "SheetMusic")
*   [ShortStory](/ShortStory "ShortStory")
*   [SoftwareApplication](/SoftwareApplication "SoftwareApplication")
*   [SoftwareSourceCode](/SoftwareSourceCode "SoftwareSourceCode")
*   [SpecialAnnouncement](/SpecialAnnouncement "SpecialAnnouncement")
*   [Statement](/Statement "Statement")
*   [TVSeason](/TVSeason "TVSeason")
*   [TVSeries](/TVSeries "TVSeries")
*   [Thesis](/Thesis "Thesis")
*   [VisualArtwork](/VisualArtwork "VisualArtwork")
*   [WebContent](/WebContent "WebContent")
*   [WebPage](/WebPage "WebPage")
*   [WebPageElement](/WebPageElement "WebPageElement")
*   [WebSite](/WebSite "WebSite")

### Acknowledgements

IPTC rNews properties

This class contains derivatives of IPTC rNews properties. rNews is a data model of publishing metadata with serializations currently available for RDFa as well as HTML5 Microdata. More information about the IPTC and rNews can be found at [rnews.org](http://rnews.org).

### Examples

```json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "CreativeWork",
      "author": "Sony",
      "contentRating": "Mature",
      "image": "videogame.jpg",
      "name": "Resistance 3: Fall of Man"
    }
    </script>
```

```json
        <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Book",
      "accessibilityAPI": "ARIA",
      "accessibilityControl": [
        "fullKeyboardControl",
        "fullMouseControl"
      ],
      "accessibilityFeature": [
        "largePrint/CSSEnabled",
        "highContrast/CSSEnabled",
        "resizeText/CSSEnabled",
        "displayTransformability",
        "longDescription",
        "alternativeText"
      ],
      "accessibilityHazard": [
        "noFlashingHazard",
        "noMotionSimulationHazard",
        "noSoundHazard"
      ],
      "aggregateRating": {
        "@type": "AggregateRating",
        "reviewCount": "0"
      },
      "bookFormat": "EBook/DAISY3",
      "copyrightHolder": {
        "@type": "Organization",
        "name": "Holt, Rinehart and Winston"
      },
      "copyrightYear": "2007",
      "description": "NIMAC-sourced textbook",
      "genre": "Educational Materials",
      "inLanguage": "en-US",
      "isFamilyFriendly": "true",
      "isbn": "9780030426599",
      "name": "Holt Physical Science",
      "numberOfPages": "598",
      "publisher": {
        "@type": "Organization",
        "name": "Holt, Rinehart and Winston"
      }
    }
    </script>
```

```json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "MusicEvent",
      "location": {
        "@type": "MusicVenue",
        "name": "Chicago Symphony Center",
        "address": "220 S. Michigan Ave, Chicago, Illinois, USA"
      },
      "name": "Shostakovich Leningrad",
      "offers": {
        "@type": "Offer",
        "url": "/examples/ticket/12341234",
        "price": "40",
        "priceCurrency": "USD",
        "availability": "https://schema.org/InStock"
      },
      "performer": [
        {
          "@type": "MusicGroup",
          "name": "Chicago Symphony Orchestra",
          "sameAs": [
            "http://cso.org/",
            "http://en.wikipedia.org/wiki/Chicago_Symphony_Orchestra"
          ]
        },
        {
          "@type": "Person",
          "image": "/examples/jvanzweden_s.jpg",
          "name": "Jaap van Zweden",
          "sameAs": "http://www.jaapvanzweden.com/"
        }
      ],
      "startDate": "2014-05-23T20:00",
      "workPerformed": [
        {
          "@type": "CreativeWork",
          "name": "Britten Four Sea Interludes and Passacaglia from Peter Grimes",
          "sameAs": "http://en.wikipedia.org/wiki/Peter_Grimes"
        },
        {
          "@type": "CreativeWork",
          "name": "Shostakovich Symphony No. 7 (Leningrad)",
          "sameAs": "http://en.wikipedia.org/wiki/Symphony_No._7_(Shostakovich)"
        }
      ]
    }
    </script>
```

```json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebPage",
      "breadcrumb": "Books > Literature & Fiction > Classics",
      "mainEntity":{
              "@type": "Book",
              "author": "/author/jd_salinger.html",
              "bookFormat": "https://schema.org/Paperback",
              "datePublished": "1991-05-01",
              "image": "catcher-in-the-rye-book-cover.jpg",
              "inLanguage": "English",
              "isbn": "0316769487",
              "name": "The Catcher in the Rye",
              "numberOfPages": "224",
              "offers": {
                "@type": "Offer",
                "availability": "https://schema.org/InStock",
                "price": "6.99",
                "priceCurrency": "USD"
              },
              "publisher": "Little, Brown, and Company",
              "aggregateRating": {
                "@type": "AggregateRating",
                "ratingValue": "4",
                "reviewCount": "3077"
              },
              "review": [
                {
                  "@type": "Review",
                  "author": "John Doe",
                  "datePublished": "2006-05-04",
                  "name": "A masterpiece of literature",
                  "reviewBody": "I really enjoyed this book. It captures the essential challenge people face as they try make sense of their lives and grow to adulthood.",
                  "reviewRating": {
                "@type": "Rating",
                "ratingValue": "5"
               }
                },
                {
                  "@type": "Review",
                  "author": "Bob Smith",
                  "datePublished": "2006-06-15",
                  "name": "A good read.",
                  "reviewBody": "Catcher in the Rye is a fun book. It's a good book to read.",
                  "reviewRating": "4"
                }
              ]
            }
    }
    </script>
```Title: Event - Schema.org Type

URL Source: https://schema.org/Event

Markdown Content:


# Event

A Schema.org Type

  [Thing](/Thing "Thing") \>   [Event](/Event "Event")  

**\[more...\]**

*   Canonical URL: https://schema.org/Event
*   Equivalent Class: dcmitype:Event
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+Event)

An event happening at a certain time and location, such as a concert, lecture, or festival. Ticketing information may be added via the [offers](/offers) property. Repeated events may be structured as separate Event objects.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Event](/Event "Event") |     |     |
| `[about](/about "about")` | [Thing](/Thing "Thing") | The subject matter of the content.  <br>Inverse property: [subjectOf](/subjectOf "subjectOf") |
| `[actor](/actor "actor")` | [PerformingGroup](/PerformingGroup "PerformingGroup")  or  <br>[Person](/Person "Person") | An actor (individual or a group), e.g. in TV, radio, movie, video games etc., or in an event. Actors can be associated with individual items or with a series, episode, clip. Supersedes [actors](/actors "actors"). |
| `[aggregateRating](/aggregateRating "aggregateRating")` | [AggregateRating](/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| `[attendee](/attendee "attendee")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization attending the event. Supersedes [attendees](/attendees "attendees"). |
| `[audience](/audience "audience")` | [Audience](/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](/serviceAudience "serviceAudience"). |
| `[composer](/composer "composer")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | The person or organization who wrote a composition, or who is the composer of a work performed at some event. |
| `[contributor](/contributor "contributor")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A secondary contributor to the CreativeWork or Event. |
| `[director](/director "director")` | [Person](/Person "Person") | A director of e.g. TV, radio, movie, video gaming etc. content, or of an event. Directors can be associated with individual items or with a series, episode, clip. Supersedes [directors](/directors "directors"). |
| `[doorTime](/doorTime "doorTime")` | [DateTime](/DateTime "DateTime")  or  <br>[Time](/Time "Time") | The time admission will commence. |
| `[duration](/duration "duration")` | [Duration](/Duration "Duration")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The duration of the item (movie, audio recording, event, etc.) in [ISO 8601 duration format](http://en.wikipedia.org/wiki/ISO_8601). |
| `[endDate](/endDate "endDate")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The end date and time of the item (in [ISO 8601 date format](http://en.wikipedia.org/wiki/ISO_8601)). |
| `[eventAttendanceMode](/eventAttendanceMode "eventAttendanceMode")` | [EventAttendanceModeEnumeration](/EventAttendanceModeEnumeration "EventAttendanceModeEnumeration") | The eventAttendanceMode of an event indicates whether it occurs online, offline, or a mix. |
| `[eventSchedule](/eventSchedule "eventSchedule")` | [Schedule](/Schedule "Schedule") | Associates an [Event](/Event) with a [Schedule](/Schedule). There are circumstances where it is preferable to share a schedule for a series of repeating events rather than data on the individual events themselves. For example, a website or application might prefer to publish a schedule for a weekly gym class rather than provide data on every event. A schedule could be processed by applications to add forthcoming events to a calendar. An [Event](/Event) that is associated with a [Schedule](/Schedule) using this property should not have [startDate](/startDate) or [endDate](/endDate) properties. These are instead defined within the associated [Schedule](/Schedule), this avoids any ambiguity for clients using the data. The property might have repeated values to specify different schedules, e.g. for different months or seasons. |
| `[eventStatus](/eventStatus "eventStatus")` | [EventStatusType](/EventStatusType "EventStatusType") | An eventStatus of an event represents its status; particularly useful when an event is cancelled or rescheduled. |
| `[funder](/funder "funder")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| `[funding](/funding "funding")` | [Grant](/Grant "Grant") | A [Grant](/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](/ownershipFundingInfo).  <br>Inverse property: [fundedItem](/fundedItem "fundedItem") |
| `[inLanguage](/inLanguage "inLanguage")` | [Language](/Language "Language")  or  <br>[Text](/Text "Text") | The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](/availableLanguage). Supersedes [language](/language "language"). |
| `[isAccessibleForFree](/isAccessibleForFree "isAccessibleForFree")` | [Boolean](/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](/free "free"). |
| `[keywords](/keywords "keywords")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text")  or  <br>[URL](/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| `[location](/location "location")` | [Place](/Place "Place")  or  <br>[PostalAddress](/PostalAddress "PostalAddress")  or  <br>[Text](/Text "Text")  or  <br>[VirtualLocation](/VirtualLocation "VirtualLocation") | The location of, for example, where an event is happening, where an organization is located, or where an action takes place. |
| `[maximumAttendeeCapacity](/maximumAttendeeCapacity "maximumAttendeeCapacity")` | [Integer](/Integer "Integer") | The total number of individuals that may attend an event or venue. |
| `[maximumPhysicalAttendeeCapacity](/maximumPhysicalAttendeeCapacity "maximumPhysicalAttendeeCapacity")` | [Integer](/Integer "Integer") | The maximum physical attendee capacity of an [Event](/Event) whose [eventAttendanceMode](/eventAttendanceMode) is [OfflineEventAttendanceMode](/OfflineEventAttendanceMode) (or the offline aspects, in the case of a [MixedEventAttendanceMode](/MixedEventAttendanceMode)). |
| `[maximumVirtualAttendeeCapacity](/maximumVirtualAttendeeCapacity "maximumVirtualAttendeeCapacity")` | [Integer](/Integer "Integer") | The maximum virtual attendee capacity of an [Event](/Event) whose [eventAttendanceMode](/eventAttendanceMode) is [OnlineEventAttendanceMode](/OnlineEventAttendanceMode) (or the online aspects, in the case of a [MixedEventAttendanceMode](/MixedEventAttendanceMode)). |
| `[offers](/offers "offers")` | [Demand](/Demand "Demand")  or  <br>[Offer](/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer.  <br>Inverse property: [itemOffered](/itemOffered "itemOffered") |
| `[organizer](/organizer "organizer")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | An organizer of an Event. |
| `[performer](/performer "performer")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A performer at the event—for example, a presenter, musician, musical group or actor. Supersedes [performers](/performers "performers"). |
| `[previousStartDate](/previousStartDate "previousStartDate")` | [Date](/Date "Date") | Used in conjunction with eventStatus for rescheduled or cancelled events. This property contains the previously scheduled start date. For rescheduled events, the startDate property should be used for the newly scheduled start date. In the (rare) case of an event that has been postponed and rescheduled multiple times, this field may be repeated. |
| `[recordedIn](/recordedIn "recordedIn")` | [CreativeWork](/CreativeWork "CreativeWork") | The CreativeWork that captured all or part of this Event.  <br>Inverse property: [recordedAt](/recordedAt "recordedAt") |
| `[remainingAttendeeCapacity](/remainingAttendeeCapacity "remainingAttendeeCapacity")` | [Integer](/Integer "Integer") | The number of attendee places for an event that remain unallocated. |
| `[review](/review "review")` | [Review](/Review "Review") | A review of the item. Supersedes [reviews](/reviews "reviews"). |
| `[sponsor](/sponsor "sponsor")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| `[startDate](/startDate "startDate")` | [Date](/Date "Date")  or  <br>[DateTime](/DateTime "DateTime") | The start date and time of the item (in [ISO 8601 date format](http://en.wikipedia.org/wiki/ISO_8601)). |
| `[subEvent](/subEvent "subEvent")` | [Event](/Event "Event") | An Event that is part of this event. For example, a conference event includes many presentations, each of which is a subEvent of the conference. Supersedes [subEvents](/subEvents "subEvents").  <br>Inverse property: [superEvent](/superEvent "superEvent") |
| `[superEvent](/superEvent "superEvent")` | [Event](/Event "Event") | An event that this event is a part of. For example, a collection of individual music performances might each have a music festival as their superEvent.  <br>Inverse property: [subEvent](/subEvent "subEvent") |
| `[translator](/translator "translator")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| `[typicalAgeRange](/typicalAgeRange "typicalAgeRange")` | [Text](/Text "Text") | The typical expected age range, e.g. '7-9', '11-'. |
| `[workFeatured](/workFeatured "workFeatured")` | [CreativeWork](/CreativeWork "CreativeWork") | A work featured in some event, e.g. exhibited in an ExhibitionEvent. Specific subproperties are available for workPerformed (e.g. a play), or a workPresented (a Movie at a ScreeningEvent). |
| `[workPerformed](/workPerformed "workPerformed")` | [CreativeWork](/CreativeWork "CreativeWork") | A work performed in some event, for example a play performed in a TheaterEvent. |
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

  

Instances of [Event](/Event "Event") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [broadcastOfEvent](/broadcastOfEvent "broadcastOfEvent") | [BroadcastEvent](/BroadcastEvent "BroadcastEvent") | The event being broadcast such as a sporting event or awards ceremony. |
| [event](/event "event") | [InformAction](/InformAction "InformAction")  or  <br>[InviteAction](/InviteAction "InviteAction")  or  <br>[JoinAction](/JoinAction "JoinAction")  or  <br>[LeaveAction](/LeaveAction "LeaveAction")  or  <br>[Organization](/Organization "Organization")  or  <br>[Place](/Place "Place")  or  <br>[PlayAction](/PlayAction "PlayAction") | Upcoming or past event associated with this place, organization, or action. |
| [events](/events "events") | [Organization](/Organization "Organization")  or  <br>[Place](/Place "Place") | Upcoming or past events associated with this place or organization. |
| [firstPerformance](/firstPerformance "firstPerformance") | [MusicComposition](/MusicComposition "MusicComposition") | The date and place the work was first performed. |
| [fundedItem](/fundedItem "fundedItem") | [Grant](/Grant "Grant") | Indicates something directly or indirectly funded or sponsored through a [Grant](/Grant). See also [ownershipFundingInfo](/ownershipFundingInfo). |
| [itemOffered](/itemOffered "itemOffered") | [Demand](/Demand "Demand")  or  <br>[Offer](/Offer "Offer") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |
| [performerIn](/performerIn "performerIn") | [Person](/Person "Person") | Event that this person is a performer or participant in. |
| [recordedAt](/recordedAt "recordedAt") | [CreativeWork](/CreativeWork "CreativeWork") | The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event. |
| [subEvent](/subEvent "subEvent") | [Event](/Event "Event") | An Event that is part of this event. For example, a conference event includes many presentations, each of which is a subEvent of the conference. |
| [subEvents](/subEvents "subEvents") | [Event](/Event "Event") | Events that are a part of this event. For example, a conference event includes many presentations, each subEvents of the conference. |
| [subjectOf](/subjectOf "subjectOf") | [Thing](/Thing "Thing") | A CreativeWork or Event about this Thing. |
| [superEvent](/superEvent "superEvent") | [Event](/Event "Event") | An event that this event is a part of. For example, a collection of individual music performances might each have a music festival as their superEvent. |

  

#### More specific Types

*   [BusinessEvent](/BusinessEvent "BusinessEvent")
*   [ChildrensEvent](/ChildrensEvent "ChildrensEvent")
*   [ComedyEvent](/ComedyEvent "ComedyEvent")
*   [CourseInstance](/CourseInstance "CourseInstance")
*   [DanceEvent](/DanceEvent "DanceEvent")
*   [DeliveryEvent](/DeliveryEvent "DeliveryEvent")
*   [EducationEvent](/EducationEvent "EducationEvent")
*   [EventSeries](/EventSeries "EventSeries")
*   [ExhibitionEvent](/ExhibitionEvent "ExhibitionEvent")
*   [Festival](/Festival "Festival")
*   [FoodEvent](/FoodEvent "FoodEvent")
*   [Hackathon](/Hackathon "Hackathon")
*   [LiteraryEvent](/LiteraryEvent "LiteraryEvent")
*   [MusicEvent](/MusicEvent "MusicEvent")
*   [PublicationEvent](/PublicationEvent "PublicationEvent")
*   [SaleEvent](/SaleEvent "SaleEvent")
*   [ScreeningEvent](/ScreeningEvent "ScreeningEvent")
*   [SocialEvent](/SocialEvent "SocialEvent")
*   [SportsEvent](/SportsEvent "SportsEvent")
*   [TheaterEvent](/TheaterEvent "TheaterEvent")
*   [VisualArtsEvent](/VisualArtsEvent "VisualArtsEvent")

### Examples
```
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "MusicGroup",
        "event": [
            {
                "@type": "Event",
                "location": "Memphis, TN, US",
                "offers": "ticketmaster.com/foofighters/may20-2011",
                "startDate": "2011-05-20",
                "url": "foo-fighters-may20-fedexforum"
            },
            {
                "@type": "Event",
                "location": "Council Bluffs, IA, US",
                "offers": "ticketmaster.com/foofighters/may23-2011",
                "startDate": "2011-05-23",
                "url": "foo-fighters-may23-midamericacenter"
            }
        ],
        "image": [
            "foofighters-1.jpg",
            "foofighters-2.jpg",
            "foofighters-3.jpg"
        ],
        "name": "Foo Fighters",
        "track": [
            {
                "@type": "MusicRecording",
                "audio": "foo-fighters-rope-play.html",
                "duration": "PT4M5S",
                "inAlbum": "foo-fighters-wasting-light.html",
                "interactionStatistic": {
                    "@type": "InteractionCounter",
                    "interactionType": "https://schema.org/ListenAction",
                    "userInteractionCount": "14300"
                },
                "name": "Rope",
                "offers": "foo-fighters-rope-buy.html",
                "url": "foo-fighters-rope.html"
            },
            {
                "@type": "MusicRecording",
                "audio": "foo-fighters-everlong-play.html",
                "duration": "PT6M33S",
                "inAlbum": "foo-fighters-color-and-shape.html",
                "name": "Everlong",
                "interactionStatistic": {
                    "@type": "InteractionCounter",
                    "interactionType": "https://schema.org/ListenAction",
                    "userInteractionCount": "11700"
                },
                "offers": "foo-fighters-everlong-buy.html",
                "url": "foo-fighters-everlong.html"
            }
        ],
        "subjectOf": {
            "@type": "VideoObject",
            "description": "Catch this exclusive interview with Dave Grohl and the Foo Fighters about their new album, Rope.",
            "duration": "PT1M33S",
            "name": "Interview with the Foo Fighters",
            "thumbnail": "foo-fighters-interview-thumb.jpg",
            "interactionStatistic": {
                "@type": "InteractionCounter",
                "interactionType": "https://schema.org/CommentAction",
                "userInteractionCount": "18"
            }
        }
    }
    </script>
```
```
    <script type="application/ld+json">
        {
          "@context": "https://schema.org",
          "@type": "ChildrensEvent",
          "name": "Story Time Reading",
          "startDate": "2020-07-24T16:00Z",
          "endDate": "2020-07-24T16:30Z",
          "eventAttendanceMode": "https://schema.org/OnlineEventAttendanceMode",
          "eventStatus": "https://schema.org/EventScheduled",
          "location": {
            "@type": "VirtualLocation",
            "url": "https://stream.storytimereadings.com/"
          },

          "image": "https://storytimereadings.com/photos/childrensphoto.jpg",
          "description": "Story Time readings for children of all ages - July 2020 edition",
          "offers": {
            "@type": "Offer",
            "url": "https://torytimereadings.com/event_offer/2020-07-24-free",
            "price": "0",
            "priceCurrency": "USD",
            "availability": "https://schema.org/InStock",
            "validFrom": "2020-07-01T12:00"
          },
          "performer": {
            "@type": "Person",
            "name": "Darren R Story",
            "alternateName": "The Virtual Story Master"
          },
          "organizer": {
            "@type": "Organization",
            "name": "Story Time Virtual Events",
            "url": "https://torytimereadings.com.com"
          }
        }
        </script>
```
```
    <script type="application/ld+json">
        {
          "@context": "https://schema.org",
          "@type": "Event",
          "name": "Count Example",
          "eventSchedule":
            {
              "@type": "Schedule",
              "startDate": "2016-12-24",
              "repeatFrequency": "P1D",
              "repeatCount": 10,
              "startTime": "09:00:00",
              "endTime": "10:00:00",
              "scheduleTimezone": "Europe/London"
            }
        }
    </script>
```# Title: FAQPage

URL Source: <https://schema.org/FAQPage>
Markdown Content:

## FAQPage Definition

Thing > CreativeWork > WebPage > FAQPage
A FAQPage is a WebPage presenting one or more "[Frequently asked questions](https://en.wikipedia.org/wiki/FAQ)".

## Structured data type definitions

You must include the required properties for your content to be eligible for display as a rich result. You can also include the recommended properties to add more information to your structured data, which could provide a better user experience.

The FAQPage type indicates that the page is an FAQ with answered questions. There must be one FAQPage type definition per page. The Google-supported properties are the following:

| Required properties | |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| mainEntity | [Question](https://schema.org/Question) An array of Question elements which contain the list of answered questions that this FAQPage is about. You must specify at least one valid [Question item](#question). A Question item includes both the question and answer. |

### Question

The full definition of Question is provided on schema.org.

The Question type defines a single answered question within the FAQ. Every Question instance must be contained within the mainEntity property array of the schema.org/FAQPage.

The Google-supported properties are the following:

| Required properties | |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| acceptedAnswer | [Answer](https://schema.org/Answer) The answer to the question. There must be one answer per question. |
| name | [Text](https://schema.org/Text) The full text of the question. For example, "How long does it take to process a refund?". |

### Answer

The full definition of Answer is provided on schema.org.

The Answer type defines the acceptedAnswer to each of the Question on this page.

The Google-supported properties are the following:

| Required properties | |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| text | [Text](https://schema.org/Text) The full answer to the question. The answer may contain HTML content such as links and lists. Google Search displays the following HTML tags:`<h1>` through `<h6>`,`<br>`, `<ol>`,`<ul>`, `<li>`,`<a>`, `<p>`,`<div>`, `<b>`,`<strong>`, `<i>`, and `<em>`. All other tags are ignored. |

## Content guidelines

* Your site must be a health or government site. It must also be well-known and authoritative.
* Only use `FAQPage` if your page contains FAQs where there's a single answer to each question. If your page has a single question and users can submit alternative answers, use[QAPage](https://developers.google.com/search/docs/appearance/structured-data/qapage?hl=en) instead. Here are some examples:
**Valid use cases**:
* An FAQ page written by the health site itself, with no way for users to submit alternative answers
* A government agency's support page that lists FAQs, with no way for users to submit alternative answers
**Invalid use cases**:
* A forum page where users can submit answers to a single question
* A product support page where users can submit answers to a single question
* A product page where users can submit multiple questions and answers on a single page
* Don't use `FAQPage` for advertising purposes.
* Make sure each `Question` includes the entire text of the question and make sure each `Answer` includes the entire text of the answer. The entire question text and answer text may be displayed.
* Question and answer content may not be displayed as a rich result if it contains any of the following types of content: obscene, profane, sexually explicit, graphically violent, promotion of dangerous or illegal activities, or hateful or harassing language.
* All `FAQ` content must be visible to the user on the source page. Here are some examples:
**Valid use cases**:
* Both the question and answer are visible on the page.
* The question is visible on the page, and the answer is hidden behind an expandable section. The user is able to access the answer by clicking the expandable section.
**Invalid use cases**: The user can't find the FAQ content on the page at all.
* If you have FAQ content that is repetitive on your site (meaning, the same question and answer appear on multiple pages on your site), mark up only one instance of that FAQ for your entire site.

## Examples in JSON-LD

```json
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "Jak długo trwa przetwarzanie zwrotu środków?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Zwrot środków jest przetwarzany w ciągu 5-7 dni roboczych."
      }
    },
    {
      "@type": "Question",
      "name": "Jak mogę skontaktować się z obsługą klienta?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "Obsługę klienta można skontaktować się telefonicznie lub przez formularz kontaktowy na naszej stronie."
      }
    }
  ]
}
```

``` html
<html>
  <head>
    <title>Finding an apprenticeship - Frequently Asked Questions(FAQ)</title>
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "FAQPage",
      "mainEntity": [{
        "@type": "Question",
        "name": "How to find an apprenticeship?",
        "acceptedAnswer": {
          "@type": "Answer",
          "text": "<p>We provide an official service to search through available apprenticeships. To get started, create an account here, specify the desired region, and your preferences. You will be able to search through all officially registered open apprenticeships.</p>"
        }
      }, {
        "@type": "Question",
        "name": "Whom to contact?",
        "acceptedAnswer": {
          "@type": "Answer",
          "text": "You can contact the apprenticeship office through our official phone hotline above, or with the web-form below. We generally respond to written requests within 7-10 days."
        }
      }]
    }
    </script>
  </head>
  <body>
  </body>
</html>
```

## Examples in Microdata

``` html
<html itemscope itemtype="https://schema.org/FAQPage">
<head></head>
<body>
  <h1>
    Frequently Asked Questions(FAQ)
  </h1>
  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
    <h2 itemprop="name">How to find an apprenticeship?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <div itemprop="text">
        We provide an official service to search through available apprenticeships. To get started, create an account here, specify the desired region, and your preferences. You will be able to search through all officially registered open apprenticeships.
      </div>
    </div>
  </div>
  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
    <h2 itemprop="name">Whom to contact?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <div itemprop="text">
        You can contact the apprenticeship office through our official phone hotline above, or with the web-form below. We generally respond to written requests within 7-10 days.
      </div>
    </div>
  </div>
</body>
</html>
```
# HowTo

Thing > CreativeWork > HowTo

Instructions that explain how to achieve a result by performing a sequence of steps.

## Structure

```json
{
  "@type": "HowTo",
  "name": "Change a Flat Tire",
  "totalTime": "PT30M",
  "tool": [
    {
      "@type": "HowToTool",
      "name": "Wheel wedges",
      "image": "http://example.org/wheel-wedges.jpg"
    },
    {
      "@type": "HowToTool",
      "name": "Jack"
    },
    {
      "@type": "HowToTool",
      "name": "Lug wrench",
      "image": "http://example.org/lug-wrench.jpg"
    },
    {
      "@type": "HowToTool",
      "name": "Spare tire"
    }
  ],
  "supply": [
    {
      "@type": "HowToSupply",
      "name": "Flares",
      "image": "http://example.org/flares.jpg"
    }
  ],
  "step": [
    {
      "@type": "HowToSection",
      "name": "Raise the car",
      "position": 2,
      "itemListElement": [
        {
          "@type": "HowToStep",
          "position": 5,
          "itemListElement": [
            {
              "@type": "HowToTip",
              "text": "Don't use the wrench just yet.",
              "position": 2
            },
            {
              "@type": "HowToDirection",
              "text": "Tighten the lug nuts by hand.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 4,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "text": "Remove the flat tire and put the spare tire on the exposed lug bolts.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 3,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "text": "Remove the hubcap and loosen the lug nuts.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 2,
          "itemListElement": [
            {
              "@type": "HowToTip",
              "text": "It doesn't need to be too high.",
              "position": 2
            },
            {
              "@type": "HowToDirection",
              "beforeMedia": {
                "@type": "ImageObject",
                "contentUrl": "http://example.org/car-on-ground.jpg"
              },
              "afterMedia": {
                "@type": "ImageObject",
                "contentUrl": "http://example.org/car-raised.jpg"
              },
              "text": "Raise the jack until the flat tire is just barely off of the ground.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 1,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "duringMedia": "http://example.org/position-jack.jpg",
              "text": "Position the jack underneath the car, next to the flat tire.",
              "position": 1
            }
          ]
        }
      ]
    },
    {
      "@type": "HowToSection",
      "name": "Finishing up",
      "position": 3,
      "itemListElement": [
        {
          "@type": "HowToStep",
          "position": 3,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "text": "Put the equipment and the flat tire away.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 2,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "text": "Replace the hubcap.",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 1,
          "itemListElement": [
            {
              "@type": "HowToDirection",
              "text": "Lower the jack and tighten the lug nuts with the wrench.",
              "position": 1
            }
          ]
        }
      ]
    },
    {
      "@type": "HowToSection",
      "name": "Preparation",
      "position": 1,
      "itemListElement": [
        {
          "@type": "HowToStep",
          "position": 2,
          "itemListElement": [
            {
              "@type": "HowToTip",
              "text": "You don't want the car to move while you're working on it.",
              "position": 2
            },
            {
              "@type": "HowToDirection",
              "text": "Position your wheel wedges in front of the front tires if a rear tire is flat, or behind the rear tires if a front tire is flat",
              "position": 1
            }
          ]
        },
        {
          "@type": "HowToStep",
          "position": 1,
          "itemListElement": [
            {
              "@type": "HowToTip",
              "text": "You're going to need space and want to be visible.",
              "position": 2
            },
            {
              "@type": "HowToDirection",
              "text": "Turn on your hazard lights and set the flares.",
              "position": 1
            }
          ]
        }
      ]
    }
  ],
  "estimatedCost": {
    "@type": "MonetaryAmount",
    "value": 20,
    "currency": "USD"
  }
}
```

## HowTo Examples

### JSON-LD

Example encoded as JSON-LD in a HTML script tag.

```json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "HowTo",
      "name": "Change a Flat Tire",
      "estimatedCost": {
        "@type": "MonetaryAmount",
        "currency": "USD",
        "value": "20"
      },
      "totalTime": "PT30M",
      "tool": [
        {
          "@type": "HowToTool",
          "name": "Spare tire"
        },
        {
          "@type": "HowToTool",
          "name": "Lug wrench",
          "image": "lug-wrench.jpg"
        },
        {
          "@type": "HowToTool",
          "name": "Jack"
        },
        {
          "@type": "HowToTool",
          "name": "Wheel wedges",
          "image": "wheel-wedges.jpg"
        }
      ],
      "supply": {
        "@type": "HowToSupply",
        "name": "Flares",
        "image": "flares.jpg"
      },
      "step": [
        {
          "@type": "HowToSection",
          "name": "Preparation",
          "position": "1",
          "itemListElement": [
            {
              "@type": "HowToStep",
              "position": "1",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Turn on your hazard lights and set the flares."
                },
                {
                  "@type": "HowToTip",
                  "position": "2",
                  "text": "You're going to need space and want to be visible."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "2",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Position your wheel wedges in front of the front tires if a rear tire is flat, or behind the rear tires if a front tire is flat"
                },
                {
                  "@type": "HowToTip",
                  "position": "2",
                  "text": "You don't want the car to move while you're working on it."
                }
              ]
            }
          ]
        },
        {
          "@type": "HowToSection",
          "name": "Raise the car",
          "position": "2",
          "itemListElement": [
            {
              "@type": "HowToStep",
              "position": "1",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "duringMedia": "position-jack.jpg",
                  "text": "Position the jack underneath the car, next to the flat tire."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "2",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "beforeMedia": {
                      "@type": "ImageObject",
                      "contentUrl": "car-on-ground.jpg"
                  },
                  "afterMedia": {
                      "@type": "ImageObject",
                      "contentUrl": "car-raised.jpg"
                  },
                  "text": "Raise the jack until the flat tire is just barely off of the ground."
                },
                {
                  "@type": "HowToTip",
                  "position": "2",
                  "text": "It doesn't need to be too high."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "3",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Remove the hubcap and loosen the lug nuts."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "4",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Remove the flat tire and put the spare tire on the exposed lug bolts."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "5",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Tighten the lug nuts by hand."
                },
                {
                  "@type": "HowToTip",
                  "position": "2",
                  "text": "Don't use the wrench just yet."
                }
              ]
            }
          ]
        },
        {
          "@type": "HowToSection",
          "name": "Finishing up",
          "position": "3",
          "itemListElement": [
            {
              "@type": "HowToStep",
              "position": "1",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Lower the jack and tighten the lug nuts with the wrench."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "2",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Replace the hubcap."
                }
              ]
            },
            {
              "@type": "HowToStep",
              "position": "3",
              "itemListElement": [
                {
                  "@type": "HowToDirection",
                  "position": "1",
                  "text": "Put the equipment and the flat tire away."
                }
              ]
            }
          ]
        }
      ]
    }
    </script>
```

### Microdata

Example encoded as Microdata embedded in HTML.

```html
    <div itemscope itemtype="https://schema.org/HowTo">
      <strong><span itemprop="name">Change a Flat Tire</span></strong>
      <div>About <span itemprop="estimatedCost" itemscope itemtype="https://schema.org/MonetaryAmount">
        <meta itemprop="currency" content="USD"/>
        <meta itemprop="value" content="20"/>
      </span>$20</div>
      <div>About <span itemprop="totalTime" content="PT30M">30 minutes</span></div>
      <div>Necessary Items:</div>
      <div itemprop="tool">Spare tire</div>
      <div itemprop="tool" itemscope itemtype="https://schema.org/HowToTool">
        <span itemprop="name">Lug wrench</span>
        <img alt="image of a lug wrench" itemprop="image" src="lug-wrench.jpg"/>
      </div>
      <div itemprop="tool">Jack</div>
      <div itemprop="tool" itemscope itemtype="https://schema.org/HowToTool">
        <span itemprop="name">Wheel wedges</span>
        <img alt="image showing wheel wedges" itemprop="image" src="wheel-wedges.jpg"/>
      </div>
      <div itemprop="supply" itemscope itemtype="https://schema.org/HowToSupply">
        <span itemprop="name">Flares</span>
        <img alt="image of flares" itemprop="image" src="flares.jpg"/>
      </div>
      <div itemprop="step" itemscope itemtype="https://schema.org/HowToSection">
        <div itemprop="name">Preparation</div>
        <meta itemprop="position" content="1"/>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="1"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Turn on your hazard lights and set the flares.</div>
          </div>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToTip">
            <meta itemprop="position" content="2"/>
            <div itemprop="text">You're going to need space and want to be visible.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="2"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Position your wheel wedges in front of the front tires if a rear tire is flat, or behind the rear tires if a front tire is flat.</div>
          </div>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToTip">
            <meta itemprop="position" content="2"/>
            <div itemprop="text">You don't want the car to move while you're working on it.</div>
          </div>
        </div>
      </div>
      <div itemprop="step" itemscope itemtype="https://schema.org/HowToSection">
        <div itemprop="name">Raise the car</div>
        <meta itemprop="position" content="2"/>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="1"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <img alt="image showing positioning of jack" itemprop="duringMedia" src="position-jack.jpg" />
            <div itemprop="text">Position the jack underneath the car, next to the flat tire.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="2"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="beforeMedia" itemscope itemtype="https://schema.org/ImageObject">
              <img alt="image showing car while still on the ground" itemprop="contentUrl" src="car-on-ground.jpg" />
            </div>
            <div itemprop="text">Raise the jack until the flat tire is just barely off of the ground.</div>
            <div itemprop="afterMedia" itemscope itemtype="https://schema.org/ImageObject">
              <img alt="image showing car raised by jack" itemprop="contentUrl" src="car-raised.jpg" />
            </div>
          </div>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToTip">
            <meta itemprop="position" content="2"/>
            <div itemprop="text">It doesn't need to be too high.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="3"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Remove the hubcap and loosen the lug nuts.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="4"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Remove the flat tire and put the spare tire on the exposed lug bolts.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="5"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Tighten the lug nuts by hand.</div>
          </div>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToTip">
            <meta itemprop="position" content="2"/>
            <div itemprop="text">Don't use the wrench just yet.</div>
          </div>
        </div>
      </div>
      <div itemprop="step" itemscope itemtype="https://schema.org/HowToSection">
        <div itemprop="name">Finishing up</div>
        <meta itemprop="position" content="3"/>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="1"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1">
            <div itemprop="text">Lower the jack and tighten the lug nuts with the wrench.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="2"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Replace the hubcap.</div>
          </div>
        </div>
        <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToStep">
          <meta itemprop="position" content="3"/>
          <div itemprop="itemListElement" itemscope itemtype="https://schema.org/HowToDirection">
            <meta itemprop="position" content="1"/>
            <div itemprop="text">Put the equipment and the flat tire away.</div>
          </div>
        </div>
      </div>
    </div>
```

## Properties

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [HowTo](/HowTo "HowTo") | | |
| [estimatedCost](/estimatedCost "estimatedCost") | [MonetaryAmount](/MonetaryAmount "MonetaryAmount") or [Text](/Text "Text") | The estimated cost of the supply or supplies consumed when performing instructions. |
| [performTime](/performTime "performTime") | [Duration](/Duration "Duration") | The length of time it takes to perform instructions or a direction (not including time to prepare the supplies), in [ISO 8601 duration format](http://en.wikipedia.org/wiki/ISO%5F8601). |
| [prepTime](/prepTime "prepTime") | [Duration](/Duration "Duration") | The length of time it takes to prepare the items to be used in instructions or a direction, in [ISO 8601 duration format](http://en.wikipedia.org/wiki/ISO%5F8601). |
| [step](/step "step") | [CreativeWork](/CreativeWork "CreativeWork") or [HowToSection](/HowToSection "HowToSection") or [HowToStep](/HowToStep "HowToStep") or [Text](/Text "Text") | A single step item (as HowToStep, text, document, video, etc.) or a HowToSection. Supersedes [steps](/steps "steps"). |
| [supply](/supply "supply") | [HowToSupply](/HowToSupply "HowToSupply") or [Text](/Text "Text") | A sub-property of instrument. A supply consumed when performing instructions or a direction. |
| [tool](/tool "tool") | [HowToTool](/HowToTool "HowToTool") or [Text](/Text "Text") | A sub property of instrument. An object used (but not consumed) when performing instructions or a direction. |
| [totalTime](/totalTime "totalTime") | [Duration](/Duration "Duration") | The total time required to perform instructions or a direction (including time to prepare the supplies), in [ISO 8601 duration format](http://en.wikipedia.org/wiki/ISO%5F8601). |
| [yield](/yield "yield") | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") or [Text](/Text "Text") | The quantity that results by performing instructions. For example, a paper airplane, 10 personalized candles. |
| Properties from [CreativeWork](/CreativeWork "CreativeWork") | | |
| [about](/about "about") | [Thing](/Thing "Thing") | The subject matter of the content.Inverse property: [subjectOf](/subjectOf "subjectOf") |
| [abstract](/abstract "abstract") | [Text](/Text "Text") | An abstract is a short description that summarizes a [CreativeWork](/CreativeWork). |
| [accessMode](/accessMode "accessMode") | [Text](/Text "Text") | The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessMode-vocabulary). |
| [accessModeSufficient](/accessModeSufficient "accessModeSufficient") | [ItemList](/ItemList "ItemList") | A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessModeSufficient-vocabulary). |
| [accessibilityAPI](/accessibilityAPI "accessibilityAPI") | [Text](https://schema.org/Text "Text") | Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityAPI-vocabulary). |
| [accessibilityControl](/accessibilityControl "accessibilityControl") | [Text](/Text "Text") | Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityControl-vocabulary). |
| [accessibilityFeature](/accessibilityFeature "accessibilityFeature") | [Text](/Text "Text") | Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityFeature-vocabulary). |
| [accessibilityHazard](/accessibilityHazard "accessibilityHazard") | [Text](/Text "Text") | A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3\. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityHazard-vocabulary). |
| [accessibilitySummary](/accessibilitySummary "accessibilitySummary") | [Text](/Text "Text") | A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed". |
| [accountablePerson](/accountablePerson "accountablePerson") | [Person](/Person "Person") | Specifies the Person that is legally accountable for the CreativeWork. |
| [acquireLicensePage](/acquireLicensePage "acquireLicensePage") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item. |
| [aggregateRating](/aggregateRating "aggregateRating") | [AggregateRating](/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| [alternativeHeadline](/alternativeHeadline "alternativeHeadline") | [Text](/Text "Text") | A secondary title of the CreativeWork. |
| [archivedAt](/archivedAt "archivedAt") | [URL](/URL "URL") or [WebPage](/WebPage "WebPage") | Indicates a page or other link involved in archival of a [CreativeWork](/CreativeWork). In the case of [MediaReview](/MediaReview), the items in a [MediaReviewItem](/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content. |
| [assesses](/assesses "assesses") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | The item being described is intended to assess the competency or learning outcome defined by the referenced term. |
| [associatedMedia](/associatedMedia "associatedMedia") | [MediaObject](/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for encoding. |
| [audience](/audience "audience") | [Audience](/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](/serviceAudience "serviceAudience"). |
| [audio](/audio "audio") | [AudioObject](/AudioObject "AudioObject") or [Clip](/Clip "Clip") or [MusicRecording](/MusicRecording "MusicRecording") | An embedded audio object. |
| [author](/author "author") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| [award](/award "award") | [Text](/Text "Text") | An award won by or for this item. Supersedes [awards](/awards "awards"). |
| [character](/character "character") | [Person](/Person "Person") | Fictional person connected with a creative work. |
| [citation](/citation "citation") | [CreativeWork](/CreativeWork "CreativeWork") or [Text](/Text "Text") | A citation or reference to another creative work, such as another publication, web page, scholarly article, etc. |
| [comment](/comment "comment") | [Comment](/Comment "Comment") | Comments, typically from users. |
| [commentCount](/commentCount "commentCount") | [Integer](/Integer "Integer") | The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere. |
| [conditionsOfAccess](/conditionsOfAccess "conditionsOfAccess") | [Text](/Text "Text") | Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an [ArchiveComponent](/ArchiveComponent) held by an [ArchiveOrganization](/ArchiveOrganization). This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language.For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts ". |
| [contentLocation](/contentLocation "contentLocation") | [Place](/Place "Place") | The location depicted or described in the content. For example, the location in a photograph or painting. |
| [contentRating](/contentRating "contentRating") | [Rating](/Rating "Rating") or [Text](/Text "Text") | Official rating of a piece of content—for example, 'MPAA PG-13'. |
| [contentReferenceTime](/contentReferenceTime "contentReferenceTime") | [DateTime](/DateTime "DateTime") | The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event. |
| [contributor](/contributor "contributor") | [Organization](/Organization "Organization") or [Person](/Person "Person") | A secondary contributor to the CreativeWork or Event. |
| [copyrightHolder](/copyrightHolder "copyrightHolder") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The party holding the legal copyright to the CreativeWork. |
| [copyrightNotice](/copyrightNotice "copyrightNotice") | [Text](/Text "Text") | Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work. |
| [copyrightYear](/copyrightYear "copyrightYear") | [Number](/Number "Number") | The year during which the claimed copyright for the CreativeWork was first asserted. |
| [correction](/correction "correction") | [CorrectionComment](/CorrectionComment "CorrectionComment") or [Text](/Text "Text") or [URL](/URL "URL") | Indicates a correction to a [CreativeWork](/CreativeWork), either via a [CorrectionComment](/CorrectionComment), textually or in another document. |
| [countryOfOrigin](/countryOfOrigin "countryOfOrigin") | [Country](/Country "Country") | The country of origin of something, including products as well as creative works such as movie and TV content.In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](/contentLocation) and [locationCreated](/locationCreated) may be more applicable.In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here. |
| [creativeWorkStatus](/creativeWorkStatus "creativeWorkStatus") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle. |
| [creator](/creator "creator") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| [creditText](/creditText "creditText") | [Text](/Text "Text") | Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work. |
| [dateCreated](/dateCreated "dateCreated") | [Date](/Date "Date") or [DateTime](/DateTime "DateTime") | The date on which the CreativeWork was created or the item was added to a DataFeed. |
| [dateModified](/dateModified "dateModified") | [Date](/Date "Date") or [DateTime](/DateTime "DateTime") | The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed. |
| [datePublished](/datePublished "datePublished") | [Date](/Date "Date") or [DateTime](/DateTime "DateTime") | Date of first publication or broadcast. For example the date a [CreativeWork](/CreativeWork) was broadcast or a [Certification](/Certification) was issued. |
| [digitalSourceType](/digitalSourceType "digitalSourceType") | [IPTCDigitalSourceEnumeration](/IPTCDigitalSourceEnumeration "IPTCDigitalSourceEnumeration") | Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some [CreativeWork](/CreativeWork). |
| [discussionUrl](/discussionUrl "discussionUrl") | [URL](/URL "URL") | A link to the page containing the comments of the CreativeWork. |
| [editEIDR](/editEIDR "editEIDR") | [Text](/Text "Text") or [URL](/URL "URL") | An [EIDR](https://eidr.org/) (Entertainment Identifier Registry) [identifier](/identifier) representing a specific edit / edition for a work of film or television.For example, the motion picture known as "Ghostbusters" whose [titleEIDR](/titleEIDR) is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3".Since schema.org types like [Movie](/Movie) and [TVEpisode](/TVEpisode) can be used for both works and their multiple expressions, it is possible to use [titleEIDR](/titleEIDR) alone (for a general description), or alongside [editEIDR](/editEIDR) for a more edit-specific description. |
| [editor](/editor "editor") | [Person](/Person "Person") | Specifies the Person who edited the CreativeWork. |
| [educationalAlignment](/educationalAlignment "educationalAlignment") | [AlignmentObject](/AlignmentObject "AlignmentObject") | An alignment to an established educational framework.This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource [teaches](/teaches) or [assesses](/assesses) a competency. |
| [educationalLevel](/educationalLevel "educationalLevel") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") or [URL](/URL "URL") | The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators. |
| [educationalUse](/educationalUse "educationalUse") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | The purpose of a work in the context of education; for example, 'assignment', 'group work'. |
| [encoding](/encoding "encoding") | [MediaObject](/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes [encodings](/encodings "encodings").Inverse property: [encodesCreativeWork](/encodesCreativeWork "encodesCreativeWork") |
| [encodingFormat](/encodingFormat "encodingFormat") | [Text](/Text "Text") or [URL](/URL "URL") | Media type typically expressed using a MIME format (see [IANA site](http://www.iana.org/assignments/media-types/media-types.xhtml) and [MDN reference](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics%5Fof%5FHTTP/MIME%5Ftypes)), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc.In cases where a [CreativeWork](/CreativeWork) has several media type representations, [encoding](/encoding) can be used to indicate each [MediaObject](/MediaObject) alongside particular [encodingFormat](/encodingFormat) information.Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes [fileFormat](/fileFormat "fileFormat"). |
| [exampleOfWork](/exampleOfWork "exampleOfWork") | [CreativeWork](/CreativeWork "CreativeWork") | A creative work that this work is an example/instance/realization/derivation of.Inverse property: [workExample](/workExample "workExample") |
| [expires](/expires "expires") | [Date](/Date "Date") or [DateTime](/DateTime "DateTime") | Date the content expires and is no longer useful or available. For example a [VideoObject](/VideoObject) or [NewsArticle](/NewsArticle) whose availability or relevance is time-limited, a [ClaimReview](/ClaimReview) fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a [Certification](/Certification) the validity has expired. |
| [funder](/funder "funder") | [Organization](/Organization "Organization") or [Person](/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| [funding](/funding "funding") | [Grant](/Grant "Grant") | A [Grant](/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](/ownershipFundingInfo).Inverse property: [fundedItem](/fundedItem "fundedItem") |
| [genre](/genre "genre") | [Text](/Text "Text") or [URL](/URL "URL") | Genre of the creative work, broadcast channel or group. |
| [hasPart](/hasPart "hasPart") | [CreativeWork](/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense).Inverse property: [isPartOf](/isPartOf "isPartOf") |
| [headline](/headline "headline") | [Text](/Text "Text") | Headline of the article. |
| [inLanguage](/inLanguage "inLanguage") | [Language](/Language "Language") or [Text](/Text "Text") | The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](/availableLanguage). Supersedes [language](/language "language"). |
| [interactionStatistic](/interactionStatistic "interactionStatistic") | [InteractionCounter](/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](/interactionCount "interactionCount"). |
| [interactivityType](/interactivityType "interactivityType") | [Text](/Text "Text") | The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'. |
| [interpretedAsClaim](/interpretedAsClaim "interpretedAsClaim") | [Claim](/Claim "Claim") | Used to indicate a specific claim contained, implied, translated or refined from the content of a [MediaObject](/MediaObject) or other [CreativeWork](/CreativeWork). The interpreting party can be indicated using [claimInterpreter](/claimInterpreter). |
| [isAccessibleForFree](/isAccessibleForFree "isAccessibleForFree") | [Boolean](/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](/free "free"). |
| [isBasedOn](/isBasedOn "isBasedOn") | [CreativeWork](/CreativeWork "CreativeWork") or [Product](/Product "Product") or [URL](/URL "URL") | A resource from which this work is derived or from which it is a modification or adaptation. Supersedes [isBasedOnUrl](/isBasedOnUrl "isBasedOnUrl"). |
| [isFamilyFriendly](/isFamilyFriendly "isFamilyFriendly") | [Boolean](/Boolean "Boolean") | Indicates whether this content is family friendly. |
| [isPartOf](/isPartOf "isPartOf") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of.Inverse property: [hasPart](/hasPart "hasPart") |
| [keywords](/keywords "keywords") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") or [URL](/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| [learningResourceType](/learningResourceType "learningResourceType") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'. |
| [license](/license "license") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | A license document that applies to this content, typically indicated by URL. |
| [locationCreated](/locationCreated "locationCreated") | [Place](/Place "Place") | The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork. |
| [mainEntity](/mainEntity "mainEntity") | [Thing](/Thing "Thing") | Indicates the primary entity described in some page or other CreativeWork.Inverse property: [mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage") |
| [maintainer](/maintainer "maintainer") | [Organization](/Organization "Organization") or [Person](/Person "Person") | A maintainer of a [Dataset](/Dataset), software package ([SoftwareApplication](/SoftwareApplication)), or other [Project](/Project). A maintainer is a [Person](/Person) or [Organization](/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| [material](/material "material") | [Product](/Product "Product") or [Text](/Text "Text") or [URL](/URL "URL") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| [materialExtent](/materialExtent "materialExtent") | [QuantitativeValue](/QuantitativeValue "QuantitativeValue") or [Text](/Text "Text") | The quantity of the materials being described or an expression of the physical space they occupy. |
| [mentions](/mentions "mentions") | [Thing](/Thing "Thing") | Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept. |
| [offers](/offers "offers") | [Demand](/Demand "Demand") or [Offer](/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer.Inverse property: [itemOffered](/itemOffered "itemOffered") |
| [pattern](/pattern "pattern") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported. |
| [position](/position "position") | [Integer](/Integer "Integer") or [Text](/Text "Text") | The position of an item in a series or sequence of items. |
| [producer](/producer "producer") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| [provider](/provider "provider") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](/carrier "carrier"). |
| [publication](/publication "publication") | [PublicationEvent](/PublicationEvent "PublicationEvent") | A publication event associated with the item. |
| [publisher](/publisher "publisher") | [Organization](/Organization "Organization") or [Person](/Person "Person") | The publisher of the article in question. |
| [publisherImprint](/publisherImprint "publisherImprint") | [Organization](/Organization "Organization") | The publishing division which published the comic. |
| [publishingPrinciples](/publishingPrinciples "publishingPrinciples") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | The publishingPrinciples property indicates (typically via [URL](/URL)) a document describing the editorial principles of an [Organization](/Organization) (or individual, e.g. a [Person](/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](/CreativeWork) (e.g. [NewsArticle](/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](/CreativeWork).While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](/funder)) can be expressed using schema.org terminology. |
| [recordedAt](/recordedAt "recordedAt") | [Event](/Event "Event") | The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event.Inverse property: [recordedIn](/recordedIn "recordedIn") |
| [releasedEvent](/releasedEvent "releasedEvent") | [PublicationEvent](/PublicationEvent "PublicationEvent") | The place and time the release was issued, expressed as a PublicationEvent. |
| [review](/review "review") | [Review](/Review "Review") | A review of the item. Supersedes [reviews](/reviews "reviews"). |
| [schemaVersion](/schemaVersion "schemaVersion") | [Text](/Text "Text") or [URL](/URL "URL") | Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. 10.0 as a simple string, or more explicitly via URL, https://schema.org/docs/releases.html#v10.0. There may be situations in which other schemas might usefully be referenced this way, e.g. http://dublincore.org/specifications/dublin-core/dces/1999-07-02/ but this has not been carefully explored in the community. |
| [sdDatePublished](/sdDatePublished "sdDatePublished") | [Date](/Date "Date") | Indicates the date on which the current structured data was generated / published. Typically used alongside [sdPublisher](/sdPublisher). |
| [sdLicense](/sdLicense "sdLicense") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | A license document that applies to this structured data, typically indicated by URL. |
| [sdPublisher](/sdPublisher "sdPublisher") | [Organization](/Organization "Organization") or [Person](/Person "Person") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The[sdPublisher](/sdPublisher) property helps make such practices more explicit. |
| [size](/size "size") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [QuantitativeValue](/QuantitativeValue "QuantitativeValue") or [SizeSpecification](/SizeSpecification "SizeSpecification") or [Text](/Text "Text") | A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](/SizeSpecification); in other cases, the [width](/width), [height](/height), [depth](/depth) and [weight](/weight) properties may be more applicable. |
| [sourceOrganization](/sourceOrganization "sourceOrganization") | [Organization](/Organization "Organization") | The Organization on whose behalf the creator was working. |
| [spatial](/spatial "spatial") | [Place](/Place "Place") | The "spatial" property can be used in cases when more specific properties (e.g. [locationCreated](/locationCreated), [spatialCoverage](/spatialCoverage), [contentLocation](/contentLocation)) are not known to be appropriate. |
| [spatialCoverage](/spatialCoverage "spatialCoverage") | [Place](/Place "Place") | The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York. |
| [sponsor](/sponsor "sponsor") | [Organization](/Organization "Organization") or [Person](/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| [teaches](/teaches "teaches") | [DefinedTerm](/DefinedTerm "DefinedTerm") or [Text](/Text "Text") | The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term. |
| [temporal](/temporal "temporal") | [DateTime](/DateTime "DateTime") or [Text](/Text "Text") | The "temporal" property can be used in cases where more specific properties (e.g. [temporalCoverage](/temporalCoverage), [dateCreated](/dateCreated), [dateModified](/dateModified), [datePublished](/datePublished)) are not known to be appropriate. |
| [temporalCoverage](/temporalCoverage "temporalCoverage") | [DateTime](/DateTime "DateTime") or [Text](/Text "Text") or [URL](/URL "URL") | The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in [ISO 8601 time interval format](https://en.wikipedia.org/wiki/ISO%5F8601#Time%5Fintervals). In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945".Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes [datasetTimeInterval](/datasetTimeInterval "datasetTimeInterval"). |
| [text](/text "text") | [Text](/Text "Text") | The textual content of this CreativeWork. |
| [thumbnail](/thumbnail "thumbnail") | [ImageObject](/ImageObject "ImageObject") | Thumbnail image for an image or video. |
| [thumbnailUrl](/thumbnailUrl "thumbnailUrl") | [URL](/URL "URL") | A thumbnail image relevant to the Thing. |
| [timeRequired](/timeRequired "timeRequired") | [Duration](/Duration "Duration") | Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience. |
| [translationOfWork](/translationOfWork "translationOfWork") | [CreativeWork](/CreativeWork "CreativeWork") | The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”.Inverse property: [workTranslation](/workTranslation "workTranslation") |
| [translator](/translator "translator") | [Organization](/Organization "Organization") or [Person](/Person "Person") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| [typicalAgeRange](/typicalAgeRange "typicalAgeRange") | [Text](/Text "Text") | The typical expected age range, e.g. '7-9', '11-'. |
| [usageInfo](/usageInfo "usageInfo") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | The schema.org [usageInfo](/usageInfo) property indicates further information about a [CreativeWork](/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options.This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses. |
| [version](/version "version") | [Number](/Number "Number") or [Text](/Text "Text") | The version of the CreativeWork embodied by a specified resource. |
| [video](/video "video") | [Clip](/Clip "Clip") or [VideoObject](/VideoObject "VideoObject") | An embedded video object. |
| [wordCount](/wordCount "wordCount") | [Integer](/Integer "Integer") | The number of words in the text of the CreativeWork such as an Article, Book, etc. |
| [workExample](/workExample "workExample") | [CreativeWork](/CreativeWork "CreativeWork") | Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book.Inverse property: [exampleOfWork](/exampleOfWork "exampleOfWork") |
| [workTranslation](/workTranslation "workTranslation") | [CreativeWork](/CreativeWork "CreativeWork") | A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo.Inverse property: [translationOfWork](/translationOfWork "translationOfWork") |
| Properties from [Thing](/Thing "Thing") | | |
| [additionalType](/additionalType "additionalType") | [Text](/Text "Text") or [URL](/URL "URL") | An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. Typically the value is a URI-identified RDF class, and in this case corresponds to the use of rdf:type in RDF. Text values can be used sparingly, for cases where useful information can be added without their being an appropriate schema to reference. In the case of text values, the class label should follow the schema.org [style guide](https://schema.org/docs/styleguide.html). |
| [alternateName](/alternateName "alternateName") | [Text](/Text "Text") | An alias for the item. |
| [description](/description "description") | [Text](/Text "Text") or [TextObject](/TextObject "TextObject") | A description of the item. |
| [disambiguatingDescription](/disambiguatingDescription "disambiguatingDescription") | [Text](/Text "Text") | A sub property of description. A short description of the item used to disambiguate from other, similar items. Information from other properties (in particular, name) may be necessary for the description to be useful for disambiguation. |
| [identifier](/identifier "identifier") | [PropertyValue](/PropertyValue "PropertyValue") or [Text](/Text "Text") or [URL](/URL "URL") | The identifier property represents any kind of identifier for any kind of [Thing](/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](/docs/datamodel.html#identifierBg) for more details. |
| [image](/image "image") | [ImageObject](/ImageObject "ImageObject") or [URL](/URL "URL") | An image of the item. This can be a [URL](/URL) or a fully described [ImageObject](/ImageObject). |
| [mainEntityOfPage](/mainEntityOfPage "mainEntityOfPage") | [CreativeWork](/CreativeWork "CreativeWork") or [URL](/URL "URL") | Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See [background notes](/docs/datamodel.html#mainEntityBackground) for details.Inverse property: [mainEntity](/mainEntity "mainEntity") |
| [name](/name "name") | [Text](/Text "Text") | The name of the item. |
| [potentialAction](/potentialAction "potentialAction") | [Action](/Action "Action") | Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role. |
| [sameAs](/sameAs "sameAs") | [URL](/URL "URL") | URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website. |
| [subjectOf](/subjectOf "subjectOf") | [CreativeWork](/CreativeWork "CreativeWork") or [Event](/Event "Event") | A CreativeWork or Event about this Thing.Inverse property: [about](/about "about") |
| [url](/url "url") | [URL](/URL "URL") | URL of the item. |
Title: LocalBusiness - Schema.org Type

URL Source: https://schema.org/LocalBusiness

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

A particular physical business or branch of an organization. Examples of LocalBusiness include a restaurant, a particular branch of a restaurant chain, a branch of a bank, a medical practice, a club, a bowling alley, etc.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [LocalBusiness](https://schema.org/LocalBusiness "LocalBusiness") |
| ``` currenciesAccepted ``` | [Text](https://schema.org/Text "Text") | The currency accepted. Use standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR". |
| ``` openingHours ``` | [Text](https://schema.org/Text "Text") | The general opening hours for a business. Opening hours can be specified as a weekly time range, starting with days, then times per day. Multiple days can be listed with commas ',' separating each day. Day or time ranges are specified using a hyphen '-'. * Days are specified using the following two-letter combinations: `Mo`, `Tu`, `We`, `Th`, `Fr`, `Sa`, `Su`. * Times are specified using 24:00 format. For example, 3pm is specified as `15:00`, 10am as `10:00`. * Here is an example: `<time itemprop="openingHours" datetime="Tu,Th 16:00-20:00">Tuesdays and Thursdays 4-8pm</time>`. * If a business is open 7 days a week, then it can be specified as `<time itemprop="openingHours" datetime="Mo-Su">Monday through Sunday, all day</time>`. |
| ``` paymentAccepted ``` | [Text](https://schema.org/Text "Text") | Cash, Credit Card, Cryptocurrency, Local Exchange Tradings System, etc. |
| ``` priceRange ``` | [Text](https://schema.org/Text "Text") | The price range of the business, for example `$$$`. |
| Properties from [Organization](https://schema.org/Organization "Organization") |
| ``` acceptedPaymentMethod ``` | [LoanOrCredit](https://schema.org/LoanOrCredit "LoanOrCredit") or [PaymentMethod](https://schema.org/PaymentMethod "PaymentMethod") or [Text](https://schema.org/Text "Text") | The payment method(s) that are accepted in general by an organization, or for some specific demand or offer. |
| ``` actionableFeedbackPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) or other news-related [Organization](https://schema.org/Organization), a statement about public engagement activities (for news media, the newsroom’s), including involving the public - digitally or otherwise -- in coverage decisions, reporting and activities after publication. |
| ``` address ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") | Physical address of the item. |
| ``` agentInteractionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of completed interactions for this entity, in a particular role (the 'agent'), in a particular action (indicated in the statistic), and in a particular context (i.e. interactionService). |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` alumni ``` | [Person](https://schema.org/Person "Person") | Alumni of an organization. Inverse property: [alumniOf](https://schema.org/alumniOf "alumniOf") |
| ``` areaServed ``` | [AdministrativeArea](https://schema.org/AdministrativeArea "AdministrativeArea") or [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](https://schema.org/serviceArea "serviceArea"). |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` brand ``` | [Brand](https://schema.org/Brand "Brand") or [Organization](https://schema.org/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| ``` companyRegistration ``` | [Certification](https://schema.org/Certification "Certification") | The official registration number of a business including the organization that issued it such as Company House or Chamber of Commerce. |
| ``` contactPoint ``` | [ContactPoint](https://schema.org/ContactPoint "ContactPoint") | A contact point for a person or organization. Supersedes [contactPoints](https://schema.org/contactPoints "contactPoints"). |
| ``` correctionsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (e.g. [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement describing (in news media, the newsroom’s) disclosure and correction policy for errors. |
| ``` department ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between an organization and a department of that organization, also described as an organization (allowing different urls, logos, opening hours). For example: a store with a pharmacy, or a bakery with a cafe. |
| ``` dissolutionDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was dissolved. |
| ``` diversityPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement on diversity policy by an [Organization](https://schema.org/Organization) e.g. a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization). For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), a statement describing the newsroom’s diversity policy on both staffing and sources, typically providing staffing data. |
| ``` diversityStaffingReport ``` | [Article](https://schema.org/Article "Article") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a report on staffing diversity issues. In a news context this might be for example ASNE or RTDNA (US) reports, or self-reported. |
| ``` duns ``` | [Text](https://schema.org/Text "Text") | The Dun & Bradstreet DUNS number for identifying an organization or business person. |
| ``` email ``` | [Text](https://schema.org/Text "Text") | Email address. |
| ``` employee ``` | [Person](https://schema.org/Person "Person") | Someone working for this organization. Supersedes [employees](https://schema.org/employees "employees"). |
| ``` ethicsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement about ethics policy, e.g. of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) regarding journalistic and publishing practices, or of a [Restaurant](https://schema.org/Restaurant), a page describing food source policies. In the case of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), an ethicsPolicy is typically a statement describing the personal, organizational, and corporate standards of behavior expected by the organization. |
| ``` event ``` | [Event](https://schema.org/Event "Event") | Upcoming or past event associated with this place, organization, or action. Supersedes [events](https://schema.org/events "events"). |
| ``` faxNumber ``` | [Text](https://schema.org/Text "Text") | The fax number. |
| ``` founder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization who founded this organization. Supersedes [founders](https://schema.org/founders "founders"). |
| ``` foundingDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was founded. |
| ``` foundingLocation ``` | [Place](https://schema.org/Place "Place") | The place where the Organization was founded. |
| ``` funder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` globalLocationNumber ``` | [Text](https://schema.org/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasCredential ``` | [EducationalOccupationalCredential](https://schema.org/EducationalOccupationalCredential "EducationalOccupationalCredential") | A credential awarded to the Person or Organization. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMemberProgram ``` | [MemberProgram](https://schema.org/MemberProgram "MemberProgram") | MemberProgram offered by an Organization, for example an eCommerce merchant or an airline. |
| ``` hasMerchantReturnPolicy ``` | [MerchantReturnPolicy](https://schema.org/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](https://schema.org/hasProductReturnPolicy "hasProductReturnPolicy"). |
| ``` hasOfferCatalog ``` | [OfferCatalog](https://schema.org/OfferCatalog "OfferCatalog") | Indicates an OfferCatalog listing for this Organization, Person, or Service. |
| ``` hasPOS ``` | [Place](https://schema.org/Place "Place") | Points-of-Sales operated by the organization or person. |
| ``` hasShippingService ``` | [ShippingService](https://schema.org/ShippingService "ShippingService") | Specification of a shipping service offered by the organization. |
| ``` interactionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](https://schema.org/interactionCount "interactionCount"). |
| ``` isicV4 ``` | [Text](https://schema.org/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| ``` iso6523Code ``` | [Text](https://schema.org/Text "Text") | An organization identifier as defined in [ISO 6523(-1)](https://en.wikipedia.org/wiki/ISO/IEC_6523). The identifier should be in the `XXXX:YYYYYY:ZZZ` or `XXXX:YYYYYY`format. Where `XXXX` is a 4 digit _ICD_ (International Code Designator), `YYYYYY` is an _OID_ (Organization Identifier) with all formatting characters (dots, dashes, spaces) removed with a maximal length of 35 characters, and `ZZZ` is an optional OPI (Organization Part Identifier) with a maximum length of 35 characters. The various components (ICD, OID, OPI) are joined with a colon character (ASCII `0x3a`). Note that many existing organization identifiers defined as attributes like [leiCode](https://schema.org/leiCode) (`0199`), [duns](https://schema.org/duns) (`0060`) or [GLN](https://schema.org/globalLocationNumber) (`0088`) can be expressed using ISO-6523. If possible, ISO-6523 codes should be preferred to populating [vatID](https://schema.org/vatID) or [taxID](https://schema.org/taxID), as ISO identifiers are less ambiguous. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` knowsAbout ``` | [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a topic that is known about - suggesting possible expertise but not implying it. We do not distinguish skill levels here, or relate this to educational content, events, objectives or [JobPosting](https://schema.org/JobPosting) descriptions. |
| ``` knowsLanguage ``` | [Language](https://schema.org/Language "Language") or [Text](https://schema.org/Text "Text") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a known language. We do not distinguish skill levels or reading/writing/speaking/signing here. Use language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). |
| ``` legalAddress ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") | The legal address of an organization which acts as the officially registered address used for legal and tax purposes. The legal address can be different from the place of operations of a business and other addresses can be part of an organization. |
| ``` legalName ``` | [Text](https://schema.org/Text "Text") | The official name of the organization, e.g. the registered company name. |
| ``` legalRepresentative ``` | [Person](https://schema.org/Person "Person") | One or multiple persons who represent this organization legally such as CEO or sole administrator. |
| ``` leiCode ``` | [Text](https://schema.org/Text "Text") | An organization identifier that uniquely identifies a legal entity as defined in ISO 17442. |
| ``` location ``` | [Place](https://schema.org/Place "Place") or [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") or [VirtualLocation](https://schema.org/VirtualLocation "VirtualLocation") | The location of, for example, where an event is happening, where an organization is located, or where an action takes place. |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` makesOffer ``` | [Offer](https://schema.org/Offer "Offer") | A pointer to products or services offered by the organization or person. Inverse property: [offeredBy](https://schema.org/offeredBy "offeredBy") |
| ``` member ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A member of an Organization or a ProgramMembership. Organizations can be members of organizations; ProgramMembership is typically for individuals. Supersedes [musicGroupMember](https://schema.org/musicGroupMember "musicGroupMember"), [members](https://schema.org/members "members"). Inverse property: [memberOf](https://schema.org/memberOf "memberOf") |
| ``` memberOf ``` | [MemberProgramTier](https://schema.org/MemberProgramTier "MemberProgramTier") or [Organization](https://schema.org/Organization "Organization") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | An Organization (or ProgramMembership) to which this Person or Organization belongs. Inverse property: [member](https://schema.org/member "member") |
| ``` naics ``` | [Text](https://schema.org/Text "Text") | The North American Industry Classification System (NAICS) code for a particular organization or business person. |
| ``` nonprofitStatus ``` | [NonprofitType](https://schema.org/NonprofitType "NonprofitType") | nonprofitStatus indicates the legal status of a non-profit organization in its primary place of business. |
| ``` numberOfEmployees ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The number of employees in an organization, e.g. business. |
| ``` ownershipFundingInfo ``` | [AboutPage](https://schema.org/AboutPage "AboutPage") or [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a description of organizational ownership structure; funding and grants. In a news/media setting, this is with particular reference to editorial independence. Note that the [funder](https://schema.org/funder) is also available and can be used to make basic funder information machine-readable. |
| ``` owns ``` | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") or [Product](https://schema.org/Product "Product") | Products owned by the organization or person. |
| ``` parentOrganization ``` | [Organization](https://schema.org/Organization "Organization") | The larger organization that this organization is a [subOrganization](https://schema.org/subOrganization) of, if any. Supersedes [branchOf](https://schema.org/branchOf "branchOf"). Inverse property: [subOrganization](https://schema.org/subOrganization "subOrganization") |
| ``` publishingPrinciples ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The publishingPrinciples property indicates (typically via [URL](https://schema.org/URL)) a document describing the editorial principles of an [Organization](https://schema.org/Organization) (or individual, e.g. a [Person](https://schema.org/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](https://schema.org/CreativeWork) (e.g. [NewsArticle](https://schema.org/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](https://schema.org/CreativeWork). While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](https://schema.org/funder)) can be expressed using schema.org terminology. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` seeks ``` | [Demand](https://schema.org/Demand "Demand") | A pointer to products or services sought by the organization or person (demand). |
| ``` skills ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A statement of knowledge, skill, ability, task or any other assertion expressing a competency that is either claimed by a person, an organization or desired or required to fulfill a role or to work in an occupation. |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` sponsor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| ``` subOrganization ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between two organizations where the first includes the second, e.g., as a subsidiary. See also: the more specific 'department' property. Inverse property: [parentOrganization](https://schema.org/parentOrganization "parentOrganization") |
| ``` taxID ``` | [Text](https://schema.org/Text "Text") | The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain. |
| ``` telephone ``` | [Text](https://schema.org/Text "Text") | The telephone number. |
| ``` unnamedSourcesPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (typically a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement about policy on use of unnamed sources and the decision process required. |
| ``` vatID ``` | [Text](https://schema.org/Text "Text") | The Value-added Tax ID of the organization or person. |
| Properties from [Place](https://schema.org/Place "Place") |
| ``` additionalProperty ``` | [PropertyValue](https://schema.org/PropertyValue "PropertyValue") | A property-value pair representing an additional characteristic of the entity, e.g. a product feature or another characteristic for which there is no matching property in schema.org. Note: Publishers should be aware that applications designed to use specific schema.org properties (e.g. https://schema.org/width, https://schema.org/color, https://schema.org/gtin13, ...) will typically expect such data to be provided using those properties, rather than using the generic property/value mechanism. |
| ``` address ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") | Physical address of the item. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` amenityFeature ``` | [LocationFeatureSpecification](https://schema.org/LocationFeatureSpecification "LocationFeatureSpecification") | An amenity feature (e.g. a characteristic or service) of the Accommodation. This generic property does not make a statement about whether the feature is included in an offer for the main accommodation or available at extra costs. |
| ``` branchCode ``` | [Text](https://schema.org/Text "Text") | A short textual code (also called "store code") that uniquely identifies a place of business. The code is typically assigned by the parentOrganization and used in structured URLs. For example, in the URL http://www.starbucks.co.uk/store-locator/etc/detail/3047 the code "3047" is a branchCode for a particular branch. |
| ``` containedInPlace ``` | [Place](https://schema.org/Place "Place") | The basic containment relation between a place and one that contains it. Supersedes [containedIn](https://schema.org/containedIn "containedIn"). Inverse property: [containsPlace](https://schema.org/containsPlace "containsPlace") |
| ``` containsPlace ``` | [Place](https://schema.org/Place "Place") | The basic containment relation between a place and another that it contains. Inverse property: [containedInPlace](https://schema.org/containedInPlace "containedInPlace") |
| ``` event ``` | [Event](https://schema.org/Event "Event") | Upcoming or past event associated with this place, organization, or action. Supersedes [events](https://schema.org/events "events"). |
| ``` faxNumber ``` | [Text](https://schema.org/Text "Text") | The fax number. |
| ``` geo ``` | [GeoCoordinates](https://schema.org/GeoCoordinates "GeoCoordinates") or [GeoShape](https://schema.org/GeoShape "GeoShape") | The geo coordinates of the place. |
| ``` geoContains ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a containing geometry to a contained geometry. "a contains b iff no points of b lie in the exterior of a, and at least one point of the interior of b lies in the interior of a". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCoveredBy ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that covers it. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCovers ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a covering geometry to a covered geometry. "Every point of b is a point of (the interior or boundary of) a". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCrosses ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that crosses it: "a crosses b: they have some but not all interior points in common, and the dimension of the intersection is less than that of at least one of them". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoDisjoint ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) are topologically disjoint: "they have no point in common. They form a set of disconnected geometries." (A symmetric relationship, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM).) |
| ``` geoEquals ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) are topologically equal, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). "Two geometries are topologically equal if their interiors intersect and no part of the interior or boundary of one geometry intersects the exterior of the other" (a symmetric relationship). |
| ``` geoIntersects ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) have at least one point in common. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoOverlaps ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that geospatially overlaps it, i.e. they have some but not all points in common. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoTouches ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) touch: "they have at least one boundary point in common, but no interior points." (A symmetric relationship, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM).) |
| ``` geoWithin ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to one that contains it, i.e. it is inside (i.e. within) its interior. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` globalLocationNumber ``` | [Text](https://schema.org/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasDriveThroughService ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether some facility (e.g. [FoodEstablishment](https://schema.org/FoodEstablishment), [CovidTestingFacility](https://schema.org/CovidTestingFacility)) offers a service that can be used by driving through in a car. In the case of [CovidTestingFacility](https://schema.org/CovidTestingFacility) such facilities could potentially help with social distancing from other potentially-infected users. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMap ``` | [Map](https://schema.org/Map "Map") or [URL](https://schema.org/URL "URL") | A URL to a map of the place. Supersedes [maps](https://schema.org/maps "maps"), [map](https://schema.org/map "map"). |
| ``` isAccessibleForFree ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](https://schema.org/free "free"). |
| ``` isicV4 ``` | [Text](https://schema.org/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` latitude ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The latitude of a location. For example `37.42242` ([WGS 84](https://en.wikipedia.org/wiki/World_Geodetic_System)). |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` longitude ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The longitude of a location. For example `-122.08585` ([WGS 84](https://en.wikipedia.org/wiki/World_Geodetic_System)). |
| ``` maximumAttendeeCapacity ``` | [Integer](https://schema.org/Integer "Integer") | The total number of individuals that may attend an event or venue. |
| ``` openingHoursSpecification ``` | [OpeningHoursSpecification](https://schema.org/OpeningHoursSpecification "OpeningHoursSpecification") | The opening hours of a certain place. |
| ``` photo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [Photograph](https://schema.org/Photograph "Photograph") | A photograph of this place. Supersedes [photos](https://schema.org/photos "photos"). |
| ``` publicAccess ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the [Place](https://schema.org/Place) is open to public visitors. If this property is omitted there is no assumed default boolean value. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` smokingAllowed ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether it is allowed to smoke in the place, e.g. in the restaurant, hotel or hotel room. |
| ``` specialOpeningHoursSpecification ``` | [OpeningHoursSpecification](https://schema.org/OpeningHoursSpecification "OpeningHoursSpecification") | The special opening hours of a certain place. Use this to explicitly override general opening hours brought in scope by [openingHoursSpecification](https://schema.org/openingHoursSpecification) or [openingHours](https://schema.org/openingHours). |
| ``` telephone ``` | [Text](https://schema.org/Text "Text") | The telephone number. |
| ``` tourBookingPage ``` | [URL](https://schema.org/URL "URL") | A page providing information on how to book a tour of some [Place](https://schema.org/Place), such as an [Accommodation](https://schema.org/Accommodation) or [ApartmentComplex](https://schema.org/ApartmentComplex) in a real estate setting, as well as other kinds of tours as appropriate. |
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

Instances of [LocalBusiness](https://schema.org/LocalBusiness "LocalBusiness") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [announcementLocation](https://schema.org/announcementLocation "announcementLocation") | [SpecialAnnouncement](https://schema.org/SpecialAnnouncement "SpecialAnnouncement") | Indicates a specific [CivicStructure](https://schema.org/CivicStructure) or [LocalBusiness](https://schema.org/LocalBusiness) associated with the SpecialAnnouncement. For example, a specific testing facility or business with special opening hours. For a larger geographic region like a quarantine of an entire region, use [spatialCoverage](https://schema.org/spatialCoverage). |

#### More specific Types

*   [AnimalShelter](https://schema.org/AnimalShelter "AnimalShelter")
*   [ArchiveOrganization](https://schema.org/ArchiveOrganization "ArchiveOrganization")
*   [AutomotiveBusiness](https://schema.org/AutomotiveBusiness "AutomotiveBusiness")
*   [ChildCare](https://schema.org/ChildCare "ChildCare")
*   [Dentist](https://schema.org/Dentist "Dentist")
*   [DryCleaningOrLaundry](https://schema.org/DryCleaningOrLaundry "DryCleaningOrLaundry")
*   [EmergencyService](https://schema.org/EmergencyService "EmergencyService")
*   [EmploymentAgency](https://schema.org/EmploymentAgency "EmploymentAgency")
*   [EntertainmentBusiness](https://schema.org/EntertainmentBusiness "EntertainmentBusiness")
*   [FinancialService](https://schema.org/FinancialService "FinancialService")
*   [FoodEstablishment](https://schema.org/FoodEstablishment "FoodEstablishment")
*   [GovernmentOffice](https://schema.org/GovernmentOffice "GovernmentOffice")
*   [HealthAndBeautyBusiness](https://schema.org/HealthAndBeautyBusiness "HealthAndBeautyBusiness")
*   [HomeAndConstructionBusiness](https://schema.org/HomeAndConstructionBusiness "HomeAndConstructionBusiness")
*   [InternetCafe](https://schema.org/InternetCafe "InternetCafe")
*   [LegalService](https://schema.org/LegalService "LegalService")
*   [Library](https://schema.org/Library "Library")
*   [LodgingBusiness](https://schema.org/LodgingBusiness "LodgingBusiness")
*   [MedicalBusiness](https://schema.org/MedicalBusiness "MedicalBusiness")
*   [ProfessionalService](https://schema.org/ProfessionalService "ProfessionalService")
*   [RadioStation](https://schema.org/RadioStation "RadioStation")
*   [RealEstateAgent](https://schema.org/RealEstateAgent "RealEstateAgent")
*   [RecyclingCenter](https://schema.org/RecyclingCenter "RecyclingCenter")
*   [SelfStorage](https://schema.org/SelfStorage "SelfStorage")
*   [ShoppingCenter](https://schema.org/ShoppingCenter "ShoppingCenter")
*   [SportsActivityLocation](https://schema.org/SportsActivityLocation "SportsActivityLocation")
*   [Store](https://schema.org/Store "Store")
*   [TelevisionStation](https://schema.org/TelevisionStation "TelevisionStation")
*   [TouristInformationCenter](https://schema.org/TouristInformationCenter "TouristInformationCenter")
*   [TravelAgency](https://schema.org/TravelAgency "TravelAgency")

### Examples
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Restaurant",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Sunnyvale",
        "addressRegion": "CA",
        "postalCode": "94086",
        "streetAddress": "1901 Lemur Ave"
      },
      "aggregateRating": {
        "@type": "AggregateRating",
        "ratingValue": "4",
        "reviewCount": "250"
      },
      "name": "GreatFood",
      "openingHours": [
        "Mo-Sa 11:00-14:30",
        "Mo-Th 17:00-21:30",
        "Fr-Sa 17:00-22:00"
      ],
      "priceRange": "$$",
      "servesCuisine": [
        "Middle Eastern",
        "Mediterranean"
      ],
      "telephone": "(408) 714-1489",
      "url": "http://www.greatfood.com"
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "LocalBusiness",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Mexico Beach",
        "addressRegion": "FL",
        "streetAddress": "3102 Highway 98"
      },
      "description": "A superb collection of fine gifts and clothing to accent your stay in Mexico Beach.",
      "name": "Beachwalk Beachwear & Giftware",
      "telephone": "850-648-4200"
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
```Title: Offer - Schema.org Type

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
```Title: Organization - Schema.org Type

URL Source: https://schema.org/Organization

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

An organization such as a school, NGO, corporation, club, etc.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Organization](https://schema.org/Organization "Organization") |
| ``` acceptedPaymentMethod ``` | [LoanOrCredit](https://schema.org/LoanOrCredit "LoanOrCredit") or [PaymentMethod](https://schema.org/PaymentMethod "PaymentMethod") or [Text](https://schema.org/Text "Text") | The payment method(s) that are accepted in general by an organization, or for some specific demand or offer. |
| ``` actionableFeedbackPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) or other news-related [Organization](https://schema.org/Organization), a statement about public engagement activities (for news media, the newsroom’s), including involving the public - digitally or otherwise -- in coverage decisions, reporting and activities after publication. |
| ``` address ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") | Physical address of the item. |
| ``` agentInteractionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of completed interactions for this entity, in a particular role (the 'agent'), in a particular action (indicated in the statistic), and in a particular context (i.e. interactionService). |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` alumni ``` | [Person](https://schema.org/Person "Person") | Alumni of an organization. Inverse property: [alumniOf](https://schema.org/alumniOf "alumniOf") |
| ``` areaServed ``` | [AdministrativeArea](https://schema.org/AdministrativeArea "AdministrativeArea") or [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](https://schema.org/serviceArea "serviceArea"). |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` brand ``` | [Brand](https://schema.org/Brand "Brand") or [Organization](https://schema.org/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| ``` companyRegistration ``` | [Certification](https://schema.org/Certification "Certification") | The official registration number of a business including the organization that issued it such as Company House or Chamber of Commerce. |
| ``` contactPoint ``` | [ContactPoint](https://schema.org/ContactPoint "ContactPoint") | A contact point for a person or organization. Supersedes [contactPoints](https://schema.org/contactPoints "contactPoints"). |
| ``` correctionsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (e.g. [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement describing (in news media, the newsroom’s) disclosure and correction policy for errors. |
| ``` department ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between an organization and a department of that organization, also described as an organization (allowing different urls, logos, opening hours). For example: a store with a pharmacy, or a bakery with a cafe. |
| ``` dissolutionDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was dissolved. |
| ``` diversityPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement on diversity policy by an [Organization](https://schema.org/Organization) e.g. a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization). For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), a statement describing the newsroom’s diversity policy on both staffing and sources, typically providing staffing data. |
| ``` diversityStaffingReport ``` | [Article](https://schema.org/Article "Article") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a report on staffing diversity issues. In a news context this might be for example ASNE or RTDNA (US) reports, or self-reported. |
| ``` duns ``` | [Text](https://schema.org/Text "Text") | The Dun & Bradstreet DUNS number for identifying an organization or business person. |
| ``` email ``` | [Text](https://schema.org/Text "Text") | Email address. |
| ``` employee ``` | [Person](https://schema.org/Person "Person") | Someone working for this organization. Supersedes [employees](https://schema.org/employees "employees"). |
| ``` ethicsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement about ethics policy, e.g. of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) regarding journalistic and publishing practices, or of a [Restaurant](https://schema.org/Restaurant), a page describing food source policies. In the case of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), an ethicsPolicy is typically a statement describing the personal, organizational, and corporate standards of behavior expected by the organization. |
| ``` event ``` | [Event](https://schema.org/Event "Event") | Upcoming or past event associated with this place, organization, or action. Supersedes [events](https://schema.org/events "events"). |
| ``` faxNumber ``` | [Text](https://schema.org/Text "Text") | The fax number. |
| ``` founder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization who founded this organization. Supersedes [founders](https://schema.org/founders "founders"). |
| ``` foundingDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was founded. |
| ``` foundingLocation ``` | [Place](https://schema.org/Place "Place") | The place where the Organization was founded. |
| ``` funder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` globalLocationNumber ``` | [Text](https://schema.org/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasCredential ``` | [EducationalOccupationalCredential](https://schema.org/EducationalOccupationalCredential "EducationalOccupationalCredential") | A credential awarded to the Person or Organization. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMemberProgram ``` | [MemberProgram](https://schema.org/MemberProgram "MemberProgram") | MemberProgram offered by an Organization, for example an eCommerce merchant or an airline. |
| ``` hasMerchantReturnPolicy ``` | [MerchantReturnPolicy](https://schema.org/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](https://schema.org/hasProductReturnPolicy "hasProductReturnPolicy"). |
| ``` hasOfferCatalog ``` | [OfferCatalog](https://schema.org/OfferCatalog "OfferCatalog") | Indicates an OfferCatalog listing for this Organization, Person, or Service. |
| ``` hasPOS ``` | [Place](https://schema.org/Place "Place") | Points-of-Sales operated by the organization or person. |
| ``` hasShippingService ``` | [ShippingService](https://schema.org/ShippingService "ShippingService") | Specification of a shipping service offered by the organization. |
| ``` interactionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](https://schema.org/interactionCount "interactionCount"). |
| ``` isicV4 ``` | [Text](https://schema.org/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| ``` iso6523Code ``` | [Text](https://schema.org/Text "Text") | An organization identifier as defined in [ISO 6523(-1)](https://en.wikipedia.org/wiki/ISO/IEC_6523). The identifier should be in the `XXXX:YYYYYY:ZZZ` or `XXXX:YYYYYY`format. Where `XXXX` is a 4 digit _ICD_ (International Code Designator), `YYYYYY` is an _OID_ (Organization Identifier) with all formatting characters (dots, dashes, spaces) removed with a maximal length of 35 characters, and `ZZZ` is an optional OPI (Organization Part Identifier) with a maximum length of 35 characters. The various components (ICD, OID, OPI) are joined with a colon character (ASCII `0x3a`). Note that many existing organization identifiers defined as attributes like [leiCode](https://schema.org/leiCode) (`0199`), [duns](https://schema.org/duns) (`0060`) or [GLN](https://schema.org/globalLocationNumber) (`0088`) can be expressed using ISO-6523. If possible, ISO-6523 codes should be preferred to populating [vatID](https://schema.org/vatID) or [taxID](https://schema.org/taxID), as ISO identifiers are less ambiguous. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` knowsAbout ``` | [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a topic that is known about - suggesting possible expertise but not implying it. We do not distinguish skill levels here, or relate this to educational content, events, objectives or [JobPosting](https://schema.org/JobPosting) descriptions. |
| ``` knowsLanguage ``` | [Language](https://schema.org/Language "Language") or [Text](https://schema.org/Text "Text") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a known language. We do not distinguish skill levels or reading/writing/speaking/signing here. Use language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). |
| ``` legalAddress ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") | The legal address of an organization which acts as the officially registered address used for legal and tax purposes. The legal address can be different from the place of operations of a business and other addresses can be part of an organization. |
| ``` legalName ``` | [Text](https://schema.org/Text "Text") | The official name of the organization, e.g. the registered company name. |
| ``` legalRepresentative ``` | [Person](https://schema.org/Person "Person") | One or multiple persons who represent this organization legally such as CEO or sole administrator. |
| ``` leiCode ``` | [Text](https://schema.org/Text "Text") | An organization identifier that uniquely identifies a legal entity as defined in ISO 17442. |
| ``` location ``` | [Place](https://schema.org/Place "Place") or [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") or [VirtualLocation](https://schema.org/VirtualLocation "VirtualLocation") | The location of, for example, where an event is happening, where an organization is located, or where an action takes place. |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` makesOffer ``` | [Offer](https://schema.org/Offer "Offer") | A pointer to products or services offered by the organization or person. Inverse property: [offeredBy](https://schema.org/offeredBy "offeredBy") |
| ``` member ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A member of an Organization or a ProgramMembership. Organizations can be members of organizations; ProgramMembership is typically for individuals. Supersedes [musicGroupMember](https://schema.org/musicGroupMember "musicGroupMember"), [members](https://schema.org/members "members"). Inverse property: [memberOf](https://schema.org/memberOf "memberOf") |
| ``` memberOf ``` | [MemberProgramTier](https://schema.org/MemberProgramTier "MemberProgramTier") or [Organization](https://schema.org/Organization "Organization") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | An Organization (or ProgramMembership) to which this Person or Organization belongs. Inverse property: [member](https://schema.org/member "member") |
| ``` naics ``` | [Text](https://schema.org/Text "Text") | The North American Industry Classification System (NAICS) code for a particular organization or business person. |
| ``` nonprofitStatus ``` | [NonprofitType](https://schema.org/NonprofitType "NonprofitType") | nonprofitStatus indicates the legal status of a non-profit organization in its primary place of business. |
| ``` numberOfEmployees ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The number of employees in an organization, e.g. business. |
| ``` ownershipFundingInfo ``` | [AboutPage](https://schema.org/AboutPage "AboutPage") or [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a description of organizational ownership structure; funding and grants. In a news/media setting, this is with particular reference to editorial independence. Note that the [funder](https://schema.org/funder) is also available and can be used to make basic funder information machine-readable. |
| ``` owns ``` | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") or [Product](https://schema.org/Product "Product") | Products owned by the organization or person. |
| ``` parentOrganization ``` | [Organization](https://schema.org/Organization "Organization") | The larger organization that this organization is a [subOrganization](https://schema.org/subOrganization) of, if any. Supersedes [branchOf](https://schema.org/branchOf "branchOf"). Inverse property: [subOrganization](https://schema.org/subOrganization "subOrganization") |
| ``` publishingPrinciples ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The publishingPrinciples property indicates (typically via [URL](https://schema.org/URL)) a document describing the editorial principles of an [Organization](https://schema.org/Organization) (or individual, e.g. a [Person](https://schema.org/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](https://schema.org/CreativeWork) (e.g. [NewsArticle](https://schema.org/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](https://schema.org/CreativeWork). While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](https://schema.org/funder)) can be expressed using schema.org terminology. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` seeks ``` | [Demand](https://schema.org/Demand "Demand") | A pointer to products or services sought by the organization or person (demand). |
| ``` skills ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A statement of knowledge, skill, ability, task or any other assertion expressing a competency that is either claimed by a person, an organization or desired or required to fulfill a role or to work in an occupation. |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` sponsor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| ``` subOrganization ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between two organizations where the first includes the second, e.g., as a subsidiary. See also: the more specific 'department' property. Inverse property: [parentOrganization](https://schema.org/parentOrganization "parentOrganization") |
| ``` taxID ``` | [Text](https://schema.org/Text "Text") | The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain. |
| ``` telephone ``` | [Text](https://schema.org/Text "Text") | The telephone number. |
| ``` unnamedSourcesPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (typically a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement about policy on use of unnamed sources and the decision process required. |
| ``` vatID ``` | [Text](https://schema.org/Text "Text") | The Value-added Tax ID of the organization or person. |
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

Instances of [Organization](https://schema.org/Organization "Organization") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [acquiredFrom](https://schema.org/acquiredFrom "acquiredFrom") | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") | The organization or person from which the product was acquired. |
| [affiliation](https://schema.org/affiliation "affiliation") | [Person](https://schema.org/Person "Person") | An organization that this person is affiliated with. For example, a school/university, a club, or a team. |
| [agent](https://schema.org/agent "agent") | [Action](https://schema.org/Action "Action") | The direct performer or driver of the action (animate or inanimate). E.g. _John_ wrote a book. |
| [alumniOf](https://schema.org/alumniOf "alumniOf") | [Person](https://schema.org/Person "Person") | An organization that the person is an alumni of. |
| [attendee](https://schema.org/attendee "attendee") | [Event](https://schema.org/Event "Event") | A person or organization attending the event. |
| [attendees](https://schema.org/attendees "attendees") | [Event](https://schema.org/Event "Event") | A person attending the event. |
| [authenticator](https://schema.org/authenticator "authenticator") | [MediaSubscription](https://schema.org/MediaSubscription "MediaSubscription") | The Organization responsible for authenticating the user's subscription. For example, many media apps require a cable/satellite provider to authenticate your subscription before playing media. |
| [author](https://schema.org/author "author") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Rating](https://schema.org/Rating "Rating") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| [bccRecipient](https://schema.org/bccRecipient "bccRecipient") | [Message](https://schema.org/Message "Message") | A sub property of recipient. The recipient blind copied on a message. |
| [bookingAgent](https://schema.org/bookingAgent "bookingAgent") | [Reservation](https://schema.org/Reservation "Reservation") | 'bookingAgent' is an out-dated term indicating a 'broker' that serves as a booking agent. |
| [branchOf](https://schema.org/branchOf "branchOf") | [LocalBusiness](https://schema.org/LocalBusiness "LocalBusiness") | The larger organization that this local business is a branch of, if any. Not to be confused with (anatomical) [branch](https://schema.org/branch). |
| [brand](https://schema.org/brand "brand") | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") or [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| [broadcastAffiliateOf](https://schema.org/broadcastAffiliateOf "broadcastAffiliateOf") | [BroadcastService](https://schema.org/BroadcastService "BroadcastService") | The media network(s) whose content is broadcast on this station. |
| [broadcaster](https://schema.org/broadcaster "broadcaster") | [BroadcastService](https://schema.org/BroadcastService "BroadcastService") | The organization owning or operating the broadcast service. |
| [broker](https://schema.org/broker "broker") | [Invoice](https://schema.org/Invoice "Invoice") or [Order](https://schema.org/Order "Order") or [Reservation](https://schema.org/Reservation "Reservation") or [Service](https://schema.org/Service "Service") | An entity that arranges for an exchange between a buyer and a seller. In most cases a broker never acquires or releases ownership of a product or service involved in an exchange. If it is not clear whether an entity is a broker, seller, or buyer, the latter two terms are preferred. |
| [buyer](https://schema.org/buyer "buyer") | [SellAction](https://schema.org/SellAction "SellAction") | A sub property of participant. The participant/person/organization that bought the object. |
| [carrier](https://schema.org/carrier "carrier") | [Flight](https://schema.org/Flight "Flight") or [ParcelDelivery](https://schema.org/ParcelDelivery "ParcelDelivery") | 'carrier' is an out-dated term indicating the 'provider' for parcel delivery and flights. |
| [ccRecipient](https://schema.org/ccRecipient "ccRecipient") | [Message](https://schema.org/Message "Message") | A sub property of recipient. The recipient copied on a message. |
| [claimInterpreter](https://schema.org/claimInterpreter "claimInterpreter") | [Claim](https://schema.org/Claim "Claim") | For a [Claim](https://schema.org/Claim) interpreted from [MediaObject](https://schema.org/MediaObject) content, the [interpretedAsClaim](https://schema.org/interpretedAsClaim) property can be used to indicate a claim contained, implied or refined from the content of a [MediaObject](https://schema.org/MediaObject). |
| [composer](https://schema.org/composer "composer") | [Event](https://schema.org/Event "Event") or [MusicComposition](https://schema.org/MusicComposition "MusicComposition") | The person or organization who wrote a composition, or who is the composer of a work performed at some event. |
| [contributor](https://schema.org/contributor "contributor") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") | A secondary contributor to the CreativeWork or Event. |
| [copyrightHolder](https://schema.org/copyrightHolder "copyrightHolder") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The party holding the legal copyright to the CreativeWork. |
| [creator](https://schema.org/creator "creator") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [UserComments](https://schema.org/UserComments "UserComments") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| [creditedTo](https://schema.org/creditedTo "creditedTo") | [MusicRelease](https://schema.org/MusicRelease "MusicRelease") | The group the release is credited to if different than the byArtist. For example, Red and Blue is credited to "Stefani Germanotta Band", but by Lady Gaga. |
| [customer](https://schema.org/customer "customer") | [Invoice](https://schema.org/Invoice "Invoice") or [Order](https://schema.org/Order "Order") | Party placing the order or paying the invoice. |
| [department](https://schema.org/department "department") | [Organization](https://schema.org/Organization "Organization") | A relationship between an organization and a department of that organization, also described as an organization (allowing different urls, logos, opening hours). For example: a store with a pharmacy, or a bakery with a cafe. |
| [eligibleWithSupplier](https://schema.org/eligibleWithSupplier "eligibleWithSupplier") | [FinancialIncentive](https://schema.org/FinancialIncentive "FinancialIncentive") | The supplier of the incentivized item/service for which the incentive is valid for such as a utility company, merchant, or contractor. |
| [employmentUnit](https://schema.org/employmentUnit "employmentUnit") | [JobPosting](https://schema.org/JobPosting "JobPosting") | Indicates the department, unit and/or facility where the employee reports and/or in which the job is to be performed. |
| [endorsee](https://schema.org/endorsee "endorsee") | [EndorseAction](https://schema.org/EndorseAction "EndorseAction") | A sub property of participant. The person/organization being supported. |
| [endorsers](https://schema.org/endorsers "endorsers") | [Diet](https://schema.org/Diet "Diet") | People or organizations that endorse the plan. |
| [followee](https://schema.org/followee "followee") | [FollowAction](https://schema.org/FollowAction "FollowAction") | A sub property of object. The person or organization being followed. |
| [founder](https://schema.org/founder "founder") | [Organization](https://schema.org/Organization "Organization") | A person or organization who founded this organization. |
| [fundedItem](https://schema.org/fundedItem "fundedItem") | [Grant](https://schema.org/Grant "Grant") | Indicates something directly or indirectly funded or sponsored through a [Grant](https://schema.org/Grant). See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). |
| [funder](https://schema.org/funder "funder") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") or [Grant](https://schema.org/Grant "Grant") or [MonetaryGrant](https://schema.org/MonetaryGrant "MonetaryGrant") or [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| [grantee](https://schema.org/grantee "grantee") | [DigitalDocumentPermission](https://schema.org/DigitalDocumentPermission "DigitalDocumentPermission") | The person, organization, contact point, or audience that has been granted this permission. |
| [hiringOrganization](https://schema.org/hiringOrganization "hiringOrganization") | [JobPosting](https://schema.org/JobPosting "JobPosting") | Organization or Person offering the job position. |
| [hostingOrganization](https://schema.org/hostingOrganization "hostingOrganization") | [MemberProgram](https://schema.org/MemberProgram "MemberProgram") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | The Organization (airline, travelers' club, retailer, etc.) the membership is made with or which offers the MemberProgram. |
| [issuedBy](https://schema.org/issuedBy "issuedBy") | [Certification](https://schema.org/Certification "Certification") or [Permit](https://schema.org/Permit "Permit") or [Ticket](https://schema.org/Ticket "Ticket") | The organization issuing the item, for example a [Permit](https://schema.org/Permit), [Ticket](https://schema.org/Ticket), or [Certification](https://schema.org/Certification). |
| [landlord](https://schema.org/landlord "landlord") | [RentAction](https://schema.org/RentAction "RentAction") | A sub property of participant. The owner of the real estate property. |
| [legislationCountersignedBy](https://schema.org/legislationCountersignedBy "legislationCountersignedBy") | [Legislation](https://schema.org/Legislation "Legislation") | The person or organization that countersigned the legislation. Depending on the legal context, a countersignature can indicate that the signed authority undertakes to assume responsibility for texts emanating from a person who is inviolable and irresponsible, (for example a King, Grand Duc or President), or that the authority is in charge of the implementation of the text. |
| [legislationPassedBy](https://schema.org/legislationPassedBy "legislationPassedBy") | [Legislation](https://schema.org/Legislation "Legislation") | The person or organization that originally passed or made the law: typically parliament (for primary legislation) or government (for secondary legislation). This indicates the "legal author" of the law, as opposed to its physical author. |
| [legislationResponsible](https://schema.org/legislationResponsible "legislationResponsible") | [Legislation](https://schema.org/Legislation "Legislation") | An individual or organization that has some kind of responsibility for the legislation. Typically the ministry who is/was in charge of elaborating the legislation, or the adressee for potential questions about the legislation once it is published. |
| [lender](https://schema.org/lender "lender") | [BorrowAction](https://schema.org/BorrowAction "BorrowAction") | A sub property of participant. The person that lends the object being borrowed. |
| [maintainer](https://schema.org/maintainer "maintainer") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A maintainer of a [Dataset](https://schema.org/Dataset), software package ([SoftwareApplication](https://schema.org/SoftwareApplication)), or other [Project](https://schema.org/Project). A maintainer is a [Person](https://schema.org/Person) or [Organization](https://schema.org/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](https://schema.org/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](https://schema.org/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](https://schema.org/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| [manufacturer](https://schema.org/manufacturer "manufacturer") | [Product](https://schema.org/Product "Product") | The manufacturer of the product. |
| [member](https://schema.org/member "member") | [Organization](https://schema.org/Organization "Organization") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | A member of an Organization or a ProgramMembership. Organizations can be members of organizations; ProgramMembership is typically for individuals. |
| [memberOf](https://schema.org/memberOf "memberOf") | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | An Organization (or ProgramMembership) to which this Person or Organization belongs. |
| [members](https://schema.org/members "members") | [Organization](https://schema.org/Organization "Organization") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | A member of this organization. |
| [merchant](https://schema.org/merchant "merchant") | [Order](https://schema.org/Order "Order") | 'merchant' is an out-dated term for 'seller'. |
| [offeredBy](https://schema.org/offeredBy "offeredBy") | [Offer](https://schema.org/Offer "Offer") | A pointer to the organization or person making the offer. |
| [organizer](https://schema.org/organizer "organizer") | [Event](https://schema.org/Event "Event") | An organizer of an Event. |
| [parentOrganization](https://schema.org/parentOrganization "parentOrganization") | [Organization](https://schema.org/Organization "Organization") | The larger organization that this organization is a [subOrganization](https://schema.org/subOrganization) of, if any. |
| [participant](https://schema.org/participant "participant") | [Action](https://schema.org/Action "Action") | Other co-agents that participated in the action indirectly. E.g. John wrote a book with _Steve_. |
| [performer](https://schema.org/performer "performer") | [Event](https://schema.org/Event "Event") | A performer at the event—for example, a presenter, musician, musical group or actor. |
| [performers](https://schema.org/performers "performers") | [Event](https://schema.org/Event "Event") | The main performer or performers of the event—for example, a presenter, musician, or actor. |
| [producer](https://schema.org/producer "producer") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| [productionCompany](https://schema.org/productionCompany "productionCompany") | [CreativeWorkSeason](https://schema.org/CreativeWorkSeason "CreativeWorkSeason") or [Episode](https://schema.org/Episode "Episode") or [MediaObject](https://schema.org/MediaObject "MediaObject") or [Movie](https://schema.org/Movie "Movie") or [MovieSeries](https://schema.org/MovieSeries "MovieSeries") or [RadioSeries](https://schema.org/RadioSeries "RadioSeries") or [TVSeries](https://schema.org/TVSeries "TVSeries") or [VideoGameSeries](https://schema.org/VideoGameSeries "VideoGameSeries") | The production company or studio responsible for the item, e.g. series, video game, episode etc. |
| [provider](https://schema.org/provider "provider") | [Action](https://schema.org/Action "Action") or [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [EducationalOccupationalProgram](https://schema.org/EducationalOccupationalProgram "EducationalOccupationalProgram") or [FinancialIncentive](https://schema.org/FinancialIncentive "FinancialIncentive") or [Invoice](https://schema.org/Invoice "Invoice") or [ParcelDelivery](https://schema.org/ParcelDelivery "ParcelDelivery") or [Reservation](https://schema.org/Reservation "Reservation") or [Service](https://schema.org/Service "Service") or [Trip](https://schema.org/Trip "Trip") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. |
| [publishedBy](https://schema.org/publishedBy "publishedBy") | [PublicationEvent](https://schema.org/PublicationEvent "PublicationEvent") | An agent associated with the publication event. |
| [publisher](https://schema.org/publisher "publisher") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [FinancialIncentive](https://schema.org/FinancialIncentive "FinancialIncentive") | The publisher of the article in question. |
| [publisherImprint](https://schema.org/publisherImprint "publisherImprint") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The publishing division which published the comic. |
| [recipient](https://schema.org/recipient "recipient") | [AuthorizeAction](https://schema.org/AuthorizeAction "AuthorizeAction") or [CommunicateAction](https://schema.org/CommunicateAction "CommunicateAction") or [DonateAction](https://schema.org/DonateAction "DonateAction") or [GiveAction](https://schema.org/GiveAction "GiveAction") or [Message](https://schema.org/Message "Message") or [PayAction](https://schema.org/PayAction "PayAction") or [ReturnAction](https://schema.org/ReturnAction "ReturnAction") or [SendAction](https://schema.org/SendAction "SendAction") or [TipAction](https://schema.org/TipAction "TipAction") | A sub property of participant. The participant who is at the receiving end of the action. |
| [recognizedBy](https://schema.org/recognizedBy "recognizedBy") | [EducationalOccupationalCredential](https://schema.org/EducationalOccupationalCredential "EducationalOccupationalCredential") | An organization that acknowledges the validity, value or utility of a credential. Note: recognition may include a process of quality assurance or accreditation. |
| [recognizingAuthority](https://schema.org/recognizingAuthority "recognizingAuthority") | [MedicalEntity](https://schema.org/MedicalEntity "MedicalEntity") | If applicable, the organization that officially recognizes this entity as part of its endorsed system of medicine. |
| [recordLabel](https://schema.org/recordLabel "recordLabel") | [MusicRelease](https://schema.org/MusicRelease "MusicRelease") | The label that issued the release. |
| [reviewedBy](https://schema.org/reviewedBy "reviewedBy") | [WebPage](https://schema.org/WebPage "WebPage") | People or organizations that have reviewed the content on this web page for accuracy and/or completeness. |
| [sdPublisher](https://schema.org/sdPublisher "sdPublisher") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](https://schema.org/sdPublisher) property helps make such practices more explicit. |
| [seller](https://schema.org/seller "seller") | [BuyAction](https://schema.org/BuyAction "BuyAction") or [Demand](https://schema.org/Demand "Demand") or [Flight](https://schema.org/Flight "Flight") or [Offer](https://schema.org/Offer "Offer") or [Order](https://schema.org/Order "Order") | An entity which offers (sells / leases / lends / loans) the services / goods. A seller may also be a provider. |
| [sender](https://schema.org/sender "sender") | [Message](https://schema.org/Message "Message") or [ReceiveAction](https://schema.org/ReceiveAction "ReceiveAction") | A sub property of participant. The participant who is at the sending end of the action. |
| [serviceOperator](https://schema.org/serviceOperator "serviceOperator") | [GovernmentService](https://schema.org/GovernmentService "GovernmentService") | The operating organization, if different from the provider. This enables the representation of services that are provided by an organization, but operated by another organization like a subcontractor. |
| [sourceOrganization](https://schema.org/sourceOrganization "sourceOrganization") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The Organization on whose behalf the creator was working. |
| [spokenByCharacter](https://schema.org/spokenByCharacter "spokenByCharacter") | [Quotation](https://schema.org/Quotation "Quotation") | The (e.g. fictional) character, Person or Organization to whom the quotation is attributed within the containing CreativeWork. |
| [sponsor](https://schema.org/sponsor "sponsor") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") or [Grant](https://schema.org/Grant "Grant") or [MedicalStudy](https://schema.org/MedicalStudy "MedicalStudy") or [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| [subOrganization](https://schema.org/subOrganization "subOrganization") | [Organization](https://schema.org/Organization "Organization") | A relationship between two organizations where the first includes the second, e.g., as a subsidiary. See also: the more specific 'department' property. |
| [toRecipient](https://schema.org/toRecipient "toRecipient") | [Message](https://schema.org/Message "Message") | A sub property of recipient. The recipient who was directly sent the message. |
| [translator](https://schema.org/translator "translator") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Event](https://schema.org/Event "Event") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| [underName](https://schema.org/underName "underName") | [Reservation](https://schema.org/Reservation "Reservation") or [Ticket](https://schema.org/Ticket "Ticket") | The person or organization the reservation or ticket is for. |
| [vendor](https://schema.org/vendor "vendor") | [BuyAction](https://schema.org/BuyAction "BuyAction") | 'vendor' is an earlier term for 'seller'. |
| [worksFor](https://schema.org/worksFor "worksFor") | [Person](https://schema.org/Person "Person") | Organizations that the person works for. |

#### More specific Types

*   [Airline](https://schema.org/Airline "Airline")
*   [Consortium](https://schema.org/Consortium "Consortium")
*   [Cooperative](https://schema.org/Cooperative "Cooperative")
*   [Corporation](https://schema.org/Corporation "Corporation")
*   [EducationalOrganization](https://schema.org/EducationalOrganization "EducationalOrganization")
*   [FundingScheme](https://schema.org/FundingScheme "FundingScheme")
*   [GovernmentOrganization](https://schema.org/GovernmentOrganization "GovernmentOrganization")
*   [LibrarySystem](https://schema.org/LibrarySystem "LibrarySystem")
*   [LocalBusiness](https://schema.org/LocalBusiness "LocalBusiness")
*   [MedicalOrganization](https://schema.org/MedicalOrganization "MedicalOrganization")
*   [NGO](https://schema.org/NGO "NGO")
*   [NewsMediaOrganization](https://schema.org/NewsMediaOrganization "NewsMediaOrganization")
*   [OnlineBusiness](https://schema.org/OnlineBusiness "OnlineBusiness")
*   [PerformingGroup](https://schema.org/PerformingGroup "PerformingGroup")
*   [PoliticalParty](https://schema.org/PoliticalParty "PoliticalParty")
*   [Project](https://schema.org/Project "Project")
*   [ResearchOrganization](https://schema.org/ResearchOrganization "ResearchOrganization")
*   [SearchRescueOrganization](https://schema.org/SearchRescueOrganization "SearchRescueOrganization")
*   [SportsOrganization](https://schema.org/SportsOrganization "SportsOrganization")
*   [WorkersUnion](https://schema.org/WorkersUnion "WorkersUnion")

### Examples

#### Example 1
TEXT:

```
Google.Org
Contact Details:
Main address: 38 avenue de l'Opéra, F-75002 Paris, France
Tel: ( 33 1) 42 68 53 00, Fax: ( 33 1) 42 68 53 01
E-mail: secretariat (at) google.org
URL: <a href="http://www.google.org">www.google.org</a>
SIRET Code: 443 061 841 00039
VAT Number: FR64443061841
Members:
    - National Scientific Members in 100 countries and territories: Country1, Country2, ...
    - Scientific Union Members, 30 organizations listed in this Yearbook: Member 1, Member 2
```

JSON-LD:
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Organization",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Paris, France",
        "postalCode": "F-75002",
        "streetAddress": "38 avenue de l'Opéra"
      },
      "email": "secretariat(at)google.org",
      "faxNumber": "+33142685301",
      "iso6523Code": "0009:44306184100039",
      "iso6523Code": "9957:FR64443061841",
      "member": [
        {
          "@type": "Organization"
        },
        {
          "@type": "Organization"
        }
      ],
      "alumni": [
        {
          "@type": "Person",
          "name": "Jack Dan"
        },
        {
          "@type": "Person",
          "name": "John Smith"
        }
      ],
      "name": "Google.org (GOOG)",
      "telephone": "+33 1 42 68 53 00"
    }
    </script> 
```

#### Example 2
HTML:
```
<p>
<a href="http://npr.org">National Public Radio</a> has a sponsor:
<a href="http://www.example.com/GloboCorp">GloboCorp</a>.
</p>
```

JSON-LD:
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Organization",
      "name": "National Public Radio",
      "url": "http://npr.org",
      "sponsor":
      {
        "@type": "Organization",
        "name": "GloboCorp",
        "url": "http://www.example.com/"
      }
    }
    </script>
```

# Person

A Schema.org Type

  [Thing](/Thing "Thing") \>   [Person](/Person "Person")  

**\[more...\]**

*   Canonical URL: https://schema.org/Person
*   Equivalent Class: foaf:Person
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+Person)

A person (alive, dead, undead, or fictional).

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Person](/Person "Person") |     |     |
| `[additionalName](/additionalName "additionalName")` | [Text](/Text "Text") | An additional name for a Person, can be used for a middle name. |
| `[address](/address "address")` | [PostalAddress](/PostalAddress "PostalAddress")  or  <br>[Text](/Text "Text") | Physical address of the item. |
| `[affiliation](/affiliation "affiliation")` | [Organization](/Organization "Organization") | An organization that this person is affiliated with. For example, a school/university, a club, or a team. |
| `[agentInteractionStatistic](/agentInteractionStatistic "agentInteractionStatistic")` | [InteractionCounter](/InteractionCounter "InteractionCounter") | The number of completed interactions for this entity, in a particular role (the 'agent'), in a particular action (indicated in the statistic), and in a particular context (i.e. interactionService). |
| `[alumniOf](/alumniOf "alumniOf")` | [EducationalOrganization](/EducationalOrganization "EducationalOrganization")  or  <br>[Organization](/Organization "Organization") | An organization that the person is an alumni of.  <br>Inverse property: [alumni](/alumni "alumni") |
| `[award](/award "award")` | [Text](/Text "Text") | An award won by or for this item. Supersedes [awards](/awards "awards"). |
| `[birthDate](/birthDate "birthDate")` | [Date](/Date "Date") | Date of birth. |
| `[birthPlace](/birthPlace "birthPlace")` | [Place](/Place "Place") | The place where the person was born. |
| `[brand](/brand "brand")` | [Brand](/Brand "Brand")  or  <br>[Organization](/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| `[callSign](/callSign "callSign")` | [Text](/Text "Text") | A [callsign](https://en.wikipedia.org/wiki/Call_sign), as used in broadcasting and radio communications to identify people, radio and TV stations, or vehicles. |
| `[children](/children "children")` | [Person](/Person "Person") | A child of the person. |
| `[colleague](/colleague "colleague")` | [Person](/Person "Person")  or  <br>[URL](/URL "URL") | A colleague of the person. Supersedes [colleagues](/colleagues "colleagues"). |
| `[contactPoint](/contactPoint "contactPoint")` | [ContactPoint](/ContactPoint "ContactPoint") | A contact point for a person or organization. Supersedes [contactPoints](/contactPoints "contactPoints"). |
| `[deathDate](/deathDate "deathDate")` | [Date](/Date "Date") | Date of death. |
| `[deathPlace](/deathPlace "deathPlace")` | [Place](/Place "Place") | The place where the person died. |
| `[duns](/duns "duns")` | [Text](/Text "Text") | The Dun & Bradstreet DUNS number for identifying an organization or business person. |
| `[email](/email "email")` | [Text](/Text "Text") | Email address. |
| `[familyName](/familyName "familyName")` | [Text](/Text "Text") | Family name. In the U.S., the last name of a Person. |
| `[faxNumber](/faxNumber "faxNumber")` | [Text](/Text "Text") | The fax number. |
| `[follows](/follows "follows")` | [Person](/Person "Person") | The most generic uni-directional social relation. |
| `[funder](/funder "funder")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| `[funding](/funding "funding")` | [Grant](/Grant "Grant") | A [Grant](/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](/ownershipFundingInfo).  <br>Inverse property: [fundedItem](/fundedItem "fundedItem") |
| `[gender](/gender "gender")` | [GenderType](/GenderType "GenderType")  or  <br>[Text](/Text "Text") | Gender of something, typically a [Person](/Person), but possibly also fictional characters, animals, etc. While https://schema.org/Male and https://schema.org/Female may be used, text strings are also acceptable for people who are not a binary gender. The [gender](/gender) property can also be used in an extended sense to cover e.g. the gender of sports teams. As with the gender of individuals, we do not try to enumerate all possibilities. A mixed-gender [SportsTeam](/SportsTeam) can be indicated with a text value of "Mixed". |
| `[givenName](/givenName "givenName")` | [Text](/Text "Text") | Given name. In the U.S., the first name of a Person. |
| `[globalLocationNumber](/globalLocationNumber "globalLocationNumber")` | [Text](/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| `[hasCertification](/hasCertification "hasCertification")` | [Certification](/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| `[hasCredential](/hasCredential "hasCredential")` | [EducationalOccupationalCredential](/EducationalOccupationalCredential "EducationalOccupationalCredential") | A credential awarded to the Person or Organization. |
| `[hasOccupation](/hasOccupation "hasOccupation")` | [Occupation](/Occupation "Occupation") | The Person's occupation. For past professions, use Role for expressing dates. |
| `[hasOfferCatalog](/hasOfferCatalog "hasOfferCatalog")` | [OfferCatalog](/OfferCatalog "OfferCatalog") | Indicates an OfferCatalog listing for this Organization, Person, or Service. |
| `[hasPOS](/hasPOS "hasPOS")` | [Place](/Place "Place") | Points-of-Sales operated by the organization or person. |
| `[height](/height "height")` | [Distance](/Distance "Distance")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The height of the item. |
| `[homeLocation](/homeLocation "homeLocation")` | [ContactPoint](/ContactPoint "ContactPoint")  or  <br>[Place](/Place "Place") | A contact location for a person's residence. |
| `[honorificPrefix](/honorificPrefix "honorificPrefix")` | [Text](/Text "Text") | An honorific prefix preceding a Person's name such as Dr/Mrs/Mr. |
| `[honorificSuffix](/honorificSuffix "honorificSuffix")` | [Text](/Text "Text") | An honorific suffix following a Person's name such as M.D./PhD/MSCSW. |
| `[interactionStatistic](/interactionStatistic "interactionStatistic")` | [InteractionCounter](/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](/interactionCount "interactionCount"). |
| `[isicV4](/isicV4 "isicV4")` | [Text](/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| `[jobTitle](/jobTitle "jobTitle")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | The job title of the person (for example, Financial Manager). |
| `[knows](/knows "knows")` | [Person](/Person "Person") | The most generic bi-directional social/work relation. |
| `[knowsAbout](/knowsAbout "knowsAbout")` | [Text](/Text "Text")  or  <br>[Thing](/Thing "Thing")  or  <br>[URL](/URL "URL") | Of a [Person](/Person), and less typically of an [Organization](/Organization), to indicate a topic that is known about - suggesting possible expertise but not implying it. We do not distinguish skill levels here, or relate this to educational content, events, objectives or [JobPosting](/JobPosting) descriptions. |
| `[knowsLanguage](/knowsLanguage "knowsLanguage")` | [Language](/Language "Language")  or  <br>[Text](/Text "Text") | Of a [Person](/Person), and less typically of an [Organization](/Organization), to indicate a known language. We do not distinguish skill levels or reading/writing/speaking/signing here. Use language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). |
| `[makesOffer](/makesOffer "makesOffer")` | [Offer](/Offer "Offer") | A pointer to products or services offered by the organization or person.  <br>Inverse property: [offeredBy](/offeredBy "offeredBy") |
| `[memberOf](/memberOf "memberOf")` | [MemberProgramTier](/MemberProgramTier "MemberProgramTier")  or  <br>[Organization](/Organization "Organization")  or  <br>[ProgramMembership](/ProgramMembership "ProgramMembership") | An Organization (or ProgramMembership) to which this Person or Organization belongs.  <br>Inverse property: [member](/member "member") |
| `[naics](/naics "naics")` | [Text](/Text "Text") | The North American Industry Classification System (NAICS) code for a particular organization or business person. |
| `[nationality](/nationality "nationality")` | [Country](/Country "Country") | Nationality of the person. |
| `[netWorth](/netWorth "netWorth")` | [MonetaryAmount](/MonetaryAmount "MonetaryAmount")  or  <br>[PriceSpecification](/PriceSpecification "PriceSpecification") | The total financial value of the person as calculated by subtracting the total value of liabilities from the total value of assets. |
| `[owns](/owns "owns")` | [OwnershipInfo](/OwnershipInfo "OwnershipInfo")  or  <br>[Product](/Product "Product") | Products owned by the organization or person. |
| `[parent](/parent "parent")` | [Person](/Person "Person") | A parent of this person. Supersedes [parents](/parents "parents"). |
| `[performerIn](/performerIn "performerIn")` | [Event](/Event "Event") | Event that this person is a performer or participant in. |
| `[pronouns](/pronouns "pronouns")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[StructuredValue](/StructuredValue "StructuredValue")  or  <br>[Text](/Text "Text") | A short string listing or describing pronouns for a person. Typically the person concerned is the best authority as pronouns are a critical part of personal identity and expression. Publishers and consumers of this information are reminded to treat this data responsibly, take country-specific laws related to gender expression into account, and be wary of out-of-date data and drawing unwarranted inferences about the person being described.  <br>  <br>In English, formulations such as "they/them", "she/her", and "he/him" are commonly used online and can also be used here. We do not intend to enumerate all possible micro-syntaxes in all languages. More structured and well-defined external values for pronouns can be referenced using the [StructuredValue](/StructuredValue) or [DefinedTerm](/DefinedTerm) values. |
| `[publishingPrinciples](/publishingPrinciples "publishingPrinciples")` | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[URL](/URL "URL") | The publishingPrinciples property indicates (typically via [URL](/URL)) a document describing the editorial principles of an [Organization](/Organization) (or individual, e.g. a [Person](/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](/CreativeWork) (e.g. [NewsArticle](/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](/CreativeWork).  <br>  <br>While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](/funder)) can be expressed using schema.org terminology. |
| `[relatedTo](/relatedTo "relatedTo")` | [Person](/Person "Person") | The most generic familial relation. |
| `[seeks](/seeks "seeks")` | [Demand](/Demand "Demand") | A pointer to products or services sought by the organization or person (demand). |
| `[sibling](/sibling "sibling")` | [Person](/Person "Person") | A sibling of the person. Supersedes [siblings](/siblings "siblings"). |
| `[skills](/skills "skills")` | [DefinedTerm](/DefinedTerm "DefinedTerm")  or  <br>[Text](/Text "Text") | A statement of knowledge, skill, ability, task or any other assertion expressing a competency that is either claimed by a person, an organization or desired or required to fulfill a role or to work in an occupation. |
| `[sponsor](/sponsor "sponsor")` | [Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| `[spouse](/spouse "spouse")` | [Person](/Person "Person") | The person's spouse. |
| `[taxID](/taxID "taxID")` | [Text](/Text "Text") | The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain. |
| `[telephone](/telephone "telephone")` | [Text](/Text "Text") | The telephone number. |
| `[vatID](/vatID "vatID")` | [Text](/Text "Text") | The Value-added Tax ID of the organization or person. |
| `[weight](/weight "weight")` | [Mass](/Mass "Mass")  or  <br>[QuantitativeValue](/QuantitativeValue "QuantitativeValue") | The weight of the product or person. |
| `[workLocation](/workLocation "workLocation")` | [ContactPoint](/ContactPoint "ContactPoint")  or  <br>[Place](/Place "Place") | A contact location for a person's place of work. |
| `[worksFor](/worksFor "worksFor")` | [Organization](/Organization "Organization") | Organizations that the person works for. |
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

  

Instances of [Person](/Person "Person") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [accountablePerson](/accountablePerson "accountablePerson") | [CreativeWork](/CreativeWork "CreativeWork") | Specifies the Person that is legally accountable for the CreativeWork. |
| [acquiredFrom](/acquiredFrom "acquiredFrom") | [OwnershipInfo](/OwnershipInfo "OwnershipInfo") | The organization or person from which the product was acquired. |
| [actor](/actor "actor") | [Clip](/Clip "Clip")  or  <br>[CreativeWorkSeason](/CreativeWorkSeason "CreativeWorkSeason")  or  <br>[Episode](/Episode "Episode")  or  <br>[Event](/Event "Event")  or  <br>[Movie](/Movie "Movie")  or  <br>[MovieSeries](/MovieSeries "MovieSeries")  or  <br>[PodcastSeries](/PodcastSeries "PodcastSeries")  or  <br>[RadioSeries](/RadioSeries "RadioSeries")  or  <br>[TVSeries](/TVSeries "TVSeries")  or  <br>[VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries")  or  <br>[VideoObject](/VideoObject "VideoObject") | An actor (individual or a group), e.g. in TV, radio, movie, video games etc., or in an event. Actors can be associated with individual items or with a series, episode, clip. |
| [actors](/actors "actors") | [Clip](/Clip "Clip")  or  <br>[Episode](/Episode "Episode")  or  <br>[Movie](/Movie "Movie")  or  <br>[MovieSeries](/MovieSeries "MovieSeries")  or  <br>[RadioSeries](/RadioSeries "RadioSeries")  or  <br>[TVSeries](/TVSeries "TVSeries")  or  <br>[VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries")  or  <br>[VideoObject](/VideoObject "VideoObject") | An actor, e.g. in TV, radio, movie, video games etc. Actors can be associated with individual items or with a series, episode, clip. |
| [agent](/agent "agent") | [Action](/Action "Action") | The direct performer or driver of the action (animate or inanimate). E.g. _John_ wrote a book. |
| [alumni](/alumni "alumni") | [EducationalOrganization](/EducationalOrganization "EducationalOrganization")  or  <br>[Organization](/Organization "Organization") | Alumni of an organization. |
| [artist](/artist "artist") | [ComicIssue](/ComicIssue "ComicIssue")  or  <br>[ComicStory](/ComicStory "ComicStory")  or  <br>[VisualArtwork](/VisualArtwork "VisualArtwork") | The primary artist for a work in a medium other than pencils or digital line art--for example, if the primary artwork is done in watercolors or digital paints. |
| [athlete](/athlete "athlete") | [SportsTeam](/SportsTeam "SportsTeam") | A person that acts as performing member of a sports team; a player as opposed to a coach. |
| [attendee](/attendee "attendee") | [Event](/Event "Event") | A person or organization attending the event. |
| [attendees](/attendees "attendees") | [Event](/Event "Event") | A person attending the event. |
| [author](/author "author") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Rating](/Rating "Rating") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| [awayTeam](/awayTeam "awayTeam") | [SportsEvent](/SportsEvent "SportsEvent") | The away team in a sports event. |
| [bccRecipient](/bccRecipient "bccRecipient") | [Message](/Message "Message") | A sub property of recipient. The recipient blind copied on a message. |
| [bookingAgent](/bookingAgent "bookingAgent") | [Reservation](/Reservation "Reservation") | 'bookingAgent' is an out-dated term indicating a 'broker' that serves as a booking agent. |
| [borrower](/borrower "borrower") | [LendAction](/LendAction "LendAction") | A sub property of participant. The person that borrows the object being lent. |
| [broker](/broker "broker") | [Invoice](/Invoice "Invoice")  or  <br>[Order](/Order "Order")  or  <br>[Reservation](/Reservation "Reservation")  or  <br>[Service](/Service "Service") | An entity that arranges for an exchange between a buyer and a seller. In most cases a broker never acquires or releases ownership of a product or service involved in an exchange. If it is not clear whether an entity is a broker, seller, or buyer, the latter two terms are preferred. |
| [buyer](/buyer "buyer") | [SellAction](/SellAction "SellAction") | A sub property of participant. The participant/person/organization that bought the object. |
| [byArtist](/byArtist "byArtist") | [MusicAlbum](/MusicAlbum "MusicAlbum")  or  <br>[MusicRecording](/MusicRecording "MusicRecording") | The artist that performed this album or recording. |
| [candidate](/candidate "candidate") | [VoteAction](/VoteAction "VoteAction") | A sub property of object. The candidate subject of this action. |
| [ccRecipient](/ccRecipient "ccRecipient") | [Message](/Message "Message") | A sub property of recipient. The recipient copied on a message. |
| [character](/character "character") | [CreativeWork](/CreativeWork "CreativeWork") | Fictional person connected with a creative work. |
| [children](/children "children") | [Person](/Person "Person") | A child of the person. |
| [claimInterpreter](/claimInterpreter "claimInterpreter") | [Claim](/Claim "Claim") | For a [Claim](/Claim) interpreted from [MediaObject](/MediaObject) content, the [interpretedAsClaim](/interpretedAsClaim) property can be used to indicate a claim contained, implied or refined from the content of a [MediaObject](/MediaObject). |
| [coach](/coach "coach") | [SportsTeam](/SportsTeam "SportsTeam") | A person that acts in a coaching role for a sports team. |
| [colleague](/colleague "colleague") | [Person](/Person "Person") | A colleague of the person. |
| [colleagues](/colleagues "colleagues") | [Person](/Person "Person") | A colleague of the person. |
| [colorist](/colorist "colorist") | [ComicIssue](/ComicIssue "ComicIssue")  or  <br>[ComicStory](/ComicStory "ComicStory")  or  <br>[VisualArtwork](/VisualArtwork "VisualArtwork") | The individual who adds color to inked drawings. |
| [competitor](/competitor "competitor") | [SportsEvent](/SportsEvent "SportsEvent") | A competitor in a sports event. |
| [composer](/composer "composer") | [Event](/Event "Event")  or  <br>[MusicComposition](/MusicComposition "MusicComposition") | The person or organization who wrote a composition, or who is the composer of a work performed at some event. |
| [contributor](/contributor "contributor") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event") | A secondary contributor to the CreativeWork or Event. |
| [copyrightHolder](/copyrightHolder "copyrightHolder") | [CreativeWork](/CreativeWork "CreativeWork") | The party holding the legal copyright to the CreativeWork. |
| [creator](/creator "creator") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[UserComments](/UserComments "UserComments") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| [creditedTo](/creditedTo "creditedTo") | [MusicRelease](/MusicRelease "MusicRelease") | The group the release is credited to if different than the byArtist. For example, Red and Blue is credited to "Stefani Germanotta Band", but by Lady Gaga. |
| [customer](/customer "customer") | [Invoice](/Invoice "Invoice")  or  <br>[Order](/Order "Order") | Party placing the order or paying the invoice. |
| [director](/director "director") | [Clip](/Clip "Clip")  or  <br>[CreativeWorkSeason](/CreativeWorkSeason "CreativeWorkSeason")  or  <br>[Episode](/Episode "Episode")  or  <br>[Event](/Event "Event")  or  <br>[Movie](/Movie "Movie")  or  <br>[MovieSeries](/MovieSeries "MovieSeries")  or  <br>[RadioSeries](/RadioSeries "RadioSeries")  or  <br>[TVSeries](/TVSeries "TVSeries")  or  <br>[VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries")  or  <br>[VideoObject](/VideoObject "VideoObject") | A director of e.g. TV, radio, movie, video gaming etc. content, or of an event. Directors can be associated with individual items or with a series, episode, clip. |
| [directors](/directors "directors") | [Clip](/Clip "Clip")  or  <br>[Episode](/Episode "Episode")  or  <br>[Movie](/Movie "Movie")  or  <br>[MovieSeries](/MovieSeries "MovieSeries")  or  <br>[RadioSeries](/RadioSeries "RadioSeries")  or  <br>[TVSeries](/TVSeries "TVSeries")  or  <br>[VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries")  or  <br>[VideoObject](/VideoObject "VideoObject") | A director of e.g. TV, radio, movie, video games etc. content. Directors can be associated with individual items or with a series, episode, clip. |
| [editor](/editor "editor") | [CreativeWork](/CreativeWork "CreativeWork") | Specifies the Person who edited the CreativeWork. |
| [employee](/employee "employee") | [Organization](/Organization "Organization") | Someone working for this organization. |
| [employees](/employees "employees") | [Organization](/Organization "Organization") | People working for this organization. |
| [endorsee](/endorsee "endorsee") | [EndorseAction](/EndorseAction "EndorseAction") | A sub property of participant. The person/organization being supported. |
| [endorsers](/endorsers "endorsers") | [Diet](/Diet "Diet") | People or organizations that endorse the plan. |
| [followee](/followee "followee") | [FollowAction](/FollowAction "FollowAction") | A sub property of object. The person or organization being followed. |
| [follows](/follows "follows") | [Person](/Person "Person") | The most generic uni-directional social relation. |
| [founder](/founder "founder") | [Organization](/Organization "Organization") | A person or organization who founded this organization. |
| [founders](/founders "founders") | [Organization](/Organization "Organization") | A person who founded this organization. |
| [fundedItem](/fundedItem "fundedItem") | [Grant](/Grant "Grant") | Indicates something directly or indirectly funded or sponsored through a [Grant](/Grant). See also [ownershipFundingInfo](/ownershipFundingInfo). |
| [funder](/funder "funder") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event")  or  <br>[Grant](/Grant "Grant")  or  <br>[MonetaryGrant](/MonetaryGrant "MonetaryGrant")  or  <br>[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| [grantee](/grantee "grantee") | [DigitalDocumentPermission](/DigitalDocumentPermission "DigitalDocumentPermission") | The person, organization, contact point, or audience that has been granted this permission. |
| [hiringOrganization](/hiringOrganization "hiringOrganization") | [JobPosting](/JobPosting "JobPosting") | Organization or Person offering the job position. |
| [homeTeam](/homeTeam "homeTeam") | [SportsEvent](/SportsEvent "SportsEvent") | The home team in a sports event. |
| [illustrator](/illustrator "illustrator") | [Book](/Book "Book") | The illustrator of the book. |
| [inker](/inker "inker") | [ComicIssue](/ComicIssue "ComicIssue")  or  <br>[ComicStory](/ComicStory "ComicStory")  or  <br>[VisualArtwork](/VisualArtwork "VisualArtwork") | The individual who traces over the pencil drawings in ink after pencils are complete. |
| [instructor](/instructor "instructor") | [CourseInstance](/CourseInstance "CourseInstance") | A person assigned to instruct or provide instructional assistance for the [CourseInstance](/CourseInstance). |
| [knows](/knows "knows") | [Person](/Person "Person") | The most generic bi-directional social/work relation. |
| [landlord](/landlord "landlord") | [RentAction](/RentAction "RentAction") | A sub property of participant. The owner of the real estate property. |
| [legalRepresentative](/legalRepresentative "legalRepresentative") | [Organization](/Organization "Organization") | One or multiple persons who represent this organization legally such as CEO or sole administrator. |
| [legislationCountersignedBy](/legislationCountersignedBy "legislationCountersignedBy") | [Legislation](/Legislation "Legislation") | The person or organization that countersigned the legislation. Depending on the legal context, a countersignature can indicate that the signed authority undertakes to assume responsibility for texts emanating from a person who is inviolable and irresponsible, (for example a King, Grand Duc or President), or that the authority is in charge of the implementation of the text. |
| [legislationPassedBy](/legislationPassedBy "legislationPassedBy") | [Legislation](/Legislation "Legislation") | The person or organization that originally passed or made the law: typically parliament (for primary legislation) or government (for secondary legislation). This indicates the "legal author" of the law, as opposed to its physical author. |
| [legislationResponsible](/legislationResponsible "legislationResponsible") | [Legislation](/Legislation "Legislation") | An individual or organization that has some kind of responsibility for the legislation. Typically the ministry who is/was in charge of elaborating the legislation, or the adressee for potential questions about the legislation once it is published. |
| [lender](/lender "lender") | [BorrowAction](/BorrowAction "BorrowAction") | A sub property of participant. The person that lends the object being borrowed. |
| [letterer](/letterer "letterer") | [ComicIssue](/ComicIssue "ComicIssue")  or  <br>[ComicStory](/ComicStory "ComicStory")  or  <br>[VisualArtwork](/VisualArtwork "VisualArtwork") | The individual who adds lettering, including speech balloons and sound effects, to artwork. |
| [loser](/loser "loser") | [WinAction](/WinAction "WinAction") | A sub property of participant. The loser of the action. |
| [lyricist](/lyricist "lyricist") | [MusicComposition](/MusicComposition "MusicComposition") | The person who wrote the words. |
| [maintainer](/maintainer "maintainer") | [CreativeWork](/CreativeWork "CreativeWork") | A maintainer of a [Dataset](/Dataset), software package ([SoftwareApplication](/SoftwareApplication)), or other [Project](/Project). A maintainer is a [Person](/Person) or [Organization](/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| [member](/member "member") | [Organization](/Organization "Organization")  or  <br>[ProgramMembership](/ProgramMembership "ProgramMembership") | A member of an Organization or a ProgramMembership. Organizations can be members of organizations; ProgramMembership is typically for individuals. |
| [members](/members "members") | [Organization](/Organization "Organization")  or  <br>[ProgramMembership](/ProgramMembership "ProgramMembership") | A member of this organization. |
| [merchant](/merchant "merchant") | [Order](/Order "Order") | 'merchant' is an out-dated term for 'seller'. |
| [musicBy](/musicBy "musicBy") | [Clip](/Clip "Clip")  or  <br>[Episode](/Episode "Episode")  or  <br>[Movie](/Movie "Movie")  or  <br>[MovieSeries](/MovieSeries "MovieSeries")  or  <br>[RadioSeries](/RadioSeries "RadioSeries")  or  <br>[TVSeries](/TVSeries "TVSeries")  or  <br>[VideoGame](/VideoGame "VideoGame")  or  <br>[VideoGameSeries](/VideoGameSeries "VideoGameSeries")  or  <br>[VideoObject](/VideoObject "VideoObject") | The composer of the soundtrack. |
| [musicGroupMember](/musicGroupMember "musicGroupMember") | [MusicGroup](/MusicGroup "MusicGroup") | A member of a music group—for example, John, Paul, George, or Ringo. |
| [offeredBy](/offeredBy "offeredBy") | [Offer](/Offer "Offer") | A pointer to the organization or person making the offer. |
| [opponent](/opponent "opponent") | [ExerciseAction](/ExerciseAction "ExerciseAction") | A sub property of participant. The opponent on this action. |
| [organizer](/organizer "organizer") | [Event](/Event "Event") | An organizer of an Event. |
| [parent](/parent "parent") | [Person](/Person "Person") | A parent of this person. |
| [parents](/parents "parents") | [Person](/Person "Person") | A parents of the person. |
| [participant](/participant "participant") | [Action](/Action "Action") | Other co-agents that participated in the action indirectly. E.g. John wrote a book with _Steve_. |
| [penciler](/penciler "penciler") | [ComicIssue](/ComicIssue "ComicIssue")  or  <br>[ComicStory](/ComicStory "ComicStory")  or  <br>[VisualArtwork](/VisualArtwork "VisualArtwork") | The individual who draws the primary narrative artwork. |
| [performer](/performer "performer") | [Event](/Event "Event") | A performer at the event—for example, a presenter, musician, musical group or actor. |
| [performers](/performers "performers") | [Event](/Event "Event") | The main performer or performers of the event—for example, a presenter, musician, or actor. |
| [producer](/producer "producer") | [CreativeWork](/CreativeWork "CreativeWork") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| [provider](/provider "provider") | [Action](/Action "Action")  or  <br>[CreativeWork](/CreativeWork "CreativeWork")  or  <br>[EducationalOccupationalProgram](/EducationalOccupationalProgram "EducationalOccupationalProgram")  or  <br>[FinancialIncentive](/FinancialIncentive "FinancialIncentive")  or  <br>[Invoice](/Invoice "Invoice")  or  <br>[ParcelDelivery](/ParcelDelivery "ParcelDelivery")  or  <br>[Reservation](/Reservation "Reservation")  or  <br>[Service](/Service "Service")  or  <br>[Trip](/Trip "Trip") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. |
| [publishedBy](/publishedBy "publishedBy") | [PublicationEvent](/PublicationEvent "PublicationEvent") | An agent associated with the publication event. |
| [publisher](/publisher "publisher") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[FinancialIncentive](/FinancialIncentive "FinancialIncentive") | The publisher of the article in question. |
| [readBy](/readBy "readBy") | [Audiobook](/Audiobook "Audiobook") | A person who reads (performs) the audiobook. |
| [recipient](/recipient "recipient") | [AuthorizeAction](/AuthorizeAction "AuthorizeAction")  or  <br>[CommunicateAction](/CommunicateAction "CommunicateAction")  or  <br>[DonateAction](/DonateAction "DonateAction")  or  <br>[GiveAction](/GiveAction "GiveAction")  or  <br>[Message](/Message "Message")  or  <br>[PayAction](/PayAction "PayAction")  or  <br>[ReturnAction](/ReturnAction "ReturnAction")  or  <br>[SendAction](/SendAction "SendAction")  or  <br>[TipAction](/TipAction "TipAction") | A sub property of participant. The participant who is at the receiving end of the action. |
| [referee](/referee "referee") | [SportsEvent](/SportsEvent "SportsEvent") | An official who watches a game or match closely to enforce the rules and arbitrate on matters arising from the play such as referees, umpires or judges. The name of the effective function can vary according to the sport. |
| [relatedTo](/relatedTo "relatedTo") | [Person](/Person "Person") | The most generic familial relation. |
| [reviewedBy](/reviewedBy "reviewedBy") | [WebPage](/WebPage "WebPage") | People or organizations that have reviewed the content on this web page for accuracy and/or completeness. |
| [sdPublisher](/sdPublisher "sdPublisher") | [CreativeWork](/CreativeWork "CreativeWork") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](/sdPublisher) property helps make such practices more explicit. |
| [seller](/seller "seller") | [BuyAction](/BuyAction "BuyAction")  or  <br>[Demand](/Demand "Demand")  or  <br>[Flight](/Flight "Flight")  or  <br>[Offer](/Offer "Offer")  or  <br>[Order](/Order "Order") | An entity which offers (sells / leases / lends / loans) the services / goods. A seller may also be a provider. |
| [sender](/sender "sender") | [Message](/Message "Message")  or  <br>[ReceiveAction](/ReceiveAction "ReceiveAction") | A sub property of participant. The participant who is at the sending end of the action. |
| [sibling](/sibling "sibling") | [Person](/Person "Person") | A sibling of the person. |
| [siblings](/siblings "siblings") | [Person](/Person "Person") | A sibling of the person. |
| [spokenByCharacter](/spokenByCharacter "spokenByCharacter") | [Quotation](/Quotation "Quotation") | The (e.g. fictional) character, Person or Organization to whom the quotation is attributed within the containing CreativeWork. |
| [sponsor](/sponsor "sponsor") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event")  or  <br>[Grant](/Grant "Grant")  or  <br>[MedicalStudy](/MedicalStudy "MedicalStudy")  or  <br>[Organization](/Organization "Organization")  or  <br>[Person](/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| [spouse](/spouse "spouse") | [Person](/Person "Person") | The person's spouse. |
| [toRecipient](/toRecipient "toRecipient") | [Message](/Message "Message") | A sub property of recipient. The recipient who was directly sent the message. |
| [translator](/translator "translator") | [CreativeWork](/CreativeWork "CreativeWork")  or  <br>[Event](/Event "Event") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| [underName](/underName "underName") | [Reservation](/Reservation "Reservation")  or  <br>[Ticket](/Ticket "Ticket") | The person or organization the reservation or ticket is for. |
| [vendor](/vendor "vendor") | [BuyAction](/BuyAction "BuyAction") | 'vendor' is an earlier term for 'seller'. |
| [winner](/winner "winner") | [LoseAction](/LoseAction "LoseAction") | A sub property of participant. The winner of the action. |

  

#### More specific Types

*   [Patient](/Patient "Patient")

### Acknowledgements

IPTC rNews properties

This class contains derivatives of IPTC rNews properties. rNews is a data model of publishing metadata with serializations currently available for RDFa as well as HTML5 Microdata. More information about the IPTC and rNews can be found at [rnews.org](http://rnews.org).

### Examples
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Person",
      "address": {
        "@type": "PostalAddress",
        "addressLocality": "Seattle",
        "addressRegion": "WA",
        "postalCode": "98052",
        "streetAddress": "20341 Whitworth Institute 405 N. Whitworth"
      },
      "colleague": [
        "http://www.xyz.edu/students/alicejones.html",
        "http://www.xyz.edu/students/bobsmith.html"
      ],
      "email": "mailto:jane-doe@xyz.edu",
      "image": "janedoe.jpg",
      "jobTitle": "Professor",
      "name": "Jane Doe",
      "telephone": "(425) 123-4567",
      "url": "http://www.janedoe.com"
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "MusicEvent",
      "location": {
        "@type": "MusicVenue",
        "name": "Chicago Symphony Center",
        "address": "220 S. Michigan Ave, Chicago, Illinois, USA"
      },
      "name": "Shostakovich Leningrad",
      "offers": {
        "@type": "Offer",
        "url": "/examples/ticket/12341234",
        "price": "40",
        "priceCurrency": "USD",
        "availability": "https://schema.org/InStock"
      },
      "performer": [
        {
          "@type": "MusicGroup",
          "name": "Chicago Symphony Orchestra",
          "sameAs": [
            "http://cso.org/",
            "http://en.wikipedia.org/wiki/Chicago_Symphony_Orchestra"
          ]
        },
        {
          "@type": "Person",
          "image": "/examples/jvanzweden_s.jpg",
          "name": "Jaap van Zweden",
          "sameAs": "http://www.jaapvanzweden.com/"
        }
      ],
      "startDate": "2014-05-23T20:00",
      "workPerformed": [
        {
          "@type": "CreativeWork",
          "name": "Britten Four Sea Interludes and Passacaglia from Peter Grimes",
          "sameAs": "http://en.wikipedia.org/wiki/Peter_Grimes"
        },
        {
          "@type": "CreativeWork",
          "name": "Shostakovich Symphony No. 7 (Leningrad)",
          "sameAs": "http://en.wikipedia.org/wiki/Symphony_No._7_(Shostakovich)"
        }
      ]
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "SportsTeam",
      "name": "San Francisco 49ers",
      "member": {
        "@type": "OrganizationRole",
        "member": {
          "@type": "Person",
          "name": "Joe Montana"
        },
        "startDate": "1979",
        "endDate": "1992",
        "roleName": "Quarterback"
      }
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Person",
      "name": "Peter Venkman",
      "hasOccupation": {
        "@type": "Occupation",
        "name": "Parapsychologist",
        "educationRequirements": "PhD in parapsychology"
      }
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Person",
      "name": "Albert Einstein",
      "hasOccupation": [
        {
          "@type": "Role",
          "hasOccupation": {
          "@type": "Occupation",
          "name": "Patent examiner",
            "occupationalCategory": "23-2099.00"
          },
          "startDate": "1901",
          "endDate": "1906"
        },
        {
          "@type": "Occupation",
          "name": "Professor of Physics",
          "educationRequirements": "PhD in Physics"
        }
      ]
    }
    </script>
```
```
    <!-- jobTitle utilising DefinedTerm -->
    <script type="application/ld+json">
    {
        "@context": "https://schema.org/",
        "@type": "Person",
        "name": "A. N. Other",
        "jobTitle": {
            "@type": "DefinedTerm",
            "inDefinedTermSet": "https://targetjobs.co.uk/careers-advice/job-descriptions",
            "termCode": "277133-aid-workerhumanitarian-worker-job-description",
            "name": "Aid worker/humanitarian worker",
            "url": "https://targetjobs.co.uk/careers-advice/job-descriptions/277133-aid-workerhumanitarian-worker-job-description"
        }
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Person",
      "name": "Christopher Froome",
      "sponsor":
      {
        "@type": "Organization",
        "name": "Sky",
        "url": "http://www.skysports.com/"
      }
    }
    </script>
```Title: Product - Schema.org Type

URL Source: https://schema.org/Product

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

Any offered product or service. For example: a pair of shoes; a concert ticket; the rental of a car; a haircut; or an episode of a TV show streamed online.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Product](https://schema.org/Product "Product") |
| ``` additionalProperty ``` | [PropertyValue](https://schema.org/PropertyValue "PropertyValue") | A property-value pair representing an additional characteristic of the entity, e.g. a product feature or another characteristic for which there is no matching property in schema.org. Note: Publishers should be aware that applications designed to use specific schema.org properties (e.g. https://schema.org/width, https://schema.org/color, https://schema.org/gtin13, ...) will typically expect such data to be provided using those properties, rather than using the generic property/value mechanism. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` asin ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | An Amazon Standard Identification Number (ASIN) is a 10-character alphanumeric unique identifier assigned by Amazon.com and its partners for product identification within the Amazon organization (summary from [Wikipedia](https://en.wikipedia.org/wiki/Amazon_Standard_Identification_Number)'s article). Note also that this is a definition for how to include ASINs in Schema.org data, and not a definition of ASINs in general - see documentation from Amazon for authoritative details. ASINs are most commonly encoded as text strings, but the [asin] property supports URL/URI as potential values too. |
| ``` audience ``` | [Audience](https://schema.org/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](https://schema.org/serviceAudience "serviceAudience"). |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` brand ``` | [Brand](https://schema.org/Brand "Brand") or [Organization](https://schema.org/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| ``` category ``` | [CategoryCode](https://schema.org/CategoryCode "CategoryCode") or [PhysicalActivityCategory](https://schema.org/PhysicalActivityCategory "PhysicalActivityCategory") or [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | A category for the item. Greater signs or slashes can be used to informally indicate a category hierarchy. |
| ``` color ``` | [Text](https://schema.org/Text "Text") | The color of the product. |
| ``` colorSwatch ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | A color swatch image, visualizing the color of a [Product](https://schema.org/Product). Should match the textual description specified in the [color](https://schema.org/color) property. This can be a URL or a fully described ImageObject. |
| ``` countryOfAssembly ``` | [Text](https://schema.org/Text "Text") | The place where the product was assembled. |
| ``` countryOfLastProcessing ``` | [Text](https://schema.org/Text "Text") | The place where the item (typically [Product](https://schema.org/Product)) was last processed and tested before importation. |
| ``` countryOfOrigin ``` | [Country](https://schema.org/Country "Country") | The country of origin of something, including products as well as creative works such as movie and TV content. In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](https://schema.org/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](https://schema.org/contentLocation) and [locationCreated](https://schema.org/locationCreated) may be more applicable. In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here. |
| ``` depth ``` | [Distance](https://schema.org/Distance "Distance") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The depth of the item. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` gtin ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | A Global Trade Item Number ([GTIN](https://www.gs1.org/standards/id-keys/gtin)). GTINs identify trade items, including products and services, using numeric identification codes. A correct [gtin](https://schema.org/gtin) value should be a valid GTIN, which means that it should be an all-numeric string of either 8, 12, 13 or 14 digits, or a "GS1 Digital Link" URL based on such a string. The numeric component should also have a [valid GS1 check digit](https://www.gs1.org/services/check-digit-calculator) and meet the other rules for valid GTINs. See also [GS1's GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) and [Wikipedia](https://en.wikipedia.org/wiki/Global_Trade_Item_Number) for more details. Left-padding of the gtin values is not required or encouraged. The [gtin](https://schema.org/gtin) property generalizes the earlier [gtin8](https://schema.org/gtin8), [gtin12](https://schema.org/gtin12), [gtin13](https://schema.org/gtin13), and [gtin14](https://schema.org/gtin14) properties. The GS1 [digital link specifications](https://www.gs1.org/standards/Digital-Link/) expresses GTINs as URLs (URIs, IRIs, etc.). Digital Links should be populated into the [hasGS1DigitalLink](https://schema.org/hasGS1DigitalLink) attribute. Note also that this is a definition for how to include GTINs in Schema.org data, and not a definition of GTINs in general - see the GS1 documentation for authoritative details. |
| ``` gtin12 ``` | [Text](https://schema.org/Text "Text") | The GTIN-12 code of the product, or the product to which the offer refers. The GTIN-12 is the 12-digit GS1 Identification Key composed of a U.P.C. Company Prefix, Item Reference, and Check Digit used to identify trade items. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin13 ``` | [Text](https://schema.org/Text "Text") | The GTIN-13 code of the product, or the product to which the offer refers. This is equivalent to 13-digit ISBN codes and EAN UCC-13. Former 12-digit UPC codes can be converted into a GTIN-13 code by simply adding a preceding zero. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin14 ``` | [Text](https://schema.org/Text "Text") | The GTIN-14 code of the product, or the product to which the offer refers. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` gtin8 ``` | [Text](https://schema.org/Text "Text") | The GTIN-8 code of the product, or the product to which the offer refers. This code is also known as EAN/UCC-8 or 8-digit EAN. See [GS1 GTIN Summary](http://www.gs1.org/barcodes/technical/idkeys/gtin) for more details. |
| ``` hasAdultConsideration ``` | [AdultOrientedEnumeration](https://schema.org/AdultOrientedEnumeration "AdultOrientedEnumeration") | Used to tag an item to be intended or suitable for consumption or use by adults only. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasEnergyConsumptionDetails ``` | [EnergyConsumptionDetails](https://schema.org/EnergyConsumptionDetails "EnergyConsumptionDetails") | Defines the energy efficiency Category (also known as "class" or "rating") for a product according to an international energy efficiency standard. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMeasurement ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | A measurement of an item, For example, the inseam of pants, the wheel size of a bicycle, the gauge of a screw, or the carbon footprint measured for certification by an authority. Usually an exact measurement, but can also be a range of measurements for adjustable products, for example belts and ski bindings. |
| ``` hasMerchantReturnPolicy ``` | [MerchantReturnPolicy](https://schema.org/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](https://schema.org/hasProductReturnPolicy "hasProductReturnPolicy"). |
| ``` height ``` | [Distance](https://schema.org/Distance "Distance") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The height of the item. |
| ``` inProductGroupWithID ``` | [Text](https://schema.org/Text "Text") | Indicates the [productGroupID](https://schema.org/productGroupID) for a [ProductGroup](https://schema.org/ProductGroup) that this product [isVariantOf](https://schema.org/isVariantOf). |
| ``` isAccessoryOrSparePartFor ``` | [Product](https://schema.org/Product "Product") | A pointer to another product (or multiple products) for which this product is an accessory or spare part. |
| ``` isConsumableFor ``` | [Product](https://schema.org/Product "Product") | A pointer to another product (or multiple products) for which this product is a consumable. |
| ``` isFamilyFriendly ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether this content is family friendly. |
| ``` isRelatedTo ``` | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, somehow related product (or multiple products). |
| ``` isSimilarTo ``` | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, functionally similar product (or multiple products). |
| ``` isVariantOf ``` | [ProductGroup](https://schema.org/ProductGroup "ProductGroup") or [ProductModel](https://schema.org/ProductModel "ProductModel") | Indicates the kind of product that this is a variant of. In the case of [ProductModel](https://schema.org/ProductModel), this is a pointer (from a ProductModel) to a base product from which this product is a variant. It is safe to infer that the variant inherits all product features from the base model, unless defined locally. This is not transitive. In the case of a [ProductGroup](https://schema.org/ProductGroup), the group description also serves as a template, representing a set of Products that vary on explicitly defined, specific dimensions only (so it defines both a set of variants, as well as which values distinguish amongst those variants). When used with [ProductGroup](https://schema.org/ProductGroup), this property can apply to any [Product](https://schema.org/Product) included in the group. Inverse property: [hasVariant](https://schema.org/hasVariant "hasVariant") |
| ``` itemCondition ``` | [OfferItemCondition](https://schema.org/OfferItemCondition "OfferItemCondition") | A predefined value from OfferItemCondition specifying the condition of the product or service, or the products or services included in the offer. Also used for product return policies to specify the condition of products accepted for returns. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` manufacturer ``` | [Organization](https://schema.org/Organization "Organization") | The manufacturer of the product. |
| ``` material ``` | [Product](https://schema.org/Product "Product") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| ``` mobileUrl ``` | [Text](https://schema.org/Text "Text") | The [mobileUrl](https://schema.org/mobileUrl) property is provided for specific situations in which data consumers need to determine whether one of several provided URLs is a dedicated 'mobile site'. To discourage over-use, and reflecting intial usecases, the property is expected only on [Product](https://schema.org/Product) and [Offer](https://schema.org/Offer), rather than [Thing](https://schema.org/Thing). The general trend in web technology is towards [responsive design](https://en.wikipedia.org/wiki/Responsive_web_design) in which content can be flexibly adapted to a wide range of browsing environments. Pages and sites referenced with the long-established [url](https://schema.org/url) property should ideally also be usable on a wide variety of devices, including mobile phones. In most cases, it would be pointless and counter productive to attempt to update all [url](https://schema.org/url) markup to use [mobileUrl](https://schema.org/mobileUrl) for more mobile-oriented pages. The property is intended for the case when items (primarily [Product](https://schema.org/Product) and [Offer](https://schema.org/Offer)) have extra URLs hosted on an additional "mobile site" alongside the main one. It should not be taken as an endorsement of this publication style. |
| ``` model ``` | [ProductModel](https://schema.org/ProductModel "ProductModel") or [Text](https://schema.org/Text "Text") | The model of the product. Use with the URL of a ProductModel or a textual representation of the model identifier. The URL of the ProductModel can be from an external source. It is recommended to additionally provide strong product identifiers via the gtin8/gtin13/gtin14 and mpn properties. |
| ``` mpn ``` | [Text](https://schema.org/Text "Text") | The Manufacturer Part Number (MPN) of the product, or the product to which the offer refers. |
| ``` negativeNotes ``` | [ItemList](https://schema.org/ItemList "ItemList") or [ListItem](https://schema.org/ListItem "ListItem") or [Text](https://schema.org/Text "Text") or [WebContent](https://schema.org/WebContent "WebContent") | Provides negative considerations regarding something, most typically in pro/con lists for reviews (alongside [positiveNotes](https://schema.org/positiveNotes)). For symmetry In the case of a [Review](https://schema.org/Review), the property describes the [itemReviewed](https://schema.org/itemReviewed) from the perspective of the review; in the case of a [Product](https://schema.org/Product), the product itself is being described. Since product descriptions tend to emphasise positive claims, it may be relatively unusual to find [negativeNotes](https://schema.org/negativeNotes) used in this way. Nevertheless for the sake of symmetry, [negativeNotes](https://schema.org/negativeNotes) can be used on [Product](https://schema.org/Product). The property values can be expressed either as unstructured text (repeated as necessary), or if ordered, as a list (in which case the most negative is at the beginning of the list). |
| ``` nsn ``` | [Text](https://schema.org/Text "Text") | Indicates the [NATO stock number](https://en.wikipedia.org/wiki/NATO_Stock_Number) (nsn) of a [Product](https://schema.org/Product). |
| ``` offers ``` | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](https://schema.org/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](https://schema.org/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [itemOffered](https://schema.org/itemOffered "itemOffered") |
| ``` pattern ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported. |
| ``` positiveNotes ``` | [ItemList](https://schema.org/ItemList "ItemList") or [ListItem](https://schema.org/ListItem "ListItem") or [Text](https://schema.org/Text "Text") or [WebContent](https://schema.org/WebContent "WebContent") | Provides positive considerations regarding something, for example product highlights or (alongside [negativeNotes](https://schema.org/negativeNotes)) pro/con lists for reviews. In the case of a [Review](https://schema.org/Review), the property describes the [itemReviewed](https://schema.org/itemReviewed) from the perspective of the review; in the case of a [Product](https://schema.org/Product), the product itself is being described. The property values can be expressed either as unstructured text (repeated as necessary), or if ordered, as a list (in which case the most positive is at the beginning of the list). |
| ``` productID ``` | [Text](https://schema.org/Text "Text") | The product identifier, such as ISBN. For example: `meta itemprop="productID" content="isbn:123-456-789"`. |
| ``` productionDate ``` | [Date](https://schema.org/Date "Date") | The date of production of the item, e.g. vehicle. |
| ``` purchaseDate ``` | [Date](https://schema.org/Date "Date") | The date the item, e.g. vehicle, was purchased by the current owner. |
| ``` releaseDate ``` | [Date](https://schema.org/Date "Date") | The release date of a product or product model. This can be used to distinguish the exact variant of a product. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` size ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") or [SizeSpecification](https://schema.org/SizeSpecification "SizeSpecification") or [Text](https://schema.org/Text "Text") | A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](https://schema.org/SizeSpecification); in other cases, the [width](https://schema.org/width), [height](https://schema.org/height), [depth](https://schema.org/depth) and [weight](https://schema.org/weight) properties may be more applicable. |
| ``` sku ``` | [Text](https://schema.org/Text "Text") | The Stock Keeping Unit (SKU), i.e. a merchant-specific identifier for a product or service, or the product to which the offer refers. |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` weight ``` | [Mass](https://schema.org/Mass "Mass") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The weight of the product or person. |
| ``` width ``` | [Distance](https://schema.org/Distance "Distance") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The width of the item. |
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

Instances of [Product](https://schema.org/Product "Product") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [fundedItem](https://schema.org/fundedItem "fundedItem") | [Grant](https://schema.org/Grant "Grant") | Indicates something directly or indirectly funded or sponsored through a [Grant](https://schema.org/Grant). See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). |
| [hasVariant](https://schema.org/hasVariant "hasVariant") | [ProductGroup](https://schema.org/ProductGroup "ProductGroup") | Indicates a [Product](https://schema.org/Product) that is a member of this [ProductGroup](https://schema.org/ProductGroup) (or [ProductModel](https://schema.org/ProductModel)). |
| [incentivizedItem](https://schema.org/incentivizedItem "incentivizedItem") | [FinancialIncentive](https://schema.org/FinancialIncentive "FinancialIncentive") | The type or specific product(s) and/or service(s) being incentivized. DefinedTermSets are used for product and service categories such as the United Nations Standard Products and Services Code: ``` { "@type": "DefinedTerm", "inDefinedTermSet": "https://www.unspsc.org/", "termCode": "261315XX", "name": "Photovoltaic module" } ``` For a specific product or service, use the Product type: ``` { "@type": "Product", "name": "Kenmore White 17" Microwave", } ``` For multiple different incentivized items, use multiple [DefinedTerm](https://schema.org/DefinedTerm) or [Product](https://schema.org/Product). |
| [isAccessoryOrSparePartFor](https://schema.org/isAccessoryOrSparePartFor "isAccessoryOrSparePartFor") | [Product](https://schema.org/Product "Product") | A pointer to another product (or multiple products) for which this product is an accessory or spare part. |
| [isBasedOn](https://schema.org/isBasedOn "isBasedOn") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A resource from which this work is derived or from which it is a modification or adaptation. |
| [isBasedOnUrl](https://schema.org/isBasedOnUrl "isBasedOnUrl") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A resource that was used in the creation of this resource. This term can be repeated for multiple sources. For example, http://example.com/great-multiplication-intro.html. |
| [isConsumableFor](https://schema.org/isConsumableFor "isConsumableFor") | [Product](https://schema.org/Product "Product") | A pointer to another product (or multiple products) for which this product is a consumable. |
| [isRelatedTo](https://schema.org/isRelatedTo "isRelatedTo") | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, somehow related product (or multiple products). |
| [isSimilarTo](https://schema.org/isSimilarTo "isSimilarTo") | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, functionally similar product (or multiple products). |
| [itemOffered](https://schema.org/itemOffered "itemOffered") | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](https://schema.org/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |
| [itemShipped](https://schema.org/itemShipped "itemShipped") | [ParcelDelivery](https://schema.org/ParcelDelivery "ParcelDelivery") | Item(s) being shipped. |
| [material](https://schema.org/material "material") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Product](https://schema.org/Product "Product") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| [orderedItem](https://schema.org/orderedItem "orderedItem") | [Order](https://schema.org/Order "Order") or [OrderItem](https://schema.org/OrderItem "OrderItem") | The item ordered. |
| [owns](https://schema.org/owns "owns") | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | Products owned by the organization or person. |
| [productSupported](https://schema.org/productSupported "productSupported") | [ContactPoint](https://schema.org/ContactPoint "ContactPoint") | The product or service this support contact point is related to (such as product support for a particular product line). This can be a specific product or product line (e.g. "iPhone") or a general category of products or services (e.g. "smartphones"). |
| [typeOfGood](https://schema.org/typeOfGood "typeOfGood") | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") or [TypeAndQuantityNode](https://schema.org/TypeAndQuantityNode "TypeAndQuantityNode") | The product that this structured value is referring to. |

#### More specific Types

*   [DietarySupplement](https://schema.org/DietarySupplement "DietarySupplement")
*   [Drug](https://schema.org/Drug "Drug")
*   [IndividualProduct](https://schema.org/IndividualProduct "IndividualProduct")
*   [ProductCollection](https://schema.org/ProductCollection "ProductCollection")
*   [ProductGroup](https://schema.org/ProductGroup "ProductGroup")
*   [ProductModel](https://schema.org/ProductModel "ProductModel")
*   [SomeProducts](https://schema.org/SomeProducts "SomeProducts")
*   [Vehicle](https://schema.org/Vehicle "Vehicle")

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
      "@context": "https://schema.org/",
      "@type": "Product",
      "name": "Crew neck white t-shirt",
      "description": "White t-shirt  made of soft and lightweight cotton jersey, ensuring comfort, a refined mélange texture adds sporty appeal.",
      "hasGS1DigitalLink": "https://gs1.appareldemo.com/01/09506000164908",
      "gtin": "09506000164908"
    }
    </script>
```
Title: ProfessionalService - Schema.org Type

URL Source: https://schema.org/ProfessionalService

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

Original definition: "provider of professional services."

The general [ProfessionalService](https://schema.org/ProfessionalService) type for local businesses was deprecated due to confusion with [Service](https://schema.org/Service). For reference, the types that it included were: [Dentist](https://schema.org/Dentist), [AccountingService](https://schema.org/AccountingService), [Attorney](https://schema.org/Attorney), [Notary](https://schema.org/Notary), as well as types for several kinds of [HomeAndConstructionBusiness](https://schema.org/HomeAndConstructionBusiness): [Electrician](https://schema.org/Electrician), [GeneralContractor](https://schema.org/GeneralContractor), [HousePainter](https://schema.org/HousePainter), [Locksmith](https://schema.org/Locksmith), [Plumber](https://schema.org/Plumber), [RoofingContractor](https://schema.org/RoofingContractor). [LegalService](https://schema.org/LegalService) was introduced as a more inclusive supertype of [Attorney](https://schema.org/Attorney).

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [LocalBusiness](https://schema.org/LocalBusiness "LocalBusiness") |
| ``` currenciesAccepted ``` | [Text](https://schema.org/Text "Text") | The currency accepted. Use standard formats: [ISO 4217 currency format](http://en.wikipedia.org/wiki/ISO_4217), e.g. "USD"; [Ticker symbol](https://en.wikipedia.org/wiki/List_of_cryptocurrencies) for cryptocurrencies, e.g. "BTC"; well known names for [Local Exchange Trading Systems](https://en.wikipedia.org/wiki/Local_exchange_trading_system) (LETS) and other currency types, e.g. "Ithaca HOUR". |
| ``` openingHours ``` | [Text](https://schema.org/Text "Text") | The general opening hours for a business. Opening hours can be specified as a weekly time range, starting with days, then times per day. Multiple days can be listed with commas ',' separating each day. Day or time ranges are specified using a hyphen '-'. * Days are specified using the following two-letter combinations: `Mo`, `Tu`, `We`, `Th`, `Fr`, `Sa`, `Su`. * Times are specified using 24:00 format. For example, 3pm is specified as `15:00`, 10am as `10:00`. * Here is an example: `<time itemprop="openingHours" datetime="Tu,Th 16:00-20:00">Tuesdays and Thursdays 4-8pm</time>`. * If a business is open 7 days a week, then it can be specified as `<time itemprop="openingHours" datetime="Mo-Su">Monday through Sunday, all day</time>`. |
| ``` paymentAccepted ``` | [Text](https://schema.org/Text "Text") | Cash, Credit Card, Cryptocurrency, Local Exchange Tradings System, etc. |
| ``` priceRange ``` | [Text](https://schema.org/Text "Text") | The price range of the business, for example `$$$`. |
| Properties from [Organization](https://schema.org/Organization "Organization") |
| ``` acceptedPaymentMethod ``` | [LoanOrCredit](https://schema.org/LoanOrCredit "LoanOrCredit") or [PaymentMethod](https://schema.org/PaymentMethod "PaymentMethod") or [Text](https://schema.org/Text "Text") | The payment method(s) that are accepted in general by an organization, or for some specific demand or offer. |
| ``` actionableFeedbackPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) or other news-related [Organization](https://schema.org/Organization), a statement about public engagement activities (for news media, the newsroom’s), including involving the public - digitally or otherwise -- in coverage decisions, reporting and activities after publication. |
| ``` address ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") | Physical address of the item. |
| ``` agentInteractionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of completed interactions for this entity, in a particular role (the 'agent'), in a particular action (indicated in the statistic), and in a particular context (i.e. interactionService). |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` alumni ``` | [Person](https://schema.org/Person "Person") | Alumni of an organization. Inverse property: [alumniOf](https://schema.org/alumniOf "alumniOf") |
| ``` areaServed ``` | [AdministrativeArea](https://schema.org/AdministrativeArea "AdministrativeArea") or [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](https://schema.org/serviceArea "serviceArea"). |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` brand ``` | [Brand](https://schema.org/Brand "Brand") or [Organization](https://schema.org/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| ``` companyRegistration ``` | [Certification](https://schema.org/Certification "Certification") | The official registration number of a business including the organization that issued it such as Company House or Chamber of Commerce. |
| ``` contactPoint ``` | [ContactPoint](https://schema.org/ContactPoint "ContactPoint") | A contact point for a person or organization. Supersedes [contactPoints](https://schema.org/contactPoints "contactPoints"). |
| ``` correctionsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (e.g. [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement describing (in news media, the newsroom’s) disclosure and correction policy for errors. |
| ``` department ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between an organization and a department of that organization, also described as an organization (allowing different urls, logos, opening hours). For example: a store with a pharmacy, or a bakery with a cafe. |
| ``` dissolutionDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was dissolved. |
| ``` diversityPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement on diversity policy by an [Organization](https://schema.org/Organization) e.g. a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization). For a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), a statement describing the newsroom’s diversity policy on both staffing and sources, typically providing staffing data. |
| ``` diversityStaffingReport ``` | [Article](https://schema.org/Article "Article") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a report on staffing diversity issues. In a news context this might be for example ASNE or RTDNA (US) reports, or self-reported. |
| ``` duns ``` | [Text](https://schema.org/Text "Text") | The Dun & Bradstreet DUNS number for identifying an organization or business person. |
| ``` email ``` | [Text](https://schema.org/Text "Text") | Email address. |
| ``` employee ``` | [Person](https://schema.org/Person "Person") | Someone working for this organization. Supersedes [employees](https://schema.org/employees "employees"). |
| ``` ethicsPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Statement about ethics policy, e.g. of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization) regarding journalistic and publishing practices, or of a [Restaurant](https://schema.org/Restaurant), a page describing food source policies. In the case of a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization), an ethicsPolicy is typically a statement describing the personal, organizational, and corporate standards of behavior expected by the organization. |
| ``` event ``` | [Event](https://schema.org/Event "Event") | Upcoming or past event associated with this place, organization, or action. Supersedes [events](https://schema.org/events "events"). |
| ``` faxNumber ``` | [Text](https://schema.org/Text "Text") | The fax number. |
| ``` founder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization who founded this organization. Supersedes [founders](https://schema.org/founders "founders"). |
| ``` foundingDate ``` | [Date](https://schema.org/Date "Date") | The date that this organization was founded. |
| ``` foundingLocation ``` | [Place](https://schema.org/Place "Place") | The place where the Organization was founded. |
| ``` funder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` globalLocationNumber ``` | [Text](https://schema.org/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasCredential ``` | [EducationalOccupationalCredential](https://schema.org/EducationalOccupationalCredential "EducationalOccupationalCredential") | A credential awarded to the Person or Organization. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMemberProgram ``` | [MemberProgram](https://schema.org/MemberProgram "MemberProgram") | MemberProgram offered by an Organization, for example an eCommerce merchant or an airline. |
| ``` hasMerchantReturnPolicy ``` | [MerchantReturnPolicy](https://schema.org/MerchantReturnPolicy "MerchantReturnPolicy") | Specifies a MerchantReturnPolicy that may be applicable. Supersedes [hasProductReturnPolicy](https://schema.org/hasProductReturnPolicy "hasProductReturnPolicy"). |
| ``` hasOfferCatalog ``` | [OfferCatalog](https://schema.org/OfferCatalog "OfferCatalog") | Indicates an OfferCatalog listing for this Organization, Person, or Service. |
| ``` hasPOS ``` | [Place](https://schema.org/Place "Place") | Points-of-Sales operated by the organization or person. |
| ``` hasShippingService ``` | [ShippingService](https://schema.org/ShippingService "ShippingService") | Specification of a shipping service offered by the organization. |
| ``` interactionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](https://schema.org/interactionCount "interactionCount"). |
| ``` isicV4 ``` | [Text](https://schema.org/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| ``` iso6523Code ``` | [Text](https://schema.org/Text "Text") | An organization identifier as defined in [ISO 6523(-1)](https://en.wikipedia.org/wiki/ISO/IEC_6523). The identifier should be in the `XXXX:YYYYYY:ZZZ` or `XXXX:YYYYYY`format. Where `XXXX` is a 4 digit _ICD_ (International Code Designator), `YYYYYY` is an _OID_ (Organization Identifier) with all formatting characters (dots, dashes, spaces) removed with a maximal length of 35 characters, and `ZZZ` is an optional OPI (Organization Part Identifier) with a maximum length of 35 characters. The various components (ICD, OID, OPI) are joined with a colon character (ASCII `0x3a`). Note that many existing organization identifiers defined as attributes like [leiCode](https://schema.org/leiCode) (`0199`), [duns](https://schema.org/duns) (`0060`) or [GLN](https://schema.org/globalLocationNumber) (`0088`) can be expressed using ISO-6523. If possible, ISO-6523 codes should be preferred to populating [vatID](https://schema.org/vatID) or [taxID](https://schema.org/taxID), as ISO identifiers are less ambiguous. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` knowsAbout ``` | [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a topic that is known about - suggesting possible expertise but not implying it. We do not distinguish skill levels here, or relate this to educational content, events, objectives or [JobPosting](https://schema.org/JobPosting) descriptions. |
| ``` knowsLanguage ``` | [Language](https://schema.org/Language "Language") or [Text](https://schema.org/Text "Text") | Of a [Person](https://schema.org/Person), and less typically of an [Organization](https://schema.org/Organization), to indicate a known language. We do not distinguish skill levels or reading/writing/speaking/signing here. Use language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). |
| ``` legalAddress ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") | The legal address of an organization which acts as the officially registered address used for legal and tax purposes. The legal address can be different from the place of operations of a business and other addresses can be part of an organization. |
| ``` legalName ``` | [Text](https://schema.org/Text "Text") | The official name of the organization, e.g. the registered company name. |
| ``` legalRepresentative ``` | [Person](https://schema.org/Person "Person") | One or multiple persons who represent this organization legally such as CEO or sole administrator. |
| ``` leiCode ``` | [Text](https://schema.org/Text "Text") | An organization identifier that uniquely identifies a legal entity as defined in ISO 17442. |
| ``` location ``` | [Place](https://schema.org/Place "Place") or [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") or [VirtualLocation](https://schema.org/VirtualLocation "VirtualLocation") | The location of, for example, where an event is happening, where an organization is located, or where an action takes place. |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` makesOffer ``` | [Offer](https://schema.org/Offer "Offer") | A pointer to products or services offered by the organization or person. Inverse property: [offeredBy](https://schema.org/offeredBy "offeredBy") |
| ``` member ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A member of an Organization or a ProgramMembership. Organizations can be members of organizations; ProgramMembership is typically for individuals. Supersedes [musicGroupMember](https://schema.org/musicGroupMember "musicGroupMember"), [members](https://schema.org/members "members"). Inverse property: [memberOf](https://schema.org/memberOf "memberOf") |
| ``` memberOf ``` | [MemberProgramTier](https://schema.org/MemberProgramTier "MemberProgramTier") or [Organization](https://schema.org/Organization "Organization") or [ProgramMembership](https://schema.org/ProgramMembership "ProgramMembership") | An Organization (or ProgramMembership) to which this Person or Organization belongs. Inverse property: [member](https://schema.org/member "member") |
| ``` naics ``` | [Text](https://schema.org/Text "Text") | The North American Industry Classification System (NAICS) code for a particular organization or business person. |
| ``` nonprofitStatus ``` | [NonprofitType](https://schema.org/NonprofitType "NonprofitType") | nonprofitStatus indicates the legal status of a non-profit organization in its primary place of business. |
| ``` numberOfEmployees ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") | The number of employees in an organization, e.g. business. |
| ``` ownershipFundingInfo ``` | [AboutPage](https://schema.org/AboutPage "AboutPage") or [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (often but not necessarily a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a description of organizational ownership structure; funding and grants. In a news/media setting, this is with particular reference to editorial independence. Note that the [funder](https://schema.org/funder) is also available and can be used to make basic funder information machine-readable. |
| ``` owns ``` | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") or [Product](https://schema.org/Product "Product") | Products owned by the organization or person. |
| ``` parentOrganization ``` | [Organization](https://schema.org/Organization "Organization") | The larger organization that this organization is a [subOrganization](https://schema.org/subOrganization) of, if any. Supersedes [branchOf](https://schema.org/branchOf "branchOf"). Inverse property: [subOrganization](https://schema.org/subOrganization "subOrganization") |
| ``` publishingPrinciples ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The publishingPrinciples property indicates (typically via [URL](https://schema.org/URL)) a document describing the editorial principles of an [Organization](https://schema.org/Organization) (or individual, e.g. a [Person](https://schema.org/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](https://schema.org/CreativeWork) (e.g. [NewsArticle](https://schema.org/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](https://schema.org/CreativeWork). While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](https://schema.org/funder)) can be expressed using schema.org terminology. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` seeks ``` | [Demand](https://schema.org/Demand "Demand") | A pointer to products or services sought by the organization or person (demand). |
| ``` skills ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A statement of knowledge, skill, ability, task or any other assertion expressing a competency that is either claimed by a person, an organization or desired or required to fulfill a role or to work in an occupation. |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` sponsor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| ``` subOrganization ``` | [Organization](https://schema.org/Organization "Organization") | A relationship between two organizations where the first includes the second, e.g., as a subsidiary. See also: the more specific 'department' property. Inverse property: [parentOrganization](https://schema.org/parentOrganization "parentOrganization") |
| ``` taxID ``` | [Text](https://schema.org/Text "Text") | The Tax / Fiscal ID of the organization or person, e.g. the TIN in the US or the CIF/NIF in Spain. |
| ``` telephone ``` | [Text](https://schema.org/Text "Text") | The telephone number. |
| ``` unnamedSourcesPolicy ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | For an [Organization](https://schema.org/Organization) (typically a [NewsMediaOrganization](https://schema.org/NewsMediaOrganization)), a statement about policy on use of unnamed sources and the decision process required. |
| ``` vatID ``` | [Text](https://schema.org/Text "Text") | The Value-added Tax ID of the organization or person. |
| Properties from [Place](https://schema.org/Place "Place") |
| ``` additionalProperty ``` | [PropertyValue](https://schema.org/PropertyValue "PropertyValue") | A property-value pair representing an additional characteristic of the entity, e.g. a product feature or another characteristic for which there is no matching property in schema.org. Note: Publishers should be aware that applications designed to use specific schema.org properties (e.g. https://schema.org/width, https://schema.org/color, https://schema.org/gtin13, ...) will typically expect such data to be provided using those properties, rather than using the generic property/value mechanism. |
| ``` address ``` | [PostalAddress](https://schema.org/PostalAddress "PostalAddress") or [Text](https://schema.org/Text "Text") | Physical address of the item. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` amenityFeature ``` | [LocationFeatureSpecification](https://schema.org/LocationFeatureSpecification "LocationFeatureSpecification") | An amenity feature (e.g. a characteristic or service) of the Accommodation. This generic property does not make a statement about whether the feature is included in an offer for the main accommodation or available at extra costs. |
| ``` branchCode ``` | [Text](https://schema.org/Text "Text") | A short textual code (also called "store code") that uniquely identifies a place of business. The code is typically assigned by the parentOrganization and used in structured URLs. For example, in the URL http://www.starbucks.co.uk/store-locator/etc/detail/3047 the code "3047" is a branchCode for a particular branch. |
| ``` containedInPlace ``` | [Place](https://schema.org/Place "Place") | The basic containment relation between a place and one that contains it. Supersedes [containedIn](https://schema.org/containedIn "containedIn"). Inverse property: [containsPlace](https://schema.org/containsPlace "containsPlace") |
| ``` containsPlace ``` | [Place](https://schema.org/Place "Place") | The basic containment relation between a place and another that it contains. Inverse property: [containedInPlace](https://schema.org/containedInPlace "containedInPlace") |
| ``` event ``` | [Event](https://schema.org/Event "Event") | Upcoming or past event associated with this place, organization, or action. Supersedes [events](https://schema.org/events "events"). |
| ``` faxNumber ``` | [Text](https://schema.org/Text "Text") | The fax number. |
| ``` geo ``` | [GeoCoordinates](https://schema.org/GeoCoordinates "GeoCoordinates") or [GeoShape](https://schema.org/GeoShape "GeoShape") | The geo coordinates of the place. |
| ``` geoContains ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a containing geometry to a contained geometry. "a contains b iff no points of b lie in the exterior of a, and at least one point of the interior of b lies in the interior of a". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCoveredBy ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that covers it. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCovers ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a covering geometry to a covered geometry. "Every point of b is a point of (the interior or boundary of) a". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoCrosses ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that crosses it: "a crosses b: they have some but not all interior points in common, and the dimension of the intersection is less than that of at least one of them". As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoDisjoint ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) are topologically disjoint: "they have no point in common. They form a set of disconnected geometries." (A symmetric relationship, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM).) |
| ``` geoEquals ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) are topologically equal, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). "Two geometries are topologically equal if their interiors intersect and no part of the interior or boundary of one geometry intersects the exterior of the other" (a symmetric relationship). |
| ``` geoIntersects ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) have at least one point in common. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoOverlaps ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to another that geospatially overlaps it, i.e. they have some but not all points in common. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` geoTouches ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents spatial relations in which two geometries (or the places they represent) touch: "they have at least one boundary point in common, but no interior points." (A symmetric relationship, as defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM).) |
| ``` geoWithin ``` | [GeospatialGeometry](https://schema.org/GeospatialGeometry "GeospatialGeometry") or [Place](https://schema.org/Place "Place") | Represents a relationship between two geometries (or the places they represent), relating a geometry to one that contains it, i.e. it is inside (i.e. within) its interior. As defined in [DE-9IM](https://en.wikipedia.org/wiki/DE-9IM). |
| ``` globalLocationNumber ``` | [Text](https://schema.org/Text "Text") | The [Global Location Number](http://www.gs1.org/gln) (GLN, sometimes also referred to as International Location Number or ILN) of the respective organization, person, or place. The GLN is a 13-digit number used to identify parties and physical locations. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasDriveThroughService ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether some facility (e.g. [FoodEstablishment](https://schema.org/FoodEstablishment), [CovidTestingFacility](https://schema.org/CovidTestingFacility)) offers a service that can be used by driving through in a car. In the case of [CovidTestingFacility](https://schema.org/CovidTestingFacility) such facilities could potentially help with social distancing from other potentially-infected users. |
| ``` hasGS1DigitalLink ``` | [URL](https://schema.org/URL "URL") | The [GS1 digital link](https://www.gs1.org/standards/gs1-digital-link) associated with the object. This URL should conform to the particular requirements of digital links. The link should only contain the Application Identifiers (AIs) that are relevant for the entity being annotated, for instance a [Product](https://schema.org/Product) or an [Organization](https://schema.org/Organization), and for the correct granularity. In particular, for products: * A Digital Link that contains a serial number (AI `21`) should only be present on instances of [IndividualProduct](https://schema.org/IndividualProduct) * A Digital Link that contains a lot number (AI `10`) should be annotated as [SomeProduct](https://schema.org/SomeProduct) if only products from that lot are sold, or [IndividualProduct](https://schema.org/IndividualProduct) if there is only a specific product. * A Digital Link that contains a global model number (AI `8013`) should be attached to a [Product](https://schema.org/Product) or a [ProductModel](https://schema.org/ProductModel). Other item types should be adapted similarly. |
| ``` hasMap ``` | [Map](https://schema.org/Map "Map") or [URL](https://schema.org/URL "URL") | A URL to a map of the place. Supersedes [maps](https://schema.org/maps "maps"), [map](https://schema.org/map "map"). |
| ``` isAccessibleForFree ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](https://schema.org/free "free"). |
| ``` isicV4 ``` | [Text](https://schema.org/Text "Text") | The International Standard of Industrial Classification of All Economic Activities (ISIC), Revision 4 code for a particular organization, business person, or place. |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` latitude ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The latitude of a location. For example `37.42242` ([WGS 84](https://en.wikipedia.org/wiki/World_Geodetic_System)). |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` longitude ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The longitude of a location. For example `-122.08585` ([WGS 84](https://en.wikipedia.org/wiki/World_Geodetic_System)). |
| ``` maximumAttendeeCapacity ``` | [Integer](https://schema.org/Integer "Integer") | The total number of individuals that may attend an event or venue. |
| ``` openingHoursSpecification ``` | [OpeningHoursSpecification](https://schema.org/OpeningHoursSpecification "OpeningHoursSpecification") | The opening hours of a certain place. |
| ``` photo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [Photograph](https://schema.org/Photograph "Photograph") | A photograph of this place. Supersedes [photos](https://schema.org/photos "photos"). |
| ``` publicAccess ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the [Place](https://schema.org/Place) is open to public visitors. If this property is omitted there is no assumed default boolean value. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` smokingAllowed ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether it is allowed to smoke in the place, e.g. in the restaurant, hotel or hotel room. |
| ``` specialOpeningHoursSpecification ``` | [OpeningHoursSpecification](https://schema.org/OpeningHoursSpecification "OpeningHoursSpecification") | The special opening hours of a certain place. Use this to explicitly override general opening hours brought in scope by [openingHoursSpecification](https://schema.org/openingHoursSpecification) or [openingHours](https://schema.org/openingHours). |
| ``` telephone ``` | [Text](https://schema.org/Text "Text") | The telephone number. |
| ``` tourBookingPage ``` | [URL](https://schema.org/URL "URL") | A page providing information on how to book a tour of some [Place](https://schema.org/Place), such as an [Accommodation](https://schema.org/Accommodation) or [ApartmentComplex](https://schema.org/ApartmentComplex) in a real estate setting, as well as other kinds of tours as appropriate. |
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
Title: Service - Schema.org Type

URL Source: https://schema.org/Service

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

A service provided by an organization, e.g. delivery service, print services, etc.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [Service](https://schema.org/Service "Service") |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` areaServed ``` | [AdministrativeArea](https://schema.org/AdministrativeArea "AdministrativeArea") or [GeoShape](https://schema.org/GeoShape "GeoShape") or [Place](https://schema.org/Place "Place") or [Text](https://schema.org/Text "Text") | The geographic area where a service or offered item is provided. Supersedes [serviceArea](https://schema.org/serviceArea "serviceArea"). |
| ``` audience ``` | [Audience](https://schema.org/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](https://schema.org/serviceAudience "serviceAudience"). |
| ``` availableChannel ``` | [ServiceChannel](https://schema.org/ServiceChannel "ServiceChannel") | A means of accessing the service (e.g. a phone bank, a web site, a location, etc.). |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` brand ``` | [Brand](https://schema.org/Brand "Brand") or [Organization](https://schema.org/Organization "Organization") | The brand(s) associated with a product or service, or the brand(s) maintained by an organization or business person. |
| ``` broker ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | An entity that arranges for an exchange between a buyer and a seller. In most cases a broker never acquires or releases ownership of a product or service involved in an exchange. If it is not clear whether an entity is a broker, seller, or buyer, the latter two terms are preferred. Supersedes [bookingAgent](https://schema.org/bookingAgent "bookingAgent"). |
| ``` category ``` | [CategoryCode](https://schema.org/CategoryCode "CategoryCode") or [PhysicalActivityCategory](https://schema.org/PhysicalActivityCategory "PhysicalActivityCategory") or [Text](https://schema.org/Text "Text") or [Thing](https://schema.org/Thing "Thing") or [URL](https://schema.org/URL "URL") | A category for the item. Greater signs or slashes can be used to informally indicate a category hierarchy. |
| ``` hasCertification ``` | [Certification](https://schema.org/Certification "Certification") | Certification information about a product, organization, service, place, or person. |
| ``` hasOfferCatalog ``` | [OfferCatalog](https://schema.org/OfferCatalog "OfferCatalog") | Indicates an OfferCatalog listing for this Organization, Person, or Service. |
| ``` hoursAvailable ``` | [OpeningHoursSpecification](https://schema.org/OpeningHoursSpecification "OpeningHoursSpecification") | The hours during which this service or contact is available. |
| ``` isRelatedTo ``` | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, somehow related product (or multiple products). |
| ``` isSimilarTo ``` | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, functionally similar product (or multiple products). |
| ``` logo ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") or [URL](https://schema.org/URL "URL") | An associated logo. |
| ``` offers ``` | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](https://schema.org/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](https://schema.org/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [itemOffered](https://schema.org/itemOffered "itemOffered") |
| ``` provider ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](https://schema.org/carrier "carrier"). |
| ``` providerMobility ``` | [Text](https://schema.org/Text "Text") | Indicates the mobility of a provided service (e.g. 'static', 'dynamic'). |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` serviceOutput ``` | [Thing](https://schema.org/Thing "Thing") | The tangible thing generated by the service, e.g. a passport, permit, etc. Supersedes [produces](https://schema.org/produces "produces"). |
| ``` serviceType ``` | [GovernmentBenefitsType](https://schema.org/GovernmentBenefitsType "GovernmentBenefitsType") or [Text](https://schema.org/Text "Text") | The type of service being offered, e.g. veterans' benefits, emergency relief, etc. |
| ``` slogan ``` | [Text](https://schema.org/Text "Text") | A slogan or motto associated with the item. |
| ``` termsOfService ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Human-readable terms of service documentation. |
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

Instances of [Service](https://schema.org/Service "Service") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [isRelatedTo](https://schema.org/isRelatedTo "isRelatedTo") | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, somehow related product (or multiple products). |
| [isSimilarTo](https://schema.org/isSimilarTo "isSimilarTo") | [Product](https://schema.org/Product "Product") or [Service](https://schema.org/Service "Service") | A pointer to another, functionally similar product (or multiple products). |
| [issuedThrough](https://schema.org/issuedThrough "issuedThrough") | [Permit](https://schema.org/Permit "Permit") | The service through which the permit was granted. |
| [itemOffered](https://schema.org/itemOffered "itemOffered") | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An item being offered (or demanded). The transactional nature of the offer or demand is documented using [businessFunction](https://schema.org/businessFunction), e.g. sell, lease etc. While several common expected types are listed explicitly in this definition, others can be used. Using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. |
| [orderedItem](https://schema.org/orderedItem "orderedItem") | [Order](https://schema.org/Order "Order") or [OrderItem](https://schema.org/OrderItem "OrderItem") | The item ordered. |
| [providesService](https://schema.org/providesService "providesService") | [ServiceChannel](https://schema.org/ServiceChannel "ServiceChannel") | The service provided by this channel. |
| [typeOfGood](https://schema.org/typeOfGood "typeOfGood") | [OwnershipInfo](https://schema.org/OwnershipInfo "OwnershipInfo") or [TypeAndQuantityNode](https://schema.org/TypeAndQuantityNode "TypeAndQuantityNode") | The product that this structured value is referring to. |

#### More specific Types

*   [BroadcastService](https://schema.org/BroadcastService "BroadcastService")
*   [CableOrSatelliteService](https://schema.org/CableOrSatelliteService "CableOrSatelliteService")
*   [FinancialProduct](https://schema.org/FinancialProduct "FinancialProduct")
*   [FoodService](https://schema.org/FoodService "FoodService")
*   [GovernmentService](https://schema.org/GovernmentService "GovernmentService")
*   [TaxiService](https://schema.org/TaxiService "TaxiService")
*   [WebAPI](https://schema.org/WebAPI "WebAPI")

### Examples
```
    <script type="application/ld+json">
    {
        "@context": "https://schema.org/",
        "@type": "Invoice",
        "broker": {
          "@type": "LocalBusiness",
          "name": "ACME Home Heating"
        },
        "accountId": "xxxx-xxxx-xxxx-1234",
        "customer": {
          "@type": "Person",
          "name": "Jane Doe"
        },
        "paymentDueDate": "2015-01-30",
        "minimumPaymentDue": {
          "@type": "PriceSpecification",
          "price": 0.00,
          "priceCurrency": "USD"
        },
        "totalPaymentDue": {
          "@type": "PriceSpecification",
          "price": 0.00,
          "priceCurrency": "USD"
        },
        "paymentStatus": "https://schema.org/PaymentComplete",
        "referencesOrder": [
          {
            "@type": "Order",
            "description": "furnace",
            "orderDate": "2014-12-01",
            "orderNumber": "123ABC",
            "paymentMethod": "http://purl.org/goodrelations/v1#ByInvoice",
            "orderedItem": {
              "@type": "Product",
              "name": "ACME Furnace 3000",
              "productID": "ABC123"
            }
          },
          {
            "@type": "Order",
            "description": "furnace installation",
            "orderDate": "2014-12-02",
            "paymentMethod": "http://purl.org/goodrelations/v1#ByInvoice",
            "orderedItem": {
              "@type": "Service",
              "description": "furnace installation"
            }
          }
        ]
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
```
    <!--- See https://github.com/ESIPFed/science-on-schema.org/blob/master/guides/DataRepository.md for a complete guide. --->

    <script type="application/ld+json">
    {
      "@context": {
        "@vocab": "https://schema.org/"
      },
      "@type": [
        "Service",
        "ResearchProject"
      ],
      "legalName": "Sample Data Repository Office",
      "name": "SDRO",
      "url": "https://www.sample-data-repository.org",
      "description": "The Sample Data Repository Service provides access to data from an imaginary domain accessible from this website.",
      "sameAs": [
        "http://www.re3data.org/repository/r3d1000000xx",
        "https://twitter.com/SDRO",
        "https://www.linkedin.com/company/123456789/"
      ],
      "category": [
        "Biological Oceanography",
        "Chemical Oceanography"
      ],
      "provider": [
        {
          "@type": "ResearchProject",
          "name": "SDRO Technical Office",
          "description": "We provide all the infrastructure for the SDRO"
        },
        {
          "@type": "ResearchProject",
          "name": "SDRO Science Support Office",
          "description": "We provide all the science support functionality for the SDRO"
        }
      ],
      "logo": {
        "@type": "ImageObject",
        "url": "https://www.sample-data-repository.org/images/logo.jpg"
      },
      "contactPoint": {
        "@type": "ContactPoint",
        "name": "Support",
        "email": "info@bco-dmo.org",
        "url": "https://www.sample-data-repository.org/about-us",
        "contactType": "customer support"
      },
      "foundingDate": "2006-09-01",
      "address": {
        "@type": "PostalAddress",
        "streetAddress": "123 Main St.",
        "addressLocality": "Anytown",
        "addressRegion": "ST",
        "postalCode": "12345",
        "addressCountry": "USA"
      },
      "parentOrganization": {
        "@type": "Organization",
        "@id": "http://www.someinstitute.edu",
        "legalName": "Some Institute",
        "name": "SI",
        "url": "http://www.someinstitute.edu",
        "address": {
          "@type": "PostalAddress",
          "streetAddress": "234 Main St.",
          "addressLocality": "Anytown",
          "addressRegion": "ST",
          "postalCode": "12345",
          "addressCountry": "USA"
        }
      },
      "identifier": {
        "@type": "PropertyValue",
        "name": "Re3data DOI: 10.17616/R37P4C",
        "propertyID": "https://registry.identifiers.org/registry/doi",
        "value": "doi:10.17616/R37P4C",
        "url": "https://doi.org/10.17616/R37P4C"
      },
      "funder": {
        "@type": "Organization",
        "@id": "https://doi.org/10.13039/100000141",
        "legalName": "Division of Ocean Sciences",
        "alternateName": "OCE",
        "url": "https://www.nsf.gov/div/index.jsp?div=OCE",
        "identifier": {
          "@type": "PropertyValue",
          "propertyID": "https://registry.identifiers.org/registry/doi",
          "value": "doi:10.13039/100000141",
          "url": "https://doi.org/10.13039/100000141"
        },
        "parentOrganization": {
          "@type": "Organization",
          "@id": "http://doi.org/10.13039/100000085",
          "legalName": "Directorate for Geosciences",
          "alternateName": "NSF-GEO",
          "url": "http://www.nsf.gov",
          "identifier": {
            "@type": "PropertyValue",
            "propertyID": "https://registry.identifiers.org/registry/doi",
            "value": "doi:10.13039/100000085",
            "url": "https://doi.org/10.13039/100000085"
          },
          "parentOrganization": {
            "@type": "Organization",
            "@id": "http://dx.doi.org/10.13039/100000001",
            "legalName": "National Science Foundation",
            "alternateName": "NSF",
            "url": "http://www.nsf.gov",
            "identifier": {
              "@type": "PropertyValue",
              "propertyID": "https://registry.identifiers.org/registry/doi",
              "value": "doi:10.13039/100000001",
              "url": "https://doi.org/10.13039/100000001"
            }
          }
        }
      },
      "availableChannel": [
        {
          "@type": "ServiceChannel",
          "serviceUrl": "https://www.sample-data-repository.org/search",
          "providesService": {
            "@type": "Service",
            "name": "SDRO Website Search",
            "description": "Search for webpages, datasets, authors, funding awards, instrumentation and measurements",
            "potentialAction": {
              "@type": "SearchAction",
              "target": "https://www.sample-data-repository.org/search?keywords={query_string}"
            }
          }
        }
      ],
      "hasOfferCatalog": {
        "@type": "OfferCatalog",
        "name": "Sample Data Repository Resource Catalog",
        "itemListElement": [
          {
            "@type": "DataCatalog",
            "@id": "https://www.sample-data-repository.org/collection/biological-data",
            "name": "Biological Data",
            "audience": {
              "@type": "Audience",
              "audienceType": "public",
              "name": "General Public"
            }
          },
          {
            "@type": "DataCatalog",
            "@id": "https://www.sample-data-repository.org/collection/geological-data",
            "name": "Geological Data",
            "audience": {
              "@type": "Audience",
              "audienceType": "public",
              "name": "General Public"
            }
          }
        ]
      }
    }
    </script>
```Title: WebPage - Schema.org Type

URL Source: https://schema.org/WebPage

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

A web page. Every web page is implicitly assumed to be declared to be of type WebPage, so the various properties about that webpage, such as `breadcrumb` may be used. We recommend explicit declaration if these properties are specified, but if they are found outside of an itemscope, they will be assumed to be about the page.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [WebPage](https://schema.org/WebPage "WebPage") |
| ``` breadcrumb ``` | [BreadcrumbList](https://schema.org/BreadcrumbList "BreadcrumbList") or [Text](https://schema.org/Text "Text") | A set of links that can help a user understand and navigate a website hierarchy. |
| ``` lastReviewed ``` | [Date](https://schema.org/Date "Date") | Date on which the content on this web page was last reviewed for accuracy and/or completeness. |
| ``` mainContentOfPage ``` | [WebPageElement](https://schema.org/WebPageElement "WebPageElement") | Indicates if this web page element is the main subject of the page. Supersedes [aspect](https://schema.org/aspect "aspect"). |
| ``` primaryImageOfPage ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") | Indicates the main image on the page. |
| ``` relatedLink ``` | [URL](https://schema.org/URL "URL") | A link related to this web page, for example to other related web pages. |
| ``` reviewedBy ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | People or organizations that have reviewed the content on this web page for accuracy and/or completeness. |
| ``` significantLink ``` | [URL](https://schema.org/URL "URL") | One of the more significant URLs on the page. Typically, these are the non-navigation links that are clicked on the most. Supersedes [significantLinks](https://schema.org/significantLinks "significantLinks"). |
| ``` speakable ``` | [SpeakableSpecification](https://schema.org/SpeakableSpecification "SpeakableSpecification") or [URL](https://schema.org/URL "URL") | Indicates sections of a Web page that are particularly 'speakable' in the sense of being highlighted as being especially appropriate for text-to-speech conversion. Other sections of a page may also be usefully spoken in particular circumstances; the 'speakable' property serves to indicate the parts most likely to be generally useful for speech. The _speakable_ property can be repeated an arbitrary number of times, with three kinds of possible 'content-locator' values: 1.) _id-value_ URL references - uses _id-value_ of an element in the page being annotated. The simplest use of _speakable_ has (potentially relative) URL values, referencing identified sections of the document concerned. 2.) CSS Selectors - addresses content in the annotated page, e.g. via class attribute. Use the [cssSelector](https://schema.org/cssSelector) property. 3.) XPaths - addresses content via XPaths (assuming an XML view of the content). Use the [xpath](https://schema.org/xpath) property. For more sophisticated markup of speakable sections beyond simple ID references, either CSS selectors or XPath expressions to pick out document section(s) as speakable. For this we define a supporting type, [SpeakableSpecification](https://schema.org/SpeakableSpecification) which is defined to be a possible value of the _speakable_ property. |
| ``` specialty ``` | [Specialty](https://schema.org/Specialty "Specialty") | One of the domain specialities to which this web page's content applies. |
| Properties from [CreativeWork](https://schema.org/CreativeWork "CreativeWork") |
| ``` about ``` | [Thing](https://schema.org/Thing "Thing") | The subject matter of the content. Inverse property: [subjectOf](https://schema.org/subjectOf "subjectOf") |
| ``` abstract ``` | [Text](https://schema.org/Text "Text") | An abstract is a short description that summarizes a [CreativeWork](https://schema.org/CreativeWork). |
| ``` accessMode ``` | [Text](https://schema.org/Text "Text") | The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessMode-vocabulary). |
| ``` accessModeSufficient ``` | [ItemList](https://schema.org/ItemList "ItemList") | A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessModeSufficient-vocabulary). |
| ``` accessibilityAPI ``` | [Text](https://schema.org/Text "Text") | Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityAPI-vocabulary). |
| ``` accessibilityControl ``` | [Text](https://schema.org/Text "Text") | Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityControl-vocabulary). |
| ``` accessibilityFeature ``` | [Text](https://schema.org/Text "Text") | Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityFeature-vocabulary). |
| ``` accessibilityHazard ``` | [Text](https://schema.org/Text "Text") | A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityHazard-vocabulary). |
| ``` accessibilitySummary ``` | [Text](https://schema.org/Text "Text") | A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed". |
| ``` accountablePerson ``` | [Person](https://schema.org/Person "Person") | Specifies the Person that is legally accountable for the CreativeWork. |
| ``` acquireLicensePage ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` alternativeHeadline ``` | [Text](https://schema.org/Text "Text") | A secondary title of the CreativeWork. |
| ``` archivedAt ``` | [URL](https://schema.org/URL "URL") or [WebPage](https://schema.org/WebPage "WebPage") | Indicates a page or other link involved in archival of a [CreativeWork](https://schema.org/CreativeWork). In the case of [MediaReview](https://schema.org/MediaReview), the items in a [MediaReviewItem](https://schema.org/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content. |
| ``` assesses ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The item being described is intended to assess the competency or learning outcome defined by the referenced term. |
| ``` associatedMedia ``` | [MediaObject](https://schema.org/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for encoding. |
| ``` audience ``` | [Audience](https://schema.org/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](https://schema.org/serviceAudience "serviceAudience"). |
| ``` audio ``` | [AudioObject](https://schema.org/AudioObject "AudioObject") or [Clip](https://schema.org/Clip "Clip") or [MusicRecording](https://schema.org/MusicRecording "MusicRecording") | An embedded audio object. |
| ``` author ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` character ``` | [Person](https://schema.org/Person "Person") | Fictional person connected with a creative work. |
| ``` citation ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Text](https://schema.org/Text "Text") | A citation or reference to another creative work, such as another publication, web page, scholarly article, etc. |
| ``` comment ``` | [Comment](https://schema.org/Comment "Comment") | Comments, typically from users. |
| ``` commentCount ``` | [Integer](https://schema.org/Integer "Integer") | The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere. |
| ``` conditionsOfAccess ``` | [Text](https://schema.org/Text "Text") | Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an [ArchiveComponent](https://schema.org/ArchiveComponent) held by an [ArchiveOrganization](https://schema.org/ArchiveOrganization). This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language. For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts ". |
| ``` contentLocation ``` | [Place](https://schema.org/Place "Place") | The location depicted or described in the content. For example, the location in a photograph or painting. |
| ``` contentRating ``` | [Rating](https://schema.org/Rating "Rating") or [Text](https://schema.org/Text "Text") | Official rating of a piece of content—for example, 'MPAA PG-13'. |
| ``` contentReferenceTime ``` | [DateTime](https://schema.org/DateTime "DateTime") | The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event. |
| ``` contributor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A secondary contributor to the CreativeWork or Event. |
| ``` copyrightHolder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The party holding the legal copyright to the CreativeWork. |
| ``` copyrightNotice ``` | [Text](https://schema.org/Text "Text") | Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work. |
| ``` copyrightYear ``` | [Number](https://schema.org/Number "Number") | The year during which the claimed copyright for the CreativeWork was first asserted. |
| ``` correction ``` | [CorrectionComment](https://schema.org/CorrectionComment "CorrectionComment") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Indicates a correction to a [CreativeWork](https://schema.org/CreativeWork), either via a [CorrectionComment](https://schema.org/CorrectionComment), textually or in another document. |
| ``` countryOfOrigin ``` | [Country](https://schema.org/Country "Country") | The country of origin of something, including products as well as creative works such as movie and TV content. In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](https://schema.org/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](https://schema.org/contentLocation) and [locationCreated](https://schema.org/locationCreated) may be more applicable. In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here. |
| ``` creativeWorkStatus ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle. |
| ``` creator ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| ``` creditText ``` | [Text](https://schema.org/Text "Text") | Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work. |
| ``` dateCreated ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date on which the CreativeWork was created or the item was added to a DataFeed. |
| ``` dateModified ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed. |
| ``` datePublished ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | Date of first publication or broadcast. For example the date a [CreativeWork](https://schema.org/CreativeWork) was broadcast or a [Certification](https://schema.org/Certification) was issued. |
| ``` digitalSourceType ``` | [IPTCDigitalSourceEnumeration](https://schema.org/IPTCDigitalSourceEnumeration "IPTCDigitalSourceEnumeration") | Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some [CreativeWork](https://schema.org/CreativeWork). |
| ``` discussionUrl ``` | [URL](https://schema.org/URL "URL") | A link to the page containing the comments of the CreativeWork. |
| ``` editEIDR ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | An [EIDR](https://eidr.org/) (Entertainment Identifier Registry) [identifier](https://schema.org/identifier) representing a specific edit / edition for a work of film or television. For example, the motion picture known as "Ghostbusters" whose [titleEIDR](https://schema.org/titleEIDR) is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3". Since schema.org types like [Movie](https://schema.org/Movie) and [TVEpisode](https://schema.org/TVEpisode) can be used for both works and their multiple expressions, it is possible to use [titleEIDR](https://schema.org/titleEIDR) alone (for a general description), or alongside [editEIDR](https://schema.org/editEIDR) for a more edit-specific description. |
| ``` editor ``` | [Person](https://schema.org/Person "Person") | Specifies the Person who edited the CreativeWork. |
| ``` educationalAlignment ``` | [AlignmentObject](https://schema.org/AlignmentObject "AlignmentObject") | An alignment to an established educational framework. This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource [teaches](https://schema.org/teaches) or [assesses](https://schema.org/assesses) a competency. |
| ``` educationalLevel ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators. |
| ``` educationalUse ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The purpose of a work in the context of education; for example, 'assignment', 'group work'. |
| ``` encoding ``` | [MediaObject](https://schema.org/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes [encodings](https://schema.org/encodings "encodings"). Inverse property: [encodesCreativeWork](https://schema.org/encodesCreativeWork "encodesCreativeWork") |
| ``` encodingFormat ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Media type typically expressed using a MIME format (see [IANA site](http://www.iana.org/assignments/media-types/media-types.xhtml) and [MDN reference](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc. In cases where a [CreativeWork](https://schema.org/CreativeWork) has several media type representations, [encoding](https://schema.org/encoding) can be used to indicate each [MediaObject](https://schema.org/MediaObject) alongside particular [encodingFormat](https://schema.org/encodingFormat) information. Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes [fileFormat](https://schema.org/fileFormat "fileFormat"). |
| ``` exampleOfWork ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A creative work that this work is an example/instance/realization/derivation of. Inverse property: [workExample](https://schema.org/workExample "workExample") |
| ``` expires ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | Date the content expires and is no longer useful or available. For example a [VideoObject](https://schema.org/VideoObject) or [NewsArticle](https://schema.org/NewsArticle) whose availability or relevance is time-limited, a [ClaimReview](https://schema.org/ClaimReview) fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a [Certification](https://schema.org/Certification) the validity has expired. |
| ``` funder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` genre ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Genre of the creative work, broadcast channel or group. |
| ``` hasPart ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense). Inverse property: [isPartOf](https://schema.org/isPartOf "isPartOf") |
| ``` headline ``` | [Text](https://schema.org/Text "Text") | Headline of the article. |
| ``` inLanguage ``` | [Language](https://schema.org/Language "Language") or [Text](https://schema.org/Text "Text") | The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](https://schema.org/availableLanguage). Supersedes [language](https://schema.org/language "language"). |
| ``` interactionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](https://schema.org/interactionCount "interactionCount"). |
| ``` interactivityType ``` | [Text](https://schema.org/Text "Text") | The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'. |
| ``` interpretedAsClaim ``` | [Claim](https://schema.org/Claim "Claim") | Used to indicate a specific claim contained, implied, translated or refined from the content of a [MediaObject](https://schema.org/MediaObject) or other [CreativeWork](https://schema.org/CreativeWork). The interpreting party can be indicated using [claimInterpreter](https://schema.org/claimInterpreter). |
| ``` isAccessibleForFree ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](https://schema.org/free "free"). |
| ``` isBasedOn ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Product](https://schema.org/Product "Product") or [URL](https://schema.org/URL "URL") | A resource from which this work is derived or from which it is a modification or adaptation. Supersedes [isBasedOnUrl](https://schema.org/isBasedOnUrl "isBasedOnUrl"). |
| ``` isFamilyFriendly ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether this content is family friendly. |
| ``` isPartOf ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of. Inverse property: [hasPart](https://schema.org/hasPart "hasPart") |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` learningResourceType ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'. |
| ``` license ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | A license document that applies to this content, typically indicated by URL. |
| ``` locationCreated ``` | [Place](https://schema.org/Place "Place") | The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork. |
| ``` mainEntity ``` | [Thing](https://schema.org/Thing "Thing") | Indicates the primary entity described in some page or other CreativeWork. Inverse property: [mainEntityOfPage](https://schema.org/mainEntityOfPage "mainEntityOfPage") |
| ``` maintainer ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A maintainer of a [Dataset](https://schema.org/Dataset), software package ([SoftwareApplication](https://schema.org/SoftwareApplication)), or other [Project](https://schema.org/Project). A maintainer is a [Person](https://schema.org/Person) or [Organization](https://schema.org/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](https://schema.org/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](https://schema.org/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](https://schema.org/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| ``` material ``` | [Product](https://schema.org/Product "Product") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| ``` materialExtent ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") or [Text](https://schema.org/Text "Text") | The quantity of the materials being described or an expression of the physical space they occupy. |
| ``` mentions ``` | [Thing](https://schema.org/Thing "Thing") | Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept. |
| ``` offers ``` | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](https://schema.org/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](https://schema.org/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [itemOffered](https://schema.org/itemOffered "itemOffered") |
| ``` pattern ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported. |
| ``` position ``` | [Integer](https://schema.org/Integer "Integer") or [Text](https://schema.org/Text "Text") | The position of an item in a series or sequence of items. |
| ``` producer ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| ``` provider ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](https://schema.org/carrier "carrier"). |
| ``` publication ``` | [PublicationEvent](https://schema.org/PublicationEvent "PublicationEvent") | A publication event associated with the item. |
| ``` publisher ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The publisher of the article in question. |
| ``` publisherImprint ``` | [Organization](https://schema.org/Organization "Organization") | The publishing division which published the comic. |
| ``` publishingPrinciples ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The publishingPrinciples property indicates (typically via [URL](https://schema.org/URL)) a document describing the editorial principles of an [Organization](https://schema.org/Organization) (or individual, e.g. a [Person](https://schema.org/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](https://schema.org/CreativeWork) (e.g. [NewsArticle](https://schema.org/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](https://schema.org/CreativeWork). While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](https://schema.org/funder)) can be expressed using schema.org terminology. |
| ``` recordedAt ``` | [Event](https://schema.org/Event "Event") | The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event. Inverse property: [recordedIn](https://schema.org/recordedIn "recordedIn") |
| ``` releasedEvent ``` | [PublicationEvent](https://schema.org/PublicationEvent "PublicationEvent") | The place and time the release was issued, expressed as a PublicationEvent. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` schemaVersion ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. `10.0` as a simple string, or more explicitly via URL, `https://schema.org/docs/releases.html#v10.0`. There may be situations in which other schemas might usefully be referenced this way, e.g. `http://dublincore.org/specifications/dublin-core/dces/1999-07-02/` but this has not been carefully explored in the community. |
| ``` sdDatePublished ``` | [Date](https://schema.org/Date "Date") | Indicates the date on which the current structured data was generated / published. Typically used alongside [sdPublisher](https://schema.org/sdPublisher). |
| ``` sdLicense ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | A license document that applies to this structured data, typically indicated by URL. |
| ``` sdPublisher ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](https://schema.org/sdPublisher) property helps make such practices more explicit. |
| ``` size ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") or [SizeSpecification](https://schema.org/SizeSpecification "SizeSpecification") or [Text](https://schema.org/Text "Text") | A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](https://schema.org/SizeSpecification); in other cases, the [width](https://schema.org/width), [height](https://schema.org/height), [depth](https://schema.org/depth) and [weight](https://schema.org/weight) properties may be more applicable. |
| ``` sourceOrganization ``` | [Organization](https://schema.org/Organization "Organization") | The Organization on whose behalf the creator was working. |
| ``` spatial ``` | [Place](https://schema.org/Place "Place") | The "spatial" property can be used in cases when more specific properties (e.g. [locationCreated](https://schema.org/locationCreated), [spatialCoverage](https://schema.org/spatialCoverage), [contentLocation](https://schema.org/contentLocation)) are not known to be appropriate. |
| ``` spatialCoverage ``` | [Place](https://schema.org/Place "Place") | The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York. |
| ``` sponsor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| ``` teaches ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term. |
| ``` temporal ``` | [DateTime](https://schema.org/DateTime "DateTime") or [Text](https://schema.org/Text "Text") | The "temporal" property can be used in cases where more specific properties (e.g. [temporalCoverage](https://schema.org/temporalCoverage), [dateCreated](https://schema.org/dateCreated), [dateModified](https://schema.org/dateModified), [datePublished](https://schema.org/datePublished)) are not known to be appropriate. |
| ``` temporalCoverage ``` | [DateTime](https://schema.org/DateTime "DateTime") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in [ISO 8601 time interval format](https://en.wikipedia.org/wiki/ISO_8601#Time_intervals). In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945". Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes [datasetTimeInterval](https://schema.org/datasetTimeInterval "datasetTimeInterval"). |
| ``` text ``` | [Text](https://schema.org/Text "Text") | The textual content of this CreativeWork. |
| ``` thumbnail ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") | Thumbnail image for an image or video. |
| ``` thumbnailUrl ``` | [URL](https://schema.org/URL "URL") | A thumbnail image relevant to the Thing. |
| ``` timeRequired ``` | [Duration](https://schema.org/Duration "Duration") | Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience. |
| ``` translationOfWork ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”. Inverse property: [workTranslation](https://schema.org/workTranslation "workTranslation") |
| ``` translator ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| ``` typicalAgeRange ``` | [Text](https://schema.org/Text "Text") | The typical expected age range, e.g. '7-9', '11-'. |
| ``` usageInfo ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The schema.org [usageInfo](https://schema.org/usageInfo) property indicates further information about a [CreativeWork](https://schema.org/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options. This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses. |
| ``` version ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The version of the CreativeWork embodied by a specified resource. |
| ``` video ``` | [Clip](https://schema.org/Clip "Clip") or [VideoObject](https://schema.org/VideoObject "VideoObject") | An embedded video object. |
| ``` wordCount ``` | [Integer](https://schema.org/Integer "Integer") | The number of words in the text of the CreativeWork such as an Article, Book, etc. |
| ``` workExample ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book. Inverse property: [exampleOfWork](https://schema.org/exampleOfWork "exampleOfWork") |
| ``` workTranslation ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo. Inverse property: [translationOfWork](https://schema.org/translationOfWork "translationOfWork") |
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

Instances of [WebPage](https://schema.org/WebPage "WebPage") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [archivedAt](https://schema.org/archivedAt "archivedAt") | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Indicates a page or other link involved in archival of a [CreativeWork](https://schema.org/CreativeWork). In the case of [MediaReview](https://schema.org/MediaReview), the items in a [MediaReviewItem](https://schema.org/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content. |
| [originalMediaLink](https://schema.org/originalMediaLink "originalMediaLink") | [MediaReview](https://schema.org/MediaReview "MediaReview") | Link to the page containing an original version of the content, or directly to an online copy of the original [MediaObject](https://schema.org/MediaObject) content, e.g. video file. |

#### More specific Types

*   [AboutPage](https://schema.org/AboutPage "AboutPage")
*   [CheckoutPage](https://schema.org/CheckoutPage "CheckoutPage")
*   [CollectionPage](https://schema.org/CollectionPage "CollectionPage")
*   [ContactPage](https://schema.org/ContactPage "ContactPage")
*   [FAQPage](https://schema.org/FAQPage "FAQPage")
*   [ItemPage](https://schema.org/ItemPage "ItemPage")
*   [MedicalWebPage](https://schema.org/MedicalWebPage "MedicalWebPage")
*   [ProfilePage](https://schema.org/ProfilePage "ProfilePage")
*   [QAPage](https://schema.org/QAPage "QAPage")
*   [RealEstateListing](https://schema.org/RealEstateListing "RealEstateListing")
*   [SearchResultsPage](https://schema.org/SearchResultsPage "SearchResultsPage")

### Examples
```
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "WebPage",
        "name": "Lecture 12: Graphs, networks, incidence matrices",
        "description": "These video lectures of Professor Gilbert Strang teaching 18.06 were recorded in Fall 1999 and do not correspond precisely to the current  edition of the textbook.",
        "publisher": {
            "@type": "CollegeOrUniversity",
            "name": "MIT OpenCourseWare"
        },
        "license": "http://creativecommons.org/licenses/by-nc-sa/3.0/us/deed.en_US"
    }
    </script>
```
```
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "WebPage",
      "breadcrumb": "Books > Literature & Fiction > Classics",
      "mainEntity":{
              "@type": "Book",
              "author": "/author/jd_salinger.html",
              "bookFormat": "https://schema.org/Paperback",
              "datePublished": "1991-05-01",
              "image": "catcher-in-the-rye-book-cover.jpg",
              "inLanguage": "English",
              "isbn": "0316769487",
              "name": "The Catcher in the Rye",
              "numberOfPages": "224",
              "offers": {
                "@type": "Offer",
                "availability": "https://schema.org/InStock",
                "price": "6.99",
                "priceCurrency": "USD"
              },
              "publisher": "Little, Brown, and Company",
              "aggregateRating": {
                "@type": "AggregateRating",
                "ratingValue": "4",
                "reviewCount": "3077"
              },
              "review": [
                {
                  "@type": "Review",
                  "author": "John Doe",
                  "datePublished": "2006-05-04",
                  "name": "A masterpiece of literature",
                  "reviewBody": "I really enjoyed this book. It captures the essential challenge people face as they try make sense of their lives and grow to adulthood.",
                  "reviewRating": {
                "@type": "Rating",
                "ratingValue": "5"
               }
                },
                {
                  "@type": "Review",
                  "author": "Bob Smith",
                  "datePublished": "2006-06-15",
                  "name": "A good read.",
                  "reviewBody": "Catcher in the Rye is a fun book. It's a good book to read.",
                  "reviewRating": "4"
                }
              ]
            }
    }
    </script>
```Title: WebSite - Schema.org Type

URL Source: https://schema.org/WebSite

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Type

A WebSite is a set of related web pages and other items typically served from a single web domain and accessible via URLs.

| Property | Expected Type | Description |
| --- | --- | --- |
| Properties from [WebSite](https://schema.org/WebSite "WebSite") |
| ``` issn ``` | [Text](https://schema.org/Text "Text") | The International Standard Serial Number (ISSN) that identifies this serial publication. You can repeat this property to identify different formats of, or the linking ISSN (ISSN-L) for, this serial publication. |
| Properties from [CreativeWork](https://schema.org/CreativeWork "CreativeWork") |
| ``` about ``` | [Thing](https://schema.org/Thing "Thing") | The subject matter of the content. Inverse property: [subjectOf](https://schema.org/subjectOf "subjectOf") |
| ``` abstract ``` | [Text](https://schema.org/Text "Text") | An abstract is a short description that summarizes a [CreativeWork](https://schema.org/CreativeWork). |
| ``` accessMode ``` | [Text](https://schema.org/Text "Text") | The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessMode-vocabulary). |
| ``` accessModeSufficient ``` | [ItemList](https://schema.org/ItemList "ItemList") | A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessModeSufficient-vocabulary). |
| ``` accessibilityAPI ``` | [Text](https://schema.org/Text "Text") | Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityAPI-vocabulary). |
| ``` accessibilityControl ``` | [Text](https://schema.org/Text "Text") | Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityControl-vocabulary). |
| ``` accessibilityFeature ``` | [Text](https://schema.org/Text "Text") | Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityFeature-vocabulary). |
| ``` accessibilityHazard ``` | [Text](https://schema.org/Text "Text") | A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3. Values should be drawn from the [approved vocabulary](https://www.w3.org/2021/a11y-discov-vocab/latest/#accessibilityHazard-vocabulary). |
| ``` accessibilitySummary ``` | [Text](https://schema.org/Text "Text") | A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed". |
| ``` accountablePerson ``` | [Person](https://schema.org/Person "Person") | Specifies the Person that is legally accountable for the CreativeWork. |
| ``` acquireLicensePage ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item. |
| ``` aggregateRating ``` | [AggregateRating](https://schema.org/AggregateRating "AggregateRating") | The overall rating, based on a collection of reviews or ratings, of the item. |
| ``` alternativeHeadline ``` | [Text](https://schema.org/Text "Text") | A secondary title of the CreativeWork. |
| ``` archivedAt ``` | [URL](https://schema.org/URL "URL") or [WebPage](https://schema.org/WebPage "WebPage") | Indicates a page or other link involved in archival of a [CreativeWork](https://schema.org/CreativeWork). In the case of [MediaReview](https://schema.org/MediaReview), the items in a [MediaReviewItem](https://schema.org/MediaReviewItem) may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content. |
| ``` assesses ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The item being described is intended to assess the competency or learning outcome defined by the referenced term. |
| ``` associatedMedia ``` | [MediaObject](https://schema.org/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for encoding. |
| ``` audience ``` | [Audience](https://schema.org/Audience "Audience") | An intended audience, i.e. a group for whom something was created. Supersedes [serviceAudience](https://schema.org/serviceAudience "serviceAudience"). |
| ``` audio ``` | [AudioObject](https://schema.org/AudioObject "AudioObject") or [Clip](https://schema.org/Clip "Clip") or [MusicRecording](https://schema.org/MusicRecording "MusicRecording") | An embedded audio object. |
| ``` author ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably. |
| ``` award ``` | [Text](https://schema.org/Text "Text") | An award won by or for this item. Supersedes [awards](https://schema.org/awards "awards"). |
| ``` character ``` | [Person](https://schema.org/Person "Person") | Fictional person connected with a creative work. |
| ``` citation ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Text](https://schema.org/Text "Text") | A citation or reference to another creative work, such as another publication, web page, scholarly article, etc. |
| ``` comment ``` | [Comment](https://schema.org/Comment "Comment") | Comments, typically from users. |
| ``` commentCount ``` | [Integer](https://schema.org/Integer "Integer") | The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere. |
| ``` conditionsOfAccess ``` | [Text](https://schema.org/Text "Text") | Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an [ArchiveComponent](https://schema.org/ArchiveComponent) held by an [ArchiveOrganization](https://schema.org/ArchiveOrganization). This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language. For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts ". |
| ``` contentLocation ``` | [Place](https://schema.org/Place "Place") | The location depicted or described in the content. For example, the location in a photograph or painting. |
| ``` contentRating ``` | [Rating](https://schema.org/Rating "Rating") or [Text](https://schema.org/Text "Text") | Official rating of a piece of content—for example, 'MPAA PG-13'. |
| ``` contentReferenceTime ``` | [DateTime](https://schema.org/DateTime "DateTime") | The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event. |
| ``` contributor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A secondary contributor to the CreativeWork or Event. |
| ``` copyrightHolder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The party holding the legal copyright to the CreativeWork. |
| ``` copyrightNotice ``` | [Text](https://schema.org/Text "Text") | Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work. |
| ``` copyrightYear ``` | [Number](https://schema.org/Number "Number") | The year during which the claimed copyright for the CreativeWork was first asserted. |
| ``` correction ``` | [CorrectionComment](https://schema.org/CorrectionComment "CorrectionComment") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Indicates a correction to a [CreativeWork](https://schema.org/CreativeWork), either via a [CorrectionComment](https://schema.org/CorrectionComment), textually or in another document. |
| ``` countryOfOrigin ``` | [Country](https://schema.org/Country "Country") | The country of origin of something, including products as well as creative works such as movie and TV content. In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of [CreativeWork](https://schema.org/CreativeWork) it is difficult to provide fully general guidance, and properties such as [contentLocation](https://schema.org/contentLocation) and [locationCreated](https://schema.org/locationCreated) may be more applicable. In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here. |
| ``` creativeWorkStatus ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle. |
| ``` creator ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork. |
| ``` creditText ``` | [Text](https://schema.org/Text "Text") | Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work. |
| ``` dateCreated ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date on which the CreativeWork was created or the item was added to a DataFeed. |
| ``` dateModified ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed. |
| ``` datePublished ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | Date of first publication or broadcast. For example the date a [CreativeWork](https://schema.org/CreativeWork) was broadcast or a [Certification](https://schema.org/Certification) was issued. |
| ``` digitalSourceType ``` | [IPTCDigitalSourceEnumeration](https://schema.org/IPTCDigitalSourceEnumeration "IPTCDigitalSourceEnumeration") | Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some [CreativeWork](https://schema.org/CreativeWork). |
| ``` discussionUrl ``` | [URL](https://schema.org/URL "URL") | A link to the page containing the comments of the CreativeWork. |
| ``` editEIDR ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | An [EIDR](https://eidr.org/) (Entertainment Identifier Registry) [identifier](https://schema.org/identifier) representing a specific edit / edition for a work of film or television. For example, the motion picture known as "Ghostbusters" whose [titleEIDR](https://schema.org/titleEIDR) is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3". Since schema.org types like [Movie](https://schema.org/Movie) and [TVEpisode](https://schema.org/TVEpisode) can be used for both works and their multiple expressions, it is possible to use [titleEIDR](https://schema.org/titleEIDR) alone (for a general description), or alongside [editEIDR](https://schema.org/editEIDR) for a more edit-specific description. |
| ``` editor ``` | [Person](https://schema.org/Person "Person") | Specifies the Person who edited the CreativeWork. |
| ``` educationalAlignment ``` | [AlignmentObject](https://schema.org/AlignmentObject "AlignmentObject") | An alignment to an established educational framework. This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource [teaches](https://schema.org/teaches) or [assesses](https://schema.org/assesses) a competency. |
| ``` educationalLevel ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators. |
| ``` educationalUse ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The purpose of a work in the context of education; for example, 'assignment', 'group work'. |
| ``` encoding ``` | [MediaObject](https://schema.org/MediaObject "MediaObject") | A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes [encodings](https://schema.org/encodings "encodings"). Inverse property: [encodesCreativeWork](https://schema.org/encodesCreativeWork "encodesCreativeWork") |
| ``` encodingFormat ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Media type typically expressed using a MIME format (see [IANA site](http://www.iana.org/assignments/media-types/media-types.xhtml) and [MDN reference](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/MIME_types)), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc. In cases where a [CreativeWork](https://schema.org/CreativeWork) has several media type representations, [encoding](https://schema.org/encoding) can be used to indicate each [MediaObject](https://schema.org/MediaObject) alongside particular [encodingFormat](https://schema.org/encodingFormat) information. Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes [fileFormat](https://schema.org/fileFormat "fileFormat"). |
| ``` exampleOfWork ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A creative work that this work is an example/instance/realization/derivation of. Inverse property: [workExample](https://schema.org/workExample "workExample") |
| ``` expires ``` | [Date](https://schema.org/Date "Date") or [DateTime](https://schema.org/DateTime "DateTime") | Date the content expires and is no longer useful or available. For example a [VideoObject](https://schema.org/VideoObject) or [NewsArticle](https://schema.org/NewsArticle) whose availability or relevance is time-limited, a [ClaimReview](https://schema.org/ClaimReview) fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a [Certification](https://schema.org/Certification) the validity has expired. |
| ``` funder ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports (sponsors) something through some kind of financial contribution. |
| ``` funding ``` | [Grant](https://schema.org/Grant "Grant") | A [Grant](https://schema.org/Grant) that directly or indirectly provide funding or sponsorship for this item. See also [ownershipFundingInfo](https://schema.org/ownershipFundingInfo). Inverse property: [fundedItem](https://schema.org/fundedItem "fundedItem") |
| ``` genre ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Genre of the creative work, broadcast channel or group. |
| ``` hasPart ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense). Inverse property: [isPartOf](https://schema.org/isPartOf "isPartOf") |
| ``` headline ``` | [Text](https://schema.org/Text "Text") | Headline of the article. |
| ``` inLanguage ``` | [Language](https://schema.org/Language "Language") or [Text](https://schema.org/Text "Text") | The language of the content or performance or used in an action. Please use one of the language codes from the [IETF BCP 47 standard](http://tools.ietf.org/html/bcp47). See also [availableLanguage](https://schema.org/availableLanguage). Supersedes [language](https://schema.org/language "language"). |
| ``` interactionStatistic ``` | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes [interactionCount](https://schema.org/interactionCount "interactionCount"). |
| ``` interactivityType ``` | [Text](https://schema.org/Text "Text") | The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'. |
| ``` interpretedAsClaim ``` | [Claim](https://schema.org/Claim "Claim") | Used to indicate a specific claim contained, implied, translated or refined from the content of a [MediaObject](https://schema.org/MediaObject) or other [CreativeWork](https://schema.org/CreativeWork). The interpreting party can be indicated using [claimInterpreter](https://schema.org/claimInterpreter). |
| ``` isAccessibleForFree ``` | [Boolean](https://schema.org/Boolean "Boolean") | A flag to signal that the item, event, or place is accessible for free. Supersedes [free](https://schema.org/free "free"). |
| ``` isBasedOn ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [Product](https://schema.org/Product "Product") or [URL](https://schema.org/URL "URL") | A resource from which this work is derived or from which it is a modification or adaptation. Supersedes [isBasedOnUrl](https://schema.org/isBasedOnUrl "isBasedOnUrl"). |
| ``` isFamilyFriendly ``` | [Boolean](https://schema.org/Boolean "Boolean") | Indicates whether this content is family friendly. |
| ``` isPartOf ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of. Inverse property: [hasPart](https://schema.org/hasPart "hasPart") |
| ``` keywords ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property. |
| ``` learningResourceType ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'. |
| ``` license ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | A license document that applies to this content, typically indicated by URL. |
| ``` locationCreated ``` | [Place](https://schema.org/Place "Place") | The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork. |
| ``` mainEntity ``` | [Thing](https://schema.org/Thing "Thing") | Indicates the primary entity described in some page or other CreativeWork. Inverse property: [mainEntityOfPage](https://schema.org/mainEntityOfPage "mainEntityOfPage") |
| ``` maintainer ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A maintainer of a [Dataset](https://schema.org/Dataset), software package ([SoftwareApplication](https://schema.org/SoftwareApplication)), or other [Project](https://schema.org/Project). A maintainer is a [Person](https://schema.org/Person) or [Organization](https://schema.org/Organization) that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When [maintainer](https://schema.org/maintainer) is applied to a specific version of something e.g. a particular version or packaging of a [Dataset](https://schema.org/Dataset), it is always possible that the upstream source has a different maintainer. The [isBasedOn](https://schema.org/isBasedOn) property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work. |
| ``` material ``` | [Product](https://schema.org/Product "Product") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | A material that something is made from, e.g. leather, wool, cotton, paper. |
| ``` materialExtent ``` | [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") or [Text](https://schema.org/Text "Text") | The quantity of the materials being described or an expression of the physical space they occupy. |
| ``` mentions ``` | [Thing](https://schema.org/Thing "Thing") | Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept. |
| ``` offers ``` | [Demand](https://schema.org/Demand "Demand") or [Offer](https://schema.org/Offer "Offer") | An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use [businessFunction](https://schema.org/businessFunction) to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a [Demand](https://schema.org/Demand). While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: [itemOffered](https://schema.org/itemOffered "itemOffered") |
| ``` pattern ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported. |
| ``` position ``` | [Integer](https://schema.org/Integer "Integer") or [Text](https://schema.org/Text "Text") | The position of an item in a series or sequence of items. |
| ``` producer ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.). |
| ``` provider ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes [carrier](https://schema.org/carrier "carrier"). |
| ``` publication ``` | [PublicationEvent](https://schema.org/PublicationEvent "PublicationEvent") | A publication event associated with the item. |
| ``` publisher ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | The publisher of the article in question. |
| ``` publisherImprint ``` | [Organization](https://schema.org/Organization "Organization") | The publishing division which published the comic. |
| ``` publishingPrinciples ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The publishingPrinciples property indicates (typically via [URL](https://schema.org/URL)) a document describing the editorial principles of an [Organization](https://schema.org/Organization) (or individual, e.g. a [Person](https://schema.org/Person) writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a [CreativeWork](https://schema.org/CreativeWork) (e.g. [NewsArticle](https://schema.org/NewsArticle)) the principles are those of the party primarily responsible for the creation of the [CreativeWork](https://schema.org/CreativeWork). While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a [funder](https://schema.org/funder)) can be expressed using schema.org terminology. |
| ``` recordedAt ``` | [Event](https://schema.org/Event "Event") | The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event. Inverse property: [recordedIn](https://schema.org/recordedIn "recordedIn") |
| ``` releasedEvent ``` | [PublicationEvent](https://schema.org/PublicationEvent "PublicationEvent") | The place and time the release was issued, expressed as a PublicationEvent. |
| ``` review ``` | [Review](https://schema.org/Review "Review") | A review of the item. Supersedes [reviews](https://schema.org/reviews "reviews"). |
| ``` schemaVersion ``` | [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. `10.0` as a simple string, or more explicitly via URL, `https://schema.org/docs/releases.html#v10.0`. There may be situations in which other schemas might usefully be referenced this way, e.g. `http://dublincore.org/specifications/dublin-core/dces/1999-07-02/` but this has not been carefully explored in the community. |
| ``` sdDatePublished ``` | [Date](https://schema.org/Date "Date") | Indicates the date on which the current structured data was generated / published. Typically used alongside [sdPublisher](https://schema.org/sdPublisher). |
| ``` sdLicense ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | A license document that applies to this structured data, typically indicated by URL. |
| ``` sdPublisher ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The [sdPublisher](https://schema.org/sdPublisher) property helps make such practices more explicit. |
| ``` size ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [QuantitativeValue](https://schema.org/QuantitativeValue "QuantitativeValue") or [SizeSpecification](https://schema.org/SizeSpecification "SizeSpecification") or [Text](https://schema.org/Text "Text") | A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured [SizeSpecification](https://schema.org/SizeSpecification); in other cases, the [width](https://schema.org/width), [height](https://schema.org/height), [depth](https://schema.org/depth) and [weight](https://schema.org/weight) properties may be more applicable. |
| ``` sourceOrganization ``` | [Organization](https://schema.org/Organization "Organization") | The Organization on whose behalf the creator was working. |
| ``` spatial ``` | [Place](https://schema.org/Place "Place") | The "spatial" property can be used in cases when more specific properties (e.g. [locationCreated](https://schema.org/locationCreated), [spatialCoverage](https://schema.org/spatialCoverage), [contentLocation](https://schema.org/contentLocation)) are not known to be appropriate. |
| ``` spatialCoverage ``` | [Place](https://schema.org/Place "Place") | The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York. |
| ``` sponsor ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event. |
| ``` teaches ``` | [DefinedTerm](https://schema.org/DefinedTerm "DefinedTerm") or [Text](https://schema.org/Text "Text") | The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term. |
| ``` temporal ``` | [DateTime](https://schema.org/DateTime "DateTime") or [Text](https://schema.org/Text "Text") | The "temporal" property can be used in cases where more specific properties (e.g. [temporalCoverage](https://schema.org/temporalCoverage), [dateCreated](https://schema.org/dateCreated), [dateModified](https://schema.org/dateModified), [datePublished](https://schema.org/datePublished)) are not known to be appropriate. |
| ``` temporalCoverage ``` | [DateTime](https://schema.org/DateTime "DateTime") or [Text](https://schema.org/Text "Text") or [URL](https://schema.org/URL "URL") | The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in [ISO 8601 time interval format](https://en.wikipedia.org/wiki/ISO_8601#Time_intervals). In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945". Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes [datasetTimeInterval](https://schema.org/datasetTimeInterval "datasetTimeInterval"). |
| ``` text ``` | [Text](https://schema.org/Text "Text") | The textual content of this CreativeWork. |
| ``` thumbnail ``` | [ImageObject](https://schema.org/ImageObject "ImageObject") | Thumbnail image for an image or video. |
| ``` thumbnailUrl ``` | [URL](https://schema.org/URL "URL") | A thumbnail image relevant to the Thing. |
| ``` timeRequired ``` | [Duration](https://schema.org/Duration "Duration") | Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience. |
| ``` translationOfWork ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | The work that this work has been translated from. E.g. 物种起源 is a translationOf “On the Origin of Species”. Inverse property: [workTranslation](https://schema.org/workTranslation "workTranslation") |
| ``` translator ``` | [Organization](https://schema.org/Organization "Organization") or [Person](https://schema.org/Person "Person") | Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event. |
| ``` typicalAgeRange ``` | [Text](https://schema.org/Text "Text") | The typical expected age range, e.g. '7-9', '11-'. |
| ``` usageInfo ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") or [URL](https://schema.org/URL "URL") | The schema.org [usageInfo](https://schema.org/usageInfo) property indicates further information about a [CreativeWork](https://schema.org/CreativeWork). This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options. This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses. |
| ``` version ``` | [Number](https://schema.org/Number "Number") or [Text](https://schema.org/Text "Text") | The version of the CreativeWork embodied by a specified resource. |
| ``` video ``` | [Clip](https://schema.org/Clip "Clip") or [VideoObject](https://schema.org/VideoObject "VideoObject") | An embedded video object. |
| ``` wordCount ``` | [Integer](https://schema.org/Integer "Integer") | The number of words in the text of the CreativeWork such as an Article, Book, etc. |
| ``` workExample ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book. Inverse property: [exampleOfWork](https://schema.org/exampleOfWork "exampleOfWork") |
| ``` workTranslation ``` | [CreativeWork](https://schema.org/CreativeWork "CreativeWork") | A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation “Journey to the West”, a German workTranslation “Monkeys Pilgerfahrt” and a Vietnamese translation Tây du ký bình khảo. Inverse property: [translationOfWork](https://schema.org/translationOfWork "translationOfWork") |
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

Instances of [WebSite](https://schema.org/WebSite "WebSite") may appear as a value for the following properties

| Property | On Types | Description |
| --- | --- | --- |
| [interactionService](https://schema.org/interactionService "interactionService") | [InteractionCounter](https://schema.org/InteractionCounter "InteractionCounter") | The WebSite or SoftwareApplication where the interactions took place. |

### Examples
```
    <script type="application/ld+json">
    {
        "@context": "https://schema.org",
        "@type": "WebSite",
        "url": "http://example.com/",
        "potentialAction": {
          "@type": "SearchAction",
          "target": "http://example.com/search?&q={query}",
          "query": "required"
        }
    }
    </script>
```Title: mentions - Schema.org Property

URL Source: https://schema.org/mentions

Markdown Content:
mentions - Schema.org Property

===============

**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details. 

[Schema.org](https://schema.org/)

*   [Docs](https://schema.org/docs/documents.html)
*   [Schemas](https://schema.org/docs/schemas.html)
*   [Validate](https://validator.schema.org/)
*   [About](https://schema.org/docs/about.html)

[×](javascript:void(0) "Clear search box")

[](javascript:void(0);)

mentions
========

A Schema.org Property

[Thing](https://schema.org/Thing "Thing")>[Property](https://schema.org/Property "Property") :: [mentions](https://schema.org/mentions "mentions")

**[more...]** 

- [x] 

*   Canonical URL: https://schema.org/mentions
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+mentions)

Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept.

### Values expected to be one of these types

```
Thing
```

### Used on these types

```
CreativeWork
```

[Terms and conditions](https://schema.org/docs/terms.html)

• Schema.org • V29.2 | 2025-05-15
Title: relatedLink - Schema.org Property

URL Source: https://schema.org/relatedLink

Markdown Content:
relatedLink - Schema.org Property

===============

**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details. 

[Schema.org](https://schema.org/)

*   [Docs](https://schema.org/docs/documents.html)
*   [Schemas](https://schema.org/docs/schemas.html)
*   [Validate](https://validator.schema.org/)
*   [About](https://schema.org/docs/about.html)

[×](javascript:void(0) "Clear search box")

[](javascript:void(0);)

relatedLink
===========

A Schema.org Property

[Thing](https://schema.org/Thing "Thing")>[Property](https://schema.org/Property "Property") :: [relatedLink](https://schema.org/relatedLink "relatedLink")

**[more...]** 

- [x] 

*   Canonical URL: https://schema.org/relatedLink
*   [Check for open issues.](https://github.com/schemaorg/schemaorg/issues?q=is%3Aissue+is%3Aopen+relatedLink)

A link related to this web page, for example to other related web pages.

### Values expected to be one of these types

```
URL
```

### Used on these types

```
WebPage
```

[Terms and conditions](https://schema.org/docs/terms.html)

• Schema.org • V29.2 | 2025-05-15
Title: significantLink - Schema.org Property

URL Source: https://schema.org/significantLink

Markdown Content:
**Note**: You are viewing the development version of [Schema.org](https://schema.org/). See [how we work](https://schema.org/docs/howwework.html) for more details.

A Schema.org Property

One of the more significant URLs on the page. Typically, these are the non-navigation links that are clicked on the most.

### Values expected to be one of these types

```
URL
```

| Supersedes |
| --- |
| ``` significantLinks ``` |
