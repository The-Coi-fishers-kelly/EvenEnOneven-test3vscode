# StartWebdesignOefening — herbruikbare startmap

## Doel

Volgens de oorspronkelijke README wordt dit project gebruikt als **basis om toekomstige webdesignoefeningen te klonen**. Het is dus een sjabloon, niet noodzakelijk een onvoltooide schooltaak. Daarom blijven `script.js` en `styles.css` bewust leeg.

## Overzicht per bestand

| Bestand | Wat doet het? |
| --- | --- |
| `index.html` | Toont een eenvoudige pagina met header, een hoofdgedeelte met tekst en knop, en een footer. Laadt de externe opmaakbibliotheek W3.CSS en de jQuery-bibliotheek. |
| `styles.css` | Een leeg CSS-bestand waarin je de standaardopmaak kan overschrijven of uitbreiden. |
| `script.js` | Een leeg JavaScript-bestand waarin je later interacties schrijft. |
| `README.md` | Documentatie voor iedereen die het sjabloon gebruikt. |

## Welke code doet wat?

### `index.html`
- `<!DOCTYPE html>`: verklaart dat de pagina moderne HTML gebruikt.
- `<html>`: bevat het volledige HTML-document.
- `<meta charset="UTF-8">`: zorgt dat bijzondere tekens goed worden weergegeven.
- `<meta name="viewport" ...>`: schaalt de pagina op mobiele schermen.
- `<link rel="stylesheet" href="https://www.w3schools.com/w3css/6/w3.css">`: haalt W3.CSS op. Dat is een verzameling bestaande opmaakklassen, zoals `w3-bar`, `w3-blue` en `w3-container`.
- `<link rel="stylesheet" href="styles.css">`: laadt je **eigen** opmaak. Omdat deze later wordt geladen, kunnen eigen regels de standaardbibliotheek overschrijven bij gelijke specificiteit.
- `<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.1/jquery.min.js"></script>`: laadt jQuery, waarmee je bijvoorbeeld eenvoudig elementen selecteert en klikgebeurtenissen programmeert.
- `<header>`, `<div>`, `<footer>`: maken de zichtbare pagina-inhoud.
- `<script src="script.js"></script>` helemaal onderaan: laadt je eigen JavaScript nadat de zichtbare HTML-elementen zijn aangemaakt.

### `styles.css`
Hier kan je bijvoorbeeld een aangepaste achtergrond, marges of een hover-effect toevoegen. Het bestand is nu leeg **omdat het een starttemplate is**.

### `script.js`
Hier kan je later een knopinteractie maken. De knop 'Learn More' heeft momenteel geen gekoppelde JavaScript-actie. Dat is niet automatisch een fout in een sjabloon.

## Zelf leren: mini-oefening
Voeg in `script.js` eens toe:

```javascript
$(".w3-button").on("click", function () {
    alert("Je hebt geklikt!");
});
```

Wat gebeurt er? `$(".w3-button")` selecteert de knop aan de hand van de CSS-klasse. `.on("click", ...)` koppelt een gebeurtenis aan die knop. De `alert()` toont een melding.

*Dit is een oefenvoorbeeld en is niet automatisch in het sjabloon opgenomen.*

## Wat is de status?
**Werkend als basisstructuur, niet als afgewerkte interactieve website.** Er is geen specifieke opdracht toegevoegd. Aan het oorspronkelijke HTML-, CSS- en JavaScript-gedrag werd niets gewijzigd.

## Controle
De bestanden zijn gelezen en de verwijzingen zijn gecontroleerd op basis van de tekst. Er is geen browser- of netwerkuitvoering getest. W3.CSS en jQuery hebben een werkende internetverbinding nodig.
