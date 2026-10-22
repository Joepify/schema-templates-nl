# Schema-templates voor Nederlandse bedrijven (JSON-LD)

Kant-en-klare JSON-LD-sjablonen voor een Nederlands mkb-bedrijf, met de velden die Google en AI-zoekmachines gebruiken om je bedrijf te herkennen: KvK-nummer, btw-nummer, adres, openingstijden, diensten met prijs, auteur en FAQ.

| Bestand | Gebruik |
|---|---|
| `local-business.json` | Op de homepage: je bedrijf als één entiteit met vaste `@id` |
| `person.json` | Op je over-pagina: de eigenaar of auteur |
| `service.json` | Op een dienstpagina, met "vanaf"-prijs exclusief btw |
| `faq.json` | Bij een zichtbare FAQ (tekst moet exact gelijk zijn) |
| `blog-article.json` | Bij blogartikelen, gekoppeld aan auteur en bedrijf via `@id` |

## Gebruik
1. Vervang `jouwdomein.nl`, namen, KvK, btw, adres en prijzen.
2. Zet elk blok in `<script type="application/ld+json">…</script>` in de `<head>`.
3. Verwijs op andere pagina's naar je bedrijf met alleen `{"@id": "https://www.jouwdomein.nl/#organization"}`, zodat Google en AI één entiteit zien.
4. Test met de [Rich Results Test](https://search.google.com/test/rich-results) en de [Schema Markup Validator](https://validator.schema.org/).

Tips: houd `sameAs` op elke pagina gelijk; zet `dateModified` ook zichtbaar op de pagina; vermeld alleen prijzen die ook op de pagina staan.

Gemaakt door [Joepify](https://www.joepify.nl), Rotterdam. Zie ook [geo-aeo-checklist-nl](https://github.com/Joepify/geo-aeo-checklist-nl). Licentie: CC0 (vrij te gebruiken).
