# Meet je Stad – Tilburg – Persoonlijk weeradvies

## Samenvatting
Template voor een simpele website die real-time de temperatuur ophaalt van een van de Meet je Stad meetstation en op basis daarvan een voorspelling afgeeft.

## Achtergrond
Dit project is onderdeel van een Meet je Stad workshop over data analyse. De workshop geeft een introductie in data analyse o.b.v. de (open) temperatuur data van Meet je Stad. Het doel van de workshop is mensen te laten zien wat er mogelijk is met data analyse. 

## Data & technologie
Het project maakt gebruik van de open data van Meet je Stad. De data worden op twee manieren gebruikt. Ten eerste bevat het project een bestand (`data.js`) met daarin informatie over de schommeling van temperaturen in een bepaalde periode van het jaar. Daarnaast haalt de website real-time de laatste meting van een sensor op. 
De website is gebouwd met HTML, CSS en Javascript. 

## Hoe te gebruiken
Je kan m.b.v. dit repository je eigen weeradvies website maken. Je kan je eigen voorspelling configureren door het volgende gedeelte in `index.html` aan te passen:

```javascript
...

// waardes die je kan aanpassen         
let name = 'Erik';
let advice = 'korte broek';
let theme = 'blauw'    
let tempLimit = 20;
let higherTxt = 'Je kan een korte broek aan! Lekker!';
let betweenTxt = 'Hmm... je moet zelf even voelen.';
let lowerTxt = 'Helaas pindakaas! Het is wat fris.';
let sensor = '427';

...
```
Hier een korte uitleg over de waardes:

- **name**: de naam van de persoon die het advies geeft.
- **advice**: hetgeen waar je advies over wil geven.
- **theme**: de achtergrondkleur van de website. Opties: zwart, blauw, geel of roze.
- **tempLimit**: de grenstemperatuur voor je voorspelling.
- **higherTxt**: de tekst die je wil zien als de huidige temperatuur hoger ligt dan de grens, of de temperatuur o.b.v. de voorspelling hoog genoeg uit gaat komen.
- **betweenTxt**: de tekst die je wil zien als de temperatuur niet zeker hoger over lager dan de grens uit gaat komen.
- **lowerTxt**: de tekst die je wil zien als de temperatuur onder de grenswaarde zal blijven.
- **sensor**: het identificatienummer (ID) van het Meet je Stad meetstation die je wil uitlezen.

Bovenstaande instelling resulteren in het onderstaande:

<img alt="Voorbeeld Meet je Stad weeradvies website" src="/meetjestad-tilburg-weeradvies-voorbeeld.png" width="300">

De website vult de informatie uit de instellingen (name, advice, theme, tempLimit en ...Txt) automatisch op de juiste plek in.


## Uitdagingen
Het weer voorspellen is een ingewikkeld iets. Bij de ontwikkeling van dit project is ervoor gekozen om met één type data (temperatuur) te werken. Dit heeft als doel de variatie in type data tijdens de workshop te minimaliseren tot één. Het project geeft een indicatie voor een weerdadvies af, maar het is niet bedoeld als accuraat middel om voorspelling op te baseren.

## Vervolgstappen
Op het moment staan er geen verdere ontwikkelingen gepland. Mocht je interesse hebben in verdere uitleg (over het project of de workshop), neem gerust contact met me op. 

## Met dank aan
[Meet je Stad](https://meetjestad.net/) voor de open data, lettertype op de website is [Robot van Google Fonts](https://fonts.google.com/specimen/Roboto). 
