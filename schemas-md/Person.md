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
```