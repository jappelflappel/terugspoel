# Mokje Gokje

Mokje Gokje is een Nederlandstalig muziektijdlijnspel voor twee tot acht teams. Open het hostscherm op de laptop en laat ieder team met één telefoon de deelname-QR scannen. De QR blijft in beeld op het hostscherm en werkt ook om opnieuw aan te sluiten. Op een andere telefoon gebruik je de teamcode van acht tekens. De host vindt die codes in **Spelbeheer**.

[Speel Mokje Gokje](https://jappelflappel.github.io/mokje-gokje/) · [Bekijk de actuele broncode](https://github.com/jappelflappel/mokje-gokje)

## Spotify

Kies **Mokje Gokje-mix** voor 69 nummers. **Volgende nummer** opent de track in Spotify en start de plaatsing in Mokje Gokje. Op de Mac opent **⌘-klik** de link in een achtergrondtab. Start de muziek in Spotify. Teams plaatsen op de eigen telefoon of via de tijdlijn op het hostscherm.

Voor **Eigen playlist** plak je de Spotify-playlistlink. De DJ speelt een nummer uit de playlist en voert de titel, artiest en het uitgavejaar in via het DJ-scherm. Sorteer op het jaar waarin de gekozen opname voor het eerst verscheen.

Het spel gebruikt gewone links naar Spotify. Inloggen en afspelen gebeuren in de Spotify-app of webspeler. [Spotify Developer Policy](https://developer.spotify.com/policy)

## Spelen

1. Elk team begint met één kaart en twee munten. De host trekt een nummer en opent de plaatsing zodra de muziek speelt.
2. Het actieve team kiest een vak in de eigen tijdlijn. Hetzelfde jaar is aan beide kanten geldig.
3. Andere teams kunnen één munt inzetten op een ander vak in die tijdlijn. Elk vak kan één keer worden geclaimd. Een juiste plaatsing gaat voor. Bij een foute plaatsing wint het eerste team met een juiste steelpoging de kaart.
4. De host onthult het jaar en beslist of het actieve team een bonusmunt krijgt. Het eerste team dat het kaartdoel haalt, wint.

## Lokaal draaien

Gebruik Node.js 22 of nieuwer.

~~~sh
npm ci
npm test
npm run dev
~~~

Open [localhost:4173](http://localhost:4173). Gebruik voor verbindingen vanaf andere apparaten op hetzelfde netwerk het lokale IP-adres van de Mac in plaats van localhost.

De bron van de webclient staat in **client/**. **server/** bevat de spelregels en HTTP-API. De lokale server bewaart kamers in SQLite. De online Worker gebruikt D1. Kamers verlopen na drie dagen zonder spelactie. De map **docs/** bevat de gebouwde client voor GitHub Pages. Bouw deze map na clientwijzigingen opnieuw met **npm run build**.
