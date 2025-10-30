Title: Article

URL Source: http://developers.google.com/search/docs/appearance/structured-data/article?hl=en

# Article
A Schema.org Type: Thing > CreativeWork > Article

Adding `Article` structured data to your news, blog, and sports article pages can help Google understand more about the web page and show better [title text](https://developers.google.com/search/docs/appearance/title-link), images, and [date information](https://developers.google.com/search/docs/appearance/publication-dates) for the article in search results on Google Search and other properties (for example, Google News and the [Google Assistant](https://developers.google.com/assistant/content/overview)). While there's no markup requirement to be eligible for Google News features like [Top stories](https://support.google.com/news/publisher-center/answer/9607026), you can add `Article` to more explicitly tell Google what your content is about (for example, that it's a news article, who the author is, or what the title of the article is).

## Best practices for author markup

To help Google best understand and represent the author of the content, we recommend following these best practices when specifying authors in markup:

| Best practices for author markup |
| --- |
| ### Include all authors in the markup | Make sure that all the authors that are presented as authors on the web page are also included in markup. |
| ### Specifying multiple authors | When specifying multiple authors, list each author in their own `author` field: "author": [ {"name": "Willow Lane"}, {"name": "Regula Felix"} ] Don't merge multiple authors in the same `author` field: "author": { "name": "Willow Lane, Regula Felix" } |
| ### Use additional fields | To help Google better understand who the author is, we strongly recommend using the `type` and `url` (or `sameAs`) properties. Use valid URLs for the `url` or `sameAs` properties. For example, if the author is a person, you could link to an author's page that provides more information about the author: "author": [ { "@type": "Person", "name": "Willow Lane", "url": "https://www.example.com/staff/willow_lane" } ] If the author is an organization, you could link to the organization's home page. "author": [ { "@type":"Organization", "name": "Some News Agency", "url": "https://www.example.com/" } ] |
| ### Only specify the author's name in the `author.name` property | In the `author.name` property, only specify the name of the author. Don't add any other piece of information. More specifically, don't add the following information: * The name of the publisher. Instead, use the `publisher` property. * The author's job title. Instead, use the appropriate property if you want to specify that information ([`jobTitle`](https://schema.org/jobTitle)). * Honorific prefix or suffix. Instead, use the appropriate property if you want to specify that information ([`honorificPrefix`](https://schema.org/honorificPrefix) or [`honorificSuffix`](https://schema.org/honorificSuffix)). * Introductory words (for example, don't include words like "posted by"). "author": [ { "@type": "Person", "name": "Echidna Jones", "honorificPrefix": "Dr", "jobTitle": "Editor in Chief" } ], "publisher": [ { "@type": "Organization", "name": "Bugs Daily" } ] } |
| ### Use the appropriate `Type` | Use the `Person` type for people, and the `Organization` type for organizations. Don't use the `Thing` type, and don't use the wrong type (for example, using the `Organization` type for a person). |

Here's an example that applies the author markup best practices:

"author":
 [
 {
 "@type": "Person",
 "name": "Willow Lane",
 "jobTitle": "Journalist",
 "url": "https://www.example.com/staff/willow-lane"
 },
 {
 "@type": "Person",
 "name": "Echidna Jones",
 "jobTitle": "Editor in Chief",
 "url": "https://www.example.com/staff/echidna-jones"
 }
 ],
"publisher":
 {
 "@type": "Organization",
 "name": "The Daily Bug",
 "url": "https://www.example.com"
 },
 // + Other fields related to the article...
}
Last updated 2025-10-14 UTC.

## Properties from Article

### articleBody
- **Type:** Text
- **Description:** The actual body of the article.

### articleSection
- **Type:** Text
- **Description:** Articles may belong to one or more 'sections' in a magazine or newspaper, such as Sports, Lifestyle, etc.

### backstory
- **Type:** CreativeWork or Text
- **Description:** For an Article, typically a NewsArticle, the backstory property provides a textual summary giving a brief explanation of why and how an article was created. In a journalistic setting this could include information about reporting process, methods, interviews, data sources, etc.

### pageEnd
- **Type:** Integer or Text
- **Description:** The page on which the work ends; for example "138" or "xvi".

### pageStart
- **Type:** Integer or Text
- **Description:** The page on which the work starts; for example "135" or "xiii".

### pagination
- **Type:** Text
- **Description:** Any description of pages that is not separated into pageStart and pageEnd; for example, "1-6, 9, 55" or "10-12, 46-49".

### speakable
- **Type:** SpeakableSpecification or URL
- **Description:** Indicates sections of a Web page that are particularly 'speakable' in the sense of being highlighted as being especially appropriate for text-to-speech conversion. Other sections of a page may also be usefully spoken in particular circumstances; the 'speakable' property serves to indicate the parts most likely to be generally useful for speech. The speakable property can be repeated an arbitrary number of times, with three kinds of possible 'content-locator' values: 1.) id-value URL references - uses id-value of an element in the page being annotated. The simplest use of speakable has (potentially relative) URL values, referencing identified sections of the document concerned. 2.) CSS Selectors - addresses content in the annotated page, e.g. via class attribute. Use the cssSelector property. 3.) XPaths - addresses content via XPaths (assuming an XML view of the content). Use the xpath property. For more sophisticated markup of speakable sections beyond simple ID references, either CSS selectors or XPath expressions to pick out document section(s) as speakable. For this we define a supporting type, SpeakableSpecification which is defined to be a possible value of the speakable property.

### wordCount
- **Type:** Integer
- **Description:** The number of words in the text of the CreativeWork such as an Article, Book, etc.

## Properties from CreativeWork

### about
- **Type:** Thing
- **Description:** The subject matter of the content. Inverse property: subjectOf

### abstract
- **Type:** Text
- **Description:** An abstract is a short description that summarizes a CreativeWork.

### accessMode
- **Type:** Text
- **Description:** The human sensory perceptual system or cognitive faculty through which a person may process or perceive information. Values should be drawn from the approved vocabulary.

### accessModeSufficient
- **Type:** ItemList
- **Description:** A list of single or combined accessModes that are sufficient to understand all the intellectual content of a resource. Values should be drawn from the approved vocabulary.

### accessibilityAPI
- **Type:** Text
- **Description:** Indicates that the resource is compatible with the referenced accessibility API. Values should be drawn from the approved vocabulary.

### accessibilityControl
- **Type:** Text
- **Description:** Identifies input methods that are sufficient to fully control the described resource. Values should be drawn from the approved vocabulary.

### accessibilityFeature
- **Type:** Text
- **Description:** Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility. Values should be drawn from the approved vocabulary.

### accessibilityHazard
- **Type:** Text
- **Description:** A characteristic of the described resource that is physiologically dangerous to some users. Related to WCAG 2.0 guideline 2.3. Values should be drawn from the approved vocabulary.

### accessibilitySummary
- **Type:** Text
- **Description:** A human-readable summary of specific accessibility features or deficiencies, consistent with the other accessibility metadata but expressing subtleties such as "short descriptions are present but long descriptions will be needed for non-visual users" or "short descriptions are present and no long descriptions are needed".

### accountablePerson
- **Type:** Person
- **Description:** Specifies the Person that is legally accountable for the CreativeWork.

### acquireLicensePage
- **Type:** CreativeWork or URL
- **Description:** Indicates a page documenting how licenses can be purchased or otherwise acquired, for the current item.

### aggregateRating
- **Type:** AggregateRating
- **Description:** The overall rating, based on a collection of reviews or ratings, of the item.

### alternativeHeadline
- **Type:** Text
- **Description:** A secondary title of the CreativeWork.

### archivedAt
- **Type:** URL or WebPage
- **Description:** Indicates a page or other link involved in archival of a CreativeWork. In the case of MediaReview, the items in a MediaReviewItem may often become inaccessible, but be archived by archival, journalistic, activist, or law enforcement organizations. In such cases, the referenced page may not directly publish the content.

### assesses
- **Type:** DefinedTerm or Text
- **Description:** The item being described is intended to assess the competency or learning outcome defined by the referenced term.

### associatedMedia
- **Type:** MediaObject
- **Description:** A media object that encodes this CreativeWork. This property is a synonym for encoding.

### audience
- **Type:** Audience
- **Description:** An intended audience, i.e. a group for whom something was created. Supersedes serviceAudience.

### audio
- **Type:** AudioObject or Clip or MusicRecording
- **Description:** An embedded audio object.

### author
- **Type:** Organization or Person
- **Description:** The author of this content or rating. Please note that author is special in that HTML 5 provides a special mechanism for indicating authorship via the rel tag. That is equivalent to this and may be used interchangeably.

### award
- **Type:** Text
- **Description:** An award won by or for this item. Supersedes awards.

### character
- **Type:** Person
- **Description:** Fictional person connected with a creative work.

### citation
- **Type:** CreativeWork or Text
- **Description:** A citation or reference to another creative work, such as another publication, web page, scholarly article, etc.

### comment
- **Type:** Comment
- **Description:** Comments, typically from users.

### commentCount
- **Type:** Integer
- **Description:** The number of comments this CreativeWork (e.g. Article, Question or Answer) has received. This is most applicable to works published in Web sites with commenting system; additional comments may exist elsewhere.

### conditionsOfAccess
- **Type:** Text
- **Description:** Conditions that affect the availability of, or method(s) of access to, an item. Typically used for real world items such as an ArchiveComponent held by an ArchiveOrganization. This property is not suitable for use as a general Web access control mechanism. It is expressed only in natural language. For example "Available by appointment from the Reading Room" or "Accessible only from logged-in accounts".

### contentLocation
- **Type:** Place
- **Description:** The location depicted or described in the content. For example, the location in a photograph or painting.

### contentRating
- **Type:** Rating or Text
- **Description:** Official rating of a piece of content—for example, 'MPAA PG-13'.

### contentReferenceTime
- **Type:** DateTime
- **Description:** The specific time described by a creative work, for works (e.g. articles, video objects etc.) that emphasise a particular moment within an Event.

### contributor
- **Type:** Organization or Person
- **Description:** A secondary contributor to the CreativeWork or Event.

### copyrightHolder
- **Type:** Organization or Person
- **Description:** The party holding the legal copyright to the CreativeWork.

### copyrightNotice
- **Type:** Text
- **Description:** Text of a notice appropriate for describing the copyright aspects of this Creative Work, ideally indicating the owner of the copyright for the Work.

### copyrightYear
- **Type:** Number
- **Description:** The year during which the claimed copyright for the CreativeWork was first asserted.

### correction
- **Type:** CorrectionComment or Text or URL
- **Description:** Indicates a correction to a CreativeWork, either via a CorrectionComment, textually or in another document.

### countryOfOrigin
- **Type:** Country
- **Description:** The country of origin of something, including products as well as creative works such as movie and TV content. In the case of TV and movie, this would be the country of the principle offices of the production company or individual responsible for the movie. For other kinds of CreativeWork it is difficult to provide fully general guidance, and properties such as contentLocation and locationCreated may be more applicable. In the case of products, the country of origin of the product. The exact interpretation of this may vary by context and product type, and cannot be fully enumerated here.

### creativeWorkStatus
- **Type:** DefinedTerm or Text
- **Description:** The status of a creative work in terms of its stage in a lifecycle. Example terms include Incomplete, Draft, Published, Obsolete. Some organizations define a set of terms for the stages of their publication lifecycle.

### creator
- **Type:** Organization or Person
- **Description:** The creator/author of this CreativeWork. This is the same as the Author property for CreativeWork.

### creditText
- **Type:** Text
- **Description:** Text that can be used to credit person(s) and/or organization(s) associated with a published Creative Work.

### dateCreated
- **Type:** Date or DateTime
- **Description:** The date on which the CreativeWork was created or the item was added to a DataFeed.

### dateModified
- **Type:** Date or DateTime
- **Description:** The date on which the CreativeWork was most recently modified or when the item's entry was modified within a DataFeed.

### datePublished
- **Type:** Date or DateTime
- **Description:** Date of first publication or broadcast. For example the date a CreativeWork was broadcast or a Certification was issued.

### digitalSourceType
- **Type:** IPTCDigitalSourceEnumeration
- **Description:** Indicates an IPTCDigitalSourceEnumeration code indicating the nature of the digital source(s) for some CreativeWork.

### discussionUrl
- **Type:** URL
- **Description:** A link to the page containing the comments of the CreativeWork.

### editEIDR
- **Type:** Text or URL
- **Description:** An EIDR (Entertainment Identifier Registry) identifier representing a specific edit / edition for a work of film or television. For example, the motion picture known as "Ghostbusters" whose titleEIDR is "10.5240/7EC7-228A-510A-053E-CBB8-J" has several edits, e.g. "10.5240/1F2A-E1C5-680A-14C6-E76B-I" and "10.5240/8A35-3BEE-6497-5D12-9E4F-3". Since schema.org types like Movie and TVEpisode can be used for both works and their multiple expressions, it is possible to use titleEIDR alone (for a general description), or alongside editEIDR for a more edit-specific description.

### editor
- **Type:** Person
- **Description:** Specifies the Person who edited the CreativeWork.

### educationalAlignment
- **Type:** AlignmentObject
- **Description:** An alignment to an established educational framework. This property should not be used where the nature of the alignment can be described using a simple property, for example to express that a resource teaches or assesses a competency.

### educationalLevel
- **Type:** DefinedTerm or Text or URL
- **Description:** The level in terms of progression through an educational or training context. Examples of educational levels include 'beginner', 'intermediate' or 'advanced', and formal sets of level indicators.

### educationalUse
- **Type:** DefinedTerm or Text
- **Description:** The purpose of a work in the context of education; for example, 'assignment', 'group work'.

### encoding
- **Type:** MediaObject
- **Description:** A media object that encodes this CreativeWork. This property is a synonym for associatedMedia. Supersedes encodings. Inverse property: encodesCreativeWork

### encodingFormat
- **Type:** Text or URL
- **Description:** Media type typically expressed using a MIME format (see IANA site and MDN reference), e.g. application/zip for a SoftwareApplication binary, audio/mpeg for .mp3 etc. In cases where a CreativeWork has several media type representations, encoding can be used to indicate each MediaObject alongside particular encodingFormat information. Unregistered or niche encoding and file formats can be indicated instead via the most appropriate URL, e.g. defining Web page or a Wikipedia/Wikidata entry. Supersedes fileFormat.

### exampleOfWork
- **Type:** CreativeWork
- **Description:** A creative work that this work is an example/instance/realization/derivation of. Inverse property: workExample

### expires
- **Type:** Date or DateTime
- **Description:** Date the content expires and is no longer useful or available. For example a VideoObject or NewsArticle whose availability or relevance is time-limited, a ClaimReview fact check whose publisher wants to indicate that it may no longer be relevant (or helpful to highlight) after some date, or a Certification the validity has expired.

### funder
- **Type:** Organization or Person
- **Description:** A person or organization that supports (sponsors) something through some kind of financial contribution.

### funding
- **Type:** Grant
- **Description:** A Grant that directly or indirectly provide funding or sponsorship for this item. See also ownershipFundingInfo. Inverse property: fundedItem

### genre
- **Type:** Text or URL
- **Description:** Genre of the creative work, broadcast channel or group.

### hasPart
- **Type:** CreativeWork
- **Description:** Indicates an item or CreativeWork that is part of this item, or CreativeWork (in some sense). Inverse property: isPartOf

### headline
- **Type:** Text
- **Description:** Headline of the article.

### inLanguage
- **Type:** Language or Text
- **Description:** The language of the content or performance or used in an action. Please use one of the language codes from the IETF BCP 47 standard. See also availableLanguage. Supersedes language.

### interactionStatistic
- **Type:** InteractionCounter
- **Description:** The number of interactions for the CreativeWork using the WebSite or SoftwareApplication. The most specific child type of InteractionCounter should be used. Supersedes interactionCount.

### interactivityType
- **Type:** Text
- **Description:** The predominant mode of learning supported by the learning resource. Acceptable values are 'active', 'expositive', or 'mixed'.

### interpretedAsClaim
- **Type:** Claim
- **Description:** Used to indicate a specific claim contained, implied, translated or refined from the content of a MediaObject or other CreativeWork. The interpreting party can be indicated using claimInterpreter.

### isAccessibleForFree
- **Type:** Boolean
- **Description:** A flag to signal that the item, event, or place is accessible for free. Supersedes free.

### isBasedOn
- **Type:** CreativeWork or Product or URL
- **Description:** A resource from which this work is derived or from which it is a modification or adaptation. Supersedes isBasedOnUrl.

### isFamilyFriendly
- **Type:** Boolean
- **Description:** Indicates whether this content is family friendly.

### isPartOf
- **Type:** CreativeWork or URL
- **Description:** Indicates an item or CreativeWork that this item, or CreativeWork (in some sense), is part of. Inverse property: hasPart

### keywords
- **Type:** DefinedTerm or Text or URL
- **Description:** Keywords or tags used to describe some item. Multiple textual entries in a keywords list are typically delimited by commas, or by repeating the property.

### learningResourceType
- **Type:** DefinedTerm or Text
- **Description:** The predominant type or kind characterizing the learning resource. For example, 'presentation', 'handout'.

### license
- **Type:** CreativeWork or URL
- **Description:** A license document that applies to this content, typically indicated by URL.

### locationCreated
- **Type:** Place
- **Description:** The location where the CreativeWork was created, which may not be the same as the location depicted in the CreativeWork.

### mainEntity
- **Type:** Thing
- **Description:** Indicates the primary entity described in some page or other CreativeWork. Inverse property: mainEntityOfPage

### maintainer
- **Type:** Organization or Person
- **Description:** A maintainer of a Dataset, software package (SoftwareApplication), or other Project. A maintainer is a Person or Organization that manages contributions to, and/or publication of, some (typically complex) artifact. It is common for distributions of software and data to be based on "upstream" sources. When maintainer is applied to a specific version of something e.g. a particular version or packaging of a Dataset, it is always possible that the upstream source has a different maintainer. The isBasedOn property can be used to indicate such relationships between datasets to make the different maintenance roles clear. Similarly in the case of software, a package may have dedicated maintainers working on integration into software distributions such as Ubuntu, as well as upstream maintainers of the underlying work.

### material
- **Type:** Product or Text or URL
- **Description:** A material that something is made from, e.g. leather, wool, cotton, paper.

### materialExtent
- **Type:** QuantitativeValue or Text
- **Description:** The quantity of the materials being described or an expression of the physical space they occupy.

### mentions
- **Type:** Thing
- **Description:** Indicates that the CreativeWork contains a reference to, but is not necessarily about a concept.

### offers
- **Type:** Demand or Offer
- **Description:** An offer to provide this item—for example, an offer to sell a product, rent the DVD of a movie, perform a service, or give away tickets to an event. Use businessFunction to indicate the kind of transaction offered, i.e. sell, lease, etc. This property can also be used to describe a Demand. While this property is listed as expected on a number of common types, it can be used in others. In that case, using a second type, such as Product or a subtype of Product, can clarify the nature of the offer. Inverse property: itemOffered

### pattern
- **Type:** DefinedTerm or Text
- **Description:** A pattern that something has, for example 'polka dot', 'striped', 'Canadian flag'. Values are typically expressed as text, although links to controlled value schemes are also supported.

### position
- **Type:** Integer or Text
- **Description:** The position of an item in a series or sequence of items.

### producer
- **Type:** Organization or Person
- **Description:** The person or organization who produced the work (e.g. music album, movie, TV/radio series etc.).

### provider
- **Type:** Organization or Person
- **Description:** The service provider, service operator, or service performer; the goods producer. Another party (a seller) may offer those services or goods on behalf of the provider. A provider may also serve as the seller. Supersedes carrier.

### publication
- **Type:** PublicationEvent
- **Description:** A publication event associated with the item.

### publisher
- **Type:** Organization or Person
- **Description:** The publisher of the article in question.

### publisherImprint
- **Type:** Organization
- **Description:** The publishing division which published the comic.

### publishingPrinciples
- **Type:** CreativeWork or URL
- **Description:** The publishingPrinciples property indicates (typically via URL) a document describing the editorial principles of an Organization (or individual, e.g. a Person writing a blog) that relate to their activities as a publisher, e.g. ethics or diversity policies. When applied to a CreativeWork (e.g. NewsArticle) the principles are those of the party primarily responsible for the creation of the CreativeWork. While such policies are most typically expressed in natural language, sometimes related information (e.g. indicating a funder) can be expressed using schema.org terminology.

### recordedAt
- **Type:** Event
- **Description:** The Event where the CreativeWork was recorded. The CreativeWork may capture all or part of the event. Inverse property: recordedIn

### releasedEvent
- **Type:** PublicationEvent
- **Description:** The place and time the release was issued, expressed as a PublicationEvent.

### review
- **Type:** Review
- **Description:** A review of the item. Supersedes reviews.

### schemaVersion
- **Type:** Text or URL
- **Description:** Indicates (by URL or string) a particular version of a schema used in some CreativeWork. This property was created primarily to indicate the use of a specific schema.org release, e.g. 10.0 as a simple string, or more explicitly via URL, https://schema.org/docs/releases.html#v10.0. There may be situations in which other schemas might usefully be referenced this way, e.g. http://dublincore.org/specifications/dublin-core/dces/1999-07-02/ but this has not been carefully explored in the community.

### sdDatePublished
- **Type:** Date
- **Description:** Indicates the date on which the current structured data was generated / published. Typically used alongside sdPublisher.

### sdLicense
- **Type:** CreativeWork or URL
- **Description:** A license document that applies to this structured data, typically indicated by URL.

### sdPublisher
- **Type:** Organization or Person
- **Description:** Indicates the party responsible for generating and publishing the current structured data markup, typically in cases where the structured data is derived automatically from existing published content but published on a different site. For example, student projects and open data initiatives often re-publish existing content with more explicitly structured metadata. The sdPublisher property helps make such practices more explicit.

### size
- **Type:** DefinedTerm or QuantitativeValue or SizeSpecification or Text
- **Description:** A standardized size of a product or creative work, specified either through a simple textual string (for example 'XL', '32Wx34L'), a QuantitativeValue with a unitCode, or a comprehensive and structured SizeSpecification; in other cases, the width, height, depth and weight properties may be more applicable.

### sourceOrganization
- **Type:** Organization
- **Description:** The Organization on whose behalf the creator was working.

### spatial
- **Type:** Place
- **Description:** The "spatial" property can be used in cases when more specific properties (e.g. locationCreated, spatialCoverage, contentLocation) are not known to be appropriate.

### spatialCoverage
- **Type:** Place
- **Description:** The spatialCoverage of a CreativeWork indicates the place(s) which are the focus of the content. It is a subproperty of contentLocation intended primarily for more technical and detailed materials. For example with a Dataset, it indicates areas that the dataset describes: a dataset of New York weather would have spatialCoverage which was the place: the state of New York.

### sponsor
- **Type:** Organization or Person
- **Description:** A person or organization that supports a thing through a pledge, promise, or financial contribution. E.g. a sponsor of a Medical Study or a corporate sponsor of an event.

### teaches
- **Type:** DefinedTerm or Text
- **Description:** The item being described is intended to help a person learn the competency or learning outcome defined by the referenced term.

### temporal
- **Type:** DateTime or Text
- **Description:** The "temporal" property can be used in cases where more specific properties (e.g. temporalCoverage, dateCreated, dateModified, datePublished) are not known to be appropriate.

### temporalCoverage
- **Type:** DateTime or Text or URL
- **Description:** The temporalCoverage of a CreativeWork indicates the period that the content applies to, i.e. that it describes, either as a DateTime or as a textual string indicating a time period in ISO 8601 time interval format. In the case of a Dataset it will typically indicate the relevant time period in a precise notation (e.g. for a 2011 census dataset, the year 2011 would be written "2011/2012"). Other forms of content, e.g. ScholarlyArticle, Book, TVSeries or TVEpisode, may indicate their temporalCoverage in broader terms - textually or via well-known URL. Written works such as books may sometimes have precise temporal coverage too, e.g. a work set in 1939 - 1945 can be indicated in ISO 8601 interval format format via "1939/1945". Open-ended date ranges can be written with ".." in place of the end date. For example, "2015-11/.." indicates a range beginning in November 2015 and with no specified final date. This is tentative and might be updated in future when ISO 8601 is officially updated. Supersedes datasetTimeInterval.

### text
- **Type:** Text
- **Description:** The textual content of this CreativeWork.

### thumbnail
- **Type:** ImageObject
- **Description:** Thumbnail image for an image or video.

### thumbnailUrl
- **Type:** URL
- **Description:** A thumbnail image relevant to the Thing.

### timeRequired
- **Type:** Duration
- **Description:** Approximate or typical time it usually takes to work with or through the content of this work for the typical or target audience.

### translationOfWork
- **Type:** CreativeWork
- **Description:** The work that this work has been translated from. E.g. 物种起源 is a translationOf "On the Origin of Species". Inverse property: workTranslation

### translator
- **Type:** Organization or Person
- **Description:** Organization or person who adapts a creative work to different languages, regional differences and technical requirements of a target market, or that translates during some event.

### typicalAgeRange
- **Type:** Text
- **Description:** The typical expected age range, e.g. '7-9', '11-'.

### usageInfo
- **Type:** CreativeWork or URL
- **Description:** The schema.org usageInfo property indicates further information about a CreativeWork. This property is applicable both to works that are freely available and to those that require payment or other transactions. It can reference additional information, e.g. community expectations on preferred linking and citation conventions, as well as purchasing details. For something that can be commercially licensed, usageInfo can provide detailed, resource-specific information about licensing options. This property can be used alongside the license property which indicates license(s) applicable to some piece of content. The usageInfo property can provide information about other licensing options, e.g. acquiring commercial usage rights for an image that is also available under non-commercial creative commons licenses.

### version
- **Type:** Number or Text
- **Description:** The version of the CreativeWork embodied by a specified resource.

### video
- **Type:** Clip or VideoObject
- **Description:** An embedded video object.

### workExample
- **Type:** CreativeWork
- **Description:** Example/instance/realization/derivation of the concept of this creative work. E.g. the paperback edition, first edition, or e-book. Inverse property: exampleOfWork

### workTranslation
- **Type:** CreativeWork
- **Description:** A work that is a translation of the content of this work. E.g. 西遊記 has an English workTranslation "Journey to the West", a German workTranslation "Monkeys Pilgerfahrt" and a Vietnamese translation Tây du ký bình khảo. Inverse property: translationOfWork

## Properties from Thing

### additionalType
- **Type:** Text or URL
- **Description:** An additional type for the item, typically used for adding more specific types from external vocabularies in microdata syntax. This is a relationship between something and a class that the thing is in. Typically the value is a URI-identified RDF class, and in this case corresponds to the use of rdf:type in RDF. Text values can be used sparingly, for cases where useful information can be added without their being an appropriate schema to reference. In the case of text values, the class label should follow the schema.org style guide.

### alternateName
- **Type:** Text
- **Description:** An alias for the item.

### description
- **Type:** Text or TextObject
- **Description:** A description of the item.

### disambiguatingDescription
- **Type:** Text
- **Description:** A sub property of description. A short description of the item used to disambiguate from other, similar items. Information from other properties (in particular, name) may be necessary for the description to be useful for disambiguation.

### identifier
- **Type:** PropertyValue or Text or URL
- **Description:** The identifier property represents any kind of identifier for any kind of Thing, such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See background notes for more details.

### image
- **Type:** ImageObject or URL
- **Description:** An image of the item. This can be a URL or a fully described ImageObject.

### mainEntityOfPage
- **Type:** CreativeWork or URL
- **Description:** Indicates a page (or other CreativeWork) for which this thing is the main entity being described. See background notes for details. Inverse property: mainEntity

### name
- **Type:** Text
- **Description:** The name of the item.

### potentialAction
- **Type:** Action
- **Description:** Indicates a potential Action, which describes an idealized action in which this thing would play an 'object' role.

### sameAs
- **Type:** URL
- **Description:** URL of a reference Web page that unambiguously indicates the item's identity. E.g. the URL of the item's Wikipedia page, Wikidata entry, or official website.

### subjectOf
- **Type:** CreativeWork or Event
- **Description:** A CreativeWork or Event about this Thing. Inverse property: about

### url
- **Type:** URL
- **Description:** URL of the item.

## Recommended properties

| Recommended properties |
| --- |
| `author` | `Person` or `Organization` The author of the article. To help Google best understand authors across various features, we recommend following the [author markup best practices](http://developers.google.com/search/docs/appearance/structured-data/article?hl=en#author-bp). |
| `author.name` | `Text` The name of the author. |
| `author.url` | `URL` A link to a web page that uniquely identifies the author of the article. For example, the author's social media page, an "about me" page, or a bio page. If the URL is an internal profile page, we recommend marking up that author using [profile page structured data](https://developers.google.com/search/docs/appearance/structured-data/profile-page). |
| `dateModified` | `DateTime` The date and time the article was most recently modified, in [ISO 8601 format](https://wikipedia.org/wiki/ISO_8601). We recommend that you provide timezone information; otherwise, we will default to [the timezone used by Googlebot](https://developers.google.com/search/docs/crawling-indexing/googlebot#timezone). Add the `dateModified` property if you want to provide more accurate date information to Google. The [Rich Results Test](https://search.google.com/test/rich-results) doesn't show a warning for this property, as it's only recommended if you decide that it's applicable to your site. |
| `datePublished` | `DateTime` The date and time the article was first published, in [ISO 8601 format](https://wikipedia.org/wiki/ISO_8601). We recommend that you provide timezone information; otherwise, we will default to [the timezone used by Googlebot](https://developers.google.com/search/docs/crawling-indexing/googlebot#timezone). Add the `datePublished` property if you want to provide more accurate date information to Google. The [Rich Results Test](https://search.google.com/test/rich-results) doesn't show a warning for this property, as it's only recommended if you decide that it's applicable to your site. |
| `headline` | `Text` The title of the article. Consider using a concise title, as long titles may be truncated on some devices. |
| `image` | Repeated `ImageObject` or `URL` The URL to an image that is representative of the article. Use images that are relevant to the article, rather than logos or captions. Additional image guidelines: * Image URLs must be crawlable and indexable. To check if Google can access your URLs, use the [URL Inspection tool](https://support.google.com/webmasters/answer/9012289). * Images must represent the marked up content. * Images must be in a file format that's [supported by Google Images](https://developers.google.com/search/docs/appearance/google-images#supported-image-formats). * For best results, we recommend providing multiple high-resolution images (minimum of 50K pixels when multiplying width and height) with the following aspect ratios: 16x9, 4x3, and 1x1. For example: "image": [ "https://example.com/photos/1x1/photo.jpg", "https://example.com/photos/4x3/photo.jpg", "https://example.com/photos/16x9/photo.jpg" ] |

## Examples

### Example 1

``` json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Article",
      "author": "John Doe",
      "interactionStatistic": [
        {
          "@type": "InteractionCounter",
          "interactionService": {
            "@type": "WebSite",
            "name": "Twitter",
            "url": "http://www.twitter.com"
          },
          "interactionType": "https://schema.org/ShareAction",
          "userInteractionCount": "1203"
        },
        {
          "@type": "InteractionCounter",
          "interactionType": "https://schema.org/CommentAction",
          "userInteractionCount": "78"
        }
      ],
      "name": "How to Tie a Reef Knot"
    }
    </script>
```

### Example 2

``` json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org/",
      "@type": "Article",
      "name": "Apple announces iPhone SE",
      "description": "New iPhone announced at 11:30 in California.",
      "about": {
        "@type": "Event",
        "name": "Apple's March 21 Announcements"
      },
      "contentReferenceTime": "2016-03-21T11:30:00-07:00"
    }
    </script>
```

### Example 3

``` json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "Periodical",
      "issn": "0140-6736",
      "hasPart": {
        "@id": "vol376",
        "@type": "PublicationVolume",
        "volumeNumber": "376",
        "hasPart": [
          {
            "@id": "issue9735",
            "@type": "PublicationIssue",
            "datePublished": "2010-07-03",
            "pageEnd": "140",
            "pageStart": "69",
            "issueNumber": "9735"
          },
          {
            "@id": "issue9734",
            "@type": "PublicationIssue",
            "datePublished": "2010-07-03",
            "pageEnd": "68",
            "pageStart": "1",
            "issueNumber": "9734"
          }
        ]
      },
      "name": "The Lancet",
      "publisher": "Elsevier"
    }
    </script>
```

### Example 4

``` json
    <script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@graph": [
        {
            "@id": "#issue",
            "@type": "PublicationIssue",
            "issueNumber": "5",
            "datePublished": "2012",
            "isPartOf": {
                "@id": "#periodical",
                "@type": [
                    "PublicationVolume",
                    "Periodical"
                ],
                "name": "Cataloging & Classification Quarterly",
                "issn": [
                    "1544-4554",
                    "0163-9374"
                ],
                "volumeNumber": "50",
                "publisher": "Taylor & Francis Group"
            }
        },
        {
            "@type": "ScholarlyArticle",
            "isPartOf": "#issue",
            "description": "The library catalog as a catalog of works was an infectious idea, which together with research led to reconceptualization in the form of the FRBR conceptual model. Two categories of lacunae emerge--the expression entity, and gaps in the model such as aggregates and dynamic documents. Evidence needed to extend the FRBR model is available in contemporary research on instantiation. The challenge for the bibliographic community is to begin to think of FRBR as a form of knowledge organization system, adding a final dimension to classification. The articles in the present special issue offer a compendium of the promise of the FRBR model.",
            "sameAs": "https://doi.org/10.1080/01639374.2012.682254",
            "about": [
                "Works",
                "Catalog"
            ],
            "pageEnd": "368",
            "pageStart": "360",
            "name": "Be Careful What You Wish For: FRBR, Some Lacunae, A Review",
            "author": "Smiraglia, Richard P."
        }
      ]
    }
    </script>
```

### Example 5

``` json
<script type="application/ld+json">
    {
      "@context": "https://schema.org",
      "@type": "NewsArticle",
      "headline": "Title of a News Article",
      "image": [
        "https://example.com/photos/1x1/photo.jpg",
        "https://example.com/photos/4x3/photo.jpg",
        "https://example.com/photos/16x9/photo.jpg"
       ],
      "datePublished": "2024-01-05T08:00:00+08:00",
      "dateModified": "2024-02-05T09:20:00+08:00",
      "author": [{
          "@type": "Person",
          "name": "Jane Doe",
          "url": "https://example.com/profile/janedoe123"
        },{
          "@type": "Person",
          "name": "John Doe",
          "url": "https://example.com/profile/johndoe123"
      }]
    }
    </script>
```
