# Lokale Veranstaltungsapp – ohne Ticketmaster

Diese Version sucht lokale Veranstaltungshinweise aus Nachrichten-/RSS-Suchergebnissen.
Sie ist für Flohmärkte, Märkte, Stadtfeste, Kirmes, Schützenfeste, Familien- und Vereinsfeste gedacht.

## Funktionen
- PLZ als Ausgangspunkt
- Radius 10 / 25 / 50 / 75 / 100 km
- nahegelegene Orte werden automatisch ermittelt
- mehrere typische Event-Suchgruppen
- Dubletten werden entfernt
- Kategorienfilter
- 10 Treffer pro Seite
- Link zur Original-Nachrichtenquelle
- versucht Veranstaltungsdatum aus Überschrift/Beschreibung zu erkennen
- kein Ticketmaster-Key und kein sonstiger kostenpflichtiger API-Key nötig

## Warum ein Server nötig ist
Browser dürfen viele Nachrichten-RSS-Feeds nicht direkt abrufen (CORS).
Darum enthält dieses Projekt `server.js`. GitHub Pages allein reicht für diese Version nicht.

## Einfaches Deployment
Geeignet sind z. B. Render, Railway oder ein eigener Node.js-Webspace.
- Projekt/ZIP hochladen bzw. GitHub-Repository verbinden
- Build Command: `npm install`
- Start Command: `npm start`
- Node 20 oder neuer

## Wichtiger Hinweis
Die App kann nicht garantieren, wirklich jede lokale Veranstaltung zu finden.
Nachrichtenhinweise sind redaktionell unvollständig und Termine werden nicht immer strukturiert angegeben.
Bei automatisch erkannten Datumsangaben ist deshalb immer die verlinkte Originalquelle maßgeblich.
