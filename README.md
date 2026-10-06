# Byggnadsbiten Dalarna

Komplett statisk webbplats med 15 sidor, 39 galleribilder och fem originalfilmer. Allt i `dist/` är färdigt att publicera. Ingen installation behövs för webbplatsen.

## GitHub Pages

1. Ladda upp innehållet i `dist/` (eller packa upp GitHub-zippen direkt) till roten i ditt repository. Behåll mappstrukturen.
2. Öppna Settings → Pages, välj Deploy from a branch och main / root.
3. GitHub visar webbplatsens adress när publiceringen är klar.

`index.html` måste ligga i roten tillsammans med `styles.css`, `app.js`, `fonts.css`, de andra HTML-sidorna och mappen `assets`. Filmerna ligger lokalt i assets, största filen cirka 21 MB.

## Kontakt och offert

Telefon, e-post, karta och Instagram leder till företagets befintliga kontaktvägar. Offertformuläret förbereder ett mejl lokalt. Besökaren granskar texten och skickar själv via sitt mejlprogram. Det finns också en länk till företagets befintliga offertformulär. Inga uppgifter skickas automatiskt, lagras på server eller sparas i webbläsaren.

## Innehåll och original

Företagsinformation, egna filmer, foton, kontaktvägar och projekt hämtades från https://www.byggnadsbiten.se den 5 oktober 2026. Bildernas källor finns i `assets/sources.json`, filmernas i `assets/video-sources.json`. Webbplatsen använder originalmaterial, inte genererade projektbilder. En originalbild med stockfilnamn anges som illustrationsbild i galleriet.

De fem offentliga originalfilmerna har paketerats som vanliga MP4-filer utan redaktionella ändringar. Bakgrundsfilmen är ljudlös och kan pausas. Vid inställningen Minskad rörelse visas stillbild tills besökaren väljer att spela. Filmernas original på Vimeo är fortsatt länkade.

Text och bilder är en daterad ögonblicksbild. Inga priser, projektantal, totalbetyg eller nya certifieringar har lagts till. Dalakåkens uppgift om 280 kvadratmeter anger uttryckligen att 40 kvadratmeter var planerad utbyggnad enligt källan.

## Redigera

Sidan fungerar med vanlig HTML, CSS och JavaScript. I utvecklingsprojektet samlar `build.py` de gemensamma delarna, `templates/hero.html` startsidans öppning och `source-manifest.json` källmaterialet. Kör `python3 build.py` från projektroten om du vill återskapa alla sidor; Python-paketet beautifulsoup4 behövs. Stil och funktion finns direkt i `dist/styles.css` och `dist/app.js`.

Typsnitt: Barlow Condensed och Onest, lokalt inkluderade med respektive OFL-licens.
