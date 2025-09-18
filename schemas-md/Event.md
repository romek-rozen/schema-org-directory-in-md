Title: Event - Schema.org Type

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
```