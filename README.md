# Dokumentacja Schematów Schema.org

## Opis projektu

To repozytorium zawiera kompleksową dokumentację najpopularniejszych typów schematów Schema.org używanych w SEO i strukturalizowanych danych. Każdy plik zawiera szczegółowy opis typu schematu, jego zastosowania, wymagane i opcjonalne właściwości oraz praktyczne przykłady implementacji.

## Struktura projektu

```bash
Schema_org/
│
├── schemas-md/           # Katalog z dokumentacją poszczególnych schematów
│   ├── AggregateOffer.md
│   ├── Brand.md
│   ├── CreativeWork.md
│   ├── Event.md
│   ├── FAQPage.md
│   ├── HowTo.md
│   ├── LocalBusiness.md
│   ├── Offer.md
│   ├── Organization.md
│   ├── Person.md
│   ├── Product.md
│   ├── ProfessionalService.md
│   ├── Service.md
│   ├── WebPage.md
│   ├── WebSite.md
│   ├── mentions.md
│   ├── relatedLink.md
│   └── significantLink.md
│
├── LISTA_STRON_SCHEMA.txt  # Lista stron ze schematami do analizy
└── master_prompt.md        # Główny dokument z instrukcjami
```

## Jak korzystać z dokumentacji

### 1. Wybór odpowiedniego schematu

Każdy plik w katalogu `schemas-md/` opisuje konkretny typ schematu:

- **Product.md** - dla stron produktowych e-commerce
- **LocalBusiness.md** / **ProfessionalService.md** - dla firm lokalnych i usług
- **Organization.md** - dla stron firmowych
- **Person.md** - dla profili osobowych
- **FAQPage.md** - dla sekcji FAQ
- **HowTo.md** - dla instrukcji i poradników
- **Event.md** - dla wydarzeń
- **WebPage.md** / **WebSite.md** - dla ogólnych stron internetowych

### 2. Struktura dokumentacji każdego schematu

Każdy plik zawiera:
- **Opis typu** - czym jest dany schemat i kiedy go używać
- **Najważniejsze właściwości** - lista kluczowych pól
- **Przykłady użycia** - praktyczne implementacje w JSON-LD
- **Wskazówki** - najlepsze praktyki i pułapki do uniknięcia
- **Relacje z innymi typami** - jak łączyć schematy

### 3. Implementacja schematów

#### Podstawowy przykład implementacji (JSON-LD):

```html
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Product",
  "name": "Nazwa produktu",
  "description": "Opis produktu",
  "image": "https://example.com/product.jpg",
  "offers": {
    "@type": "Offer",
    "price": "99.99",
    "priceCurrency": "PLN",
    "availability": "https://schema.org/InStock"
  }
}
</script>
```

### 4. Testowanie schematów

Po implementacji schematów należy je przetestować używając:

1. **Google Rich Results Test**: https://search.google.com/test/rich-results
2. **Schema.org Validator**: https://validator.schema.org/
3. **Google Search Console** - sekcja "Ulepszenia"

## Najlepsze praktyki

1. **Używaj tylko prawdziwych danych** - nie wypełniaj schematów fikcyjnymi informacjami
2. **Bądź kompletny** - uzupełnij wszystkie wymagane pola
3. **Zachowaj spójność** - dane w schemacie muszą odpowiadać treści na stronie
4. **Testuj regularnie** - sprawdzaj poprawność schematów po każdej zmianie
5. **Śledź wyniki** - monitoruj w Google Search Console jak schematy wpływają na wyświetlanie

## Przydatne linki

- [Oficjalna dokumentacja Schema.org](https://schema.org/)
- [Google Structured Data Guidelines](https://developers.google.com/search/docs/advanced/structured-data/intro-structured-data)
- [Rich Results Gallery](https://developers.google.com/search/docs/advanced/structured-data/search-gallery)

## Wsparcie

W razie pytań dotyczących implementacji schematów Schema.org, zajrzyj do odpowiedniego pliku w katalogu `schemas-md/` lub skonsultuj się z oficjalną dokumentacją Schema.org.

## Licencja

Dokumentacja jest udostępniona w celach edukacyjnych. Schematy Schema.org są standardem otwartym zarządzanym przez społeczność.

---

*Ostatnia aktualizacja: Styczeń 2025*
