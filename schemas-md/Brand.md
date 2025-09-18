Title: Brand - Schema.org Type

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
