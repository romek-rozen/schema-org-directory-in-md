Title: Product - Schema.org Type

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
