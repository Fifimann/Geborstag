# Geborstag

Kleine, statische Einladung/RSVP-Seite — bereit für GitHub Pages. Du hast Option A gewählt (externer Formular-Endpoint), deshalb sendet das Formular die Daten an einen konfigurierbaren Endpoint (z. B. Formspree).

Was in diesem Repo ist
- index.html — Die deutsche Einladungsseite mit dem Formular (Vorname, Nachname, Kommt, Anzahl Gäste, Nachricht).
- css/styles.css — Einfaches, responsives Styling.
- js/app.js — Formular-POST; setze die Konstante `FORM_ENDPOINT` auf deine Formular-URL.

Wie du das Formular mit Formspree verbindest
1. Gehe zu https://formspree.io/ und erstelle ein Formular (kostenloser Einstieg möglich).
2. Du bekommst eine Endpoint-URL im Format `https://formspree.io/f/<form_id>`.
3. Öffne `js/app.js` und ersetze den Platzhalter `<<TRAGE_HIER_ENDPOINT_EIN>>` durch deine Endpoint-URL.

Lokal testen
1. Repository klonen:
   git clone git@github.com:Fifimann/Geborstag.git
2. In das Verzeichnis wechseln:
   cd Geborstag
3. Einen einfachen statischen Server starten, z. B.:
   python3 -m http.server 8000
   oder mit Node (falls installiert):
   npx serve .
4. Im Browser öffnen: http://localhost:8000

Veröffentlichen mit GitHub Pages
1. Gehe zu deinem Repository → Settings → Pages.
2. Wähle Branch: `main` (oder deinen Default-Branch) und Root als Ordner.
3. Speichern. Nach ein paar Minuten ist die Seite verfügbar unter:
   https://<dein-github-username>.github.io/Geborstag

Hinweis
- Das Formular sendet keine E-Mail-Adressen (du wolltest kein E-Mail-Feld). Falls du später E-Mails sammeln willst, füge ein Feld `E-Mail` in `index.html` ein.
- Wenn du stattdessen ein selbstgehostetes Backend möchtest, sag Bescheid — ich erstelle dann Express-API und speichere Einträge (Option B).

Viel Spaß mit deiner Geburtstagseinladung!