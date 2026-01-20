# Plankie

Een interactieve, web-based tool voor het visueel indelen van tijdschriften en magazines. Deze applicatie draait volledig in de browser en maakt het mogelijk om via 'drag & drop' snel een bladformule neer te zetten, pagina's te schuiven en de voortgang te bewaken.

De tool is ontworpen om direct bruikbaar te zijn zonder installatie van zware software of databases. Alle data wordt lokaal in de browser opgeslagen, waardoor je privacy gewaarborgd blijft.

## Belangrijkste functies

### 1. Visueel grid & drag-and-drop
Het hart van de tool is een visueel overzicht van alle spreads. Je kunt pagina's eenvoudig verslepen om de volgorde aan te passen. De logica houdt rekening met spreads (linker- en rechterpagina's) en zorgt dat de rug van het blad altijd correct wordt weergegeven.

### 2. Slimme vergrendeling (Lock & Flow)
Pagina's of hele artikelen kunnen worden vergrendeld via het slot-icoontje. 
* **Vaste rotsen:** Een vergrendelde pagina blijft altijd op dat specifieke paginanummer staan (bijvoorbeeld een vaste advertentie op pagina 4).
* **Waterstroom:** Wanneer je niet-vergrendelde pagina's verplaatst of toevoegt, 'stromen' deze automatisch om de vergrendelde pagina's heen. Hierdoor blijft je vaste stramien intact terwijl je met de redactionele inhoud schuift.
* **Groeps-lock:** Klik je op het slotje van een pagina die deel uitmaakt van een artikelgroep? Dan wordt direct het hele artikel vergrendeld of ontgrendeld.

### 3. Groeperen & kleuren
Je kunt meerdere pagina's selecteren en groeperen tot één artikel. Deze krijgen automatisch een gedeelde kleur en titel. Dit maakt het in één oogopslag duidelijk waar een artikel begint en eindigt. Ook kun je handmatig kleuren toekennen aan pagina's of rubrieken voor een beter overzicht.

### 4. Import & export
* **Excel-export:** Genereer met één klik een visueel Excel-bestand (`.xlsx`). De bestandsnaam wordt automatisch gegenereerd als `Plank_[Titel]_[Datum]`.
* **Excel-import:** Importeer een artikellijst om direct een basisplan te genereren. Dit bestand moet drie kolommen bevatten met in kolom 1 de rubrieksnaam, in kolom 2 de artikelnaam en in kolom 3 het aantal pagina's dat je voor het artikel wilt reserveren.
* **Back-ups:** Je kunt de volledige staat van je flatplan opslaan als een `.json` bestand en dit later weer inladen.
* **PDF/print:** De tool is geoptimaliseerd voor print naar A4, zodat je een fysieke versie van het plankje kunt uitdraaien voor overleg.

## Hoe te gebruiken

### Online (GitHub Pages)
Bezoek de [GitHub Pages URL van dit project](https://ee1koo.github.io/plankie/) om de tool direct te gebruiken in je browser.

### Lokaal
1.  Download het bestand `index.html` uit deze repository.
2.  Open het bestand in een moderne browser (Chrome, Edge, Firefox, Safari).
3.  Je kunt direct beginnen met plannen.

## Besturing

* **Slepen:** Pak een pagina op en sleep deze naar een nieuwe plek.
* **Klikken:** Klik op tekstvakken om titels of rubrieken aan te passen.
* **Selectiemodus:** Activeer de selectiemodus rechtsboven om meerdere pagina's tegelijk te selecteren voor groepering.
* **A / W:** Gebruik de knoppen onderaan een pagina om deze snel te markeren als Advertentie of Werf.

## Versiegeschiedenis

**v1.10**
* Excel-export bestandsnaam aangepast naar formaat `Plank_[Naam]_[Datum]`.

**v1.9**
* Verbeterde vergrendeling: het slotje werkt nu op de hele groep als een pagina onderdeel is van een artikel.

**v1.8**
* Flow-logic toegevoegd: vergrendelde pagina's fungeren als vaste obstakels waar andere content omheen vloeit.

**v1.7**
* Introductie van de visuele lock-functie en placeholders.

## Privacy & data
Deze applicatie is 'client-side'. Dit betekent dat er geen gegevens naar een server worden verstuurd. Alles wat je invult, wordt opgeslagen in de `localStorage` van je eigen browser. Als je je browsergegevens wist, wordt het flatplan ook gewist. Maak daarom regelmatig een backup via de export-functie.
