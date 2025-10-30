# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a **Schema.org documentation repository** containing comprehensive Polish-language documentation for Schema.org structured data types used in SEO and web development. The repository serves as a reference guide for implementing JSON-LD structured data markup according to Schema.org standards.

## Repository Purpose

The repository provides:
- Detailed documentation for popular Schema.org types (Product, Organization, LocalBusiness, FAQPage, HowTo, Event, etc.)
- Practical JSON-LD implementation examples
- Guidelines for Google Rich Results optimization
- Polish-specific considerations (NIP, REGON, KRS identifiers, PLN currency, etc.)

## Project Structure

```
Schema_org/
├── schemas-md/              # Individual schema type documentation
│   ├── Product.md
│   ├── Organization.md
│   ├── LocalBusiness.md
│   ├── FAQPage.md
│   ├── HowTo.md
│   ├── Event.md
│   ├── Person.md
│   ├── Article.md
│   ├── WebPage.md
│   ├── WebSite.md
│   ├── Service.md
│   ├── ProfessionalService.md
│   ├── Brand.md
│   ├── Offer.md
│   ├── AggregateOffer.md
│   ├── CreativeWork.md
│   ├── mentions.md
│   ├── relatedLink.md
│   └── significantLink.md
├── master_prompt.md         # System prompt for JSON-LD generation
├── LISTA_STRON_SCHEMA.txt   # List of Schema.org URLs
└── README.md                # Main documentation
```

## Key Files

### `master_prompt.md`
This is the **core system prompt** that defines the logic for:
- **Schema type detection**: Automatic identification of appropriate Schema.org types based on content indicators
- **JSON-LD generation rules**: Templates and validation requirements for each schema type
- **Polish-specific mappings**: How to handle NIP, REGON, KRS, Polish addresses (addressCountry: "PL"), and PLN currency
- **Google Rich Results optimization**: Guidelines for creating schemas that work with Google's structured data features

When generating or validating JSON-LD schemas, always reference this file for:
- Type detection logic (lines 229-242)
- Required fields per type (line 246)
- Format requirements (dates, prices, URLs)
- Multi-type implementations
- Common mistakes to avoid

### `schemas-md/*.md`
Each file contains:
- Schema type definition (imported from schema.org)
- Property tables with expected types
- Practical JSON-LD examples
- Usage guidance

These files are primarily **reference documentation** scraped from Schema.org, formatted in Markdown.

### `README.md`
User-facing documentation that explains:
- How to choose the right schema type
- Implementation guidelines
- Testing procedures (Google Rich Results Test, Schema.org Validator)
- Best practices

## Working with JSON-LD Schemas

### Validation Requirements

When creating or validating JSON-LD schemas:

1. **Required fields** (always check):
   - `@context`: must be `"https://schema.org"`
   - `@type`: valid Schema.org type
   - `name`: required for most types

2. **Date formats**: ISO 8601 (YYYY-MM-DD or with time)

3. **Price formats**: Numbers without currency symbols (e.g., `"5999"` not `"5999 zł"`)

4. **URLs**: Full URLs with http/https protocol

5. **Polish specifics**:
   - Currency: `"priceCurrency": "PLN"`
   - Country: `"addressCountry": "PL"`
   - NIP: use `vatID` or `taxID`
   - REGON/KRS: use `identifier` with `PropertyValue`

### Schema Type Detection Logic

Reference `master_prompt.md` lines 229-242 for automatic type detection:
- Product: price, "zł", "PLN", availability, stock indicators
- FAQPage: "FAQ", questions, Q&A structure
- Event: dates, "konferencja", "warsztaty", event indicators
- HowTo: "krok po kroku", "instrukcja", "jak", tutorial patterns
- Organization: NIP, REGON, company data
- LocalBusiness: opening hours, physical location
- Service: "usługa", "świadczymy", "oferujemy"
- Person: biography, CV, job title
- WebPage: breadcrumbs, meta tags

### Common Schema Templates

Refer to `master_prompt.md` for complete templates:
- Basic schemas: lines 28-227
- Multi-type implementations: lines 271-299
- AggregateOffer example: lines 302-316
- Advanced features: lines 346-353

## Testing Structured Data

After implementing schemas, validate using:
1. **Google Rich Results Test**: https://search.google.com/test/rich-results
2. **Schema.org Validator**: https://validator.schema.org/
3. **Google Search Console**: "Ulepszenia" section

## Documentation Maintenance

When updating documentation:

1. **Consistency**: Ensure JSON-LD examples match the validation rules in `master_prompt.md`
2. **Polish context**: Always include Polish-specific examples (PLN prices, Polish addresses)
3. **Google compliance**: Verify schemas work with Google Rich Results
4. **Real data only**: Examples should use realistic data, not placeholder text

## Content Language

- **Documentation language**: Polish
- **Code/JSON**: English property names (Schema.org standard)
- **Comments**: Polish for user-facing docs, English for technical implementation

## No Build Process

This is a **documentation-only repository** with:
- No package.json
- No build scripts
- No test suite
- No compilation steps

All files are static Markdown documentation and can be edited directly.

## Git Workflow

- **Main branch**: `master`
- Clean working tree at conversation start
- Standard git workflow applies for commits and PRs

## Related Resources

- Official Schema.org: https://schema.org/
- Google Structured Data Guidelines: https://developers.google.com/search/docs/advanced/structured-data/intro-structured-data
- Rich Results Gallery: https://developers.google.com/search/docs/advanced/structured-data/search-gallery
