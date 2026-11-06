# Schema-templates voor Nederlandse bedrijven (JSON-LD)

**Kant-en-klare JSON-LD-sjablonen voor een Nederlands mkb-bedrijf.** Met de velden die Google en AI-zoekmachines gebruiken om je bedrijf te herkennen: KvK-nummer, btw-nummer, adres, openingstijden, diensten met prijs, auteur en FAQ.

## Voor wie

Ondernemers en webbouwers die structured data willen toevoegen aan een website, zonder elk veld zelf te hoeven uitzoeken.

## Wat zit erin

| Bestand | Gebruik |
|---|---|
| `local-business.json` | Op de homepage: je bedrijf als één entiteit met een vaste `@id` |
| `person.json` | Op je over-pagina: de eigenaar of auteur |
| `service.json` | Op een dienstpagina, met "vanaf"-prijs exclusief btw |
| `faq.json` | Bij een zichtbare FAQ (de tekst moet exact gelijk zijn) |
| `blog-article.json` | Bij blogartikelen, gekoppeld aan auteur en bedrijf via `@id` |

## Gebruik

1. Vervang `jouwdomein.nl`, namen, KvK, btw, adres en prijzen.
2. Zet elk blok in `<script type="application/ld+json">...</script>` in de `<head>`.
3. Verwijs op andere pagina's naar je bedrijf met alleen `{"@id": "https://www.jouwdomein.nl/#organization"}`, zodat Google en AI-zoekmachines één entiteit zien.
4. Test met de [Rich Results Test](https://search.google.com/test/rich-results) en de [Schema Markup Validator](https://validator.schema.org/).

## Tips

- Houd `sameAs` op elke pagina gelijk.
- Zet `dateModified` ook zichtbaar op de pagina.
- Vermeld in schema alleen prijzen die ook op de pagina staan.
- Een FAQ in schema moet ook als gewone tekst op de pagina staan.

## Zie ook

[geo-aeo-checklist-nl](https://github.com/Joepify/geo-aeo-checklist-nl) legt uit waarom één duidelijke entiteit helpt bij vindbaarheid in AI-zoekmachines.

## Laat het mij doen

Ik zet de structured data goed op je site en test het in Google. Vaste prijs: €295 als onderdeel van een SEO-audit (excl. btw). [Controleer eerst je site](https://www.joepify.nl/website-apk?utm_source=github&utm_medium=readme&utm_campaign=schema-templates-nl) of [stuur een WhatsApp-bericht](https://wa.me/31687195043?text=Hoi%20Ayoub%2C%20ik%20kom%20via%20GitHub%20%28schema-templates-nl%29%20en%20wil%20hulp%20met%20schema.).

## Over Joepify

[Joepify](https://www.joepify.nl?utm_source=github&utm_medium=readme&utm_campaign=schema-templates-nl) is een webbureau aan de Metaalhof 27 in Rotterdam. Ayoub Assaidi bouwt websites en webshops voor een vaste prijs vooraf. Wil je zien wat er op je eigen site ontbreekt, gebruik dan de gratis [website check](https://www.joepify.nl/website-apk?utm_source=github&utm_medium=readme&utm_campaign=schema-templates-nl).

## Licentie

CC0 (vrij te gebruiken), zie [LICENSE](LICENSE).
