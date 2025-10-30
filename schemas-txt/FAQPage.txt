# Title: FAQPage

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
