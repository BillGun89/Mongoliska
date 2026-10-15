# Mongolbota – lär dig mongoliska

En svensk–mongolisk lärplattform med responsiv design. Projektet bygger vidare på dina uppladdade `index.html` och `words.json`.

## Kom igång

**Snabbast:** öppna filen `Mongolbota_hela_sidan.html` i Chrome, Safari eller Firefox. Den innehåller HTML, CSS, JavaScript och alla ord i en enda fil och behöver inte en server.

**För att redigera koden:** öppna `index.html` i projektmappen. Behåll `style.css`, `app.js` och `data.js` i samma mapp. Vid publicering kan du ladda upp dem till GitHub Pages eller valfritt statiskt webbhotell.

## Vad ingår?

- 512 unika ord och uttryck från grundmaterialet, din extra JSON-lista och utökade kategorier.
- Sökklar ordbok och kategorifilter, även på mongoliska och med latinsk translitterering.
- Ordkort, flervalsfrågor, stavning med kyrilliskt skärmtangentbord, och para ihop.
- 61 skrivna vardagsmeningar med meningsbyggande och tidsformer.
- Ett separat meningsläge där samtliga ord kan komma med. Detta använder språkligt återanvändbara mallar kring ordet/uttrycket i citattecken. Det är inte en automatisk grammatisk böjare som kan stoppa godtyckliga ord i vilken mening som helst.
- Verb, grammatikquiz, parlör, interaktivt alfabet, egna ord, XP och personliga framsteg.
- Responsiv mobil- och desktopdesign, ljust/mörkt läge.

## Lägga till ord

Du kan lägga in ett enskilt ord eller importera JSON under **Egna ord**. De sparas i den aktuella webbläsarens `localStorage`. Du kan även exportera dem igen.

Formatet är:

```json
[
  {"mn": "Морь", "sv": "Häst", "cat": "Djur"},
  {"mn": "Сайн уу?", "sv": "Hej", "cat": "Fraser"}
]
```

Vid publicering på en webbserver kan du redigera `words.json` i projektmappen för att ändra den utökade ordlistan för alla besökare. När HTML-filen öppnas direkt från datorn används den inbyggda kopian; använd i så fall formuläret eller importfunktionen för ändringar utan server. `data.js` innehåller dessutom grundorden, de skrivna meningarna och parlören.

## Bra att känna till

- Personliga framsteg delas inte mellan enheter, då projektet saknar konto och databas.
- Uttalsknappar visas endast om webbläsaren erbjuder en mongolisk talsyntesröst. Uttalsstödet är därför enhetsberoende.
- Stavning och enklare quiz utgår från de angivna översättningarna. En mänsklig språkgranskning av extra ord och exempel är lämplig före undervisning.
- Projektet använder Google Fonts om nätuppkoppling finns; lokala systemtypsnitt används annars.

## Projektfiler

- `index.html` – layout och sidornas innehåll
- `style.css` – design och responsiv CSS
- `data.js` – grundord och språkdata
- `app.js` – logik, övningar och elevens framsteg
- `words.json` – utökad ordlista, redigerbar vid publicering
