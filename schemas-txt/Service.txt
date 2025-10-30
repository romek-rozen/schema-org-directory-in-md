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
```