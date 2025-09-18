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
```