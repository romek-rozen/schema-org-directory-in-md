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
```