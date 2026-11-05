# VKT CleanMate

[English](../README.md) | [中文](README_zh.md) | [日本語](README_ja.md) | Deutsch | [Español](README_es.md) | [Français](README_fr.md)

Erst sehen, was gelöscht wird — dann löschen. Vertraute Seiten bleiben unangetastet, und Sie erfahren nebenbei, wohin Ihre Zeit tatsächlich geht.

> Chrome · Edge · Firefox · Manifest V3 · Minimale Berechtigungen · Nur lokal · Keine Analyse

Teil der [VKT](https://www.annmax1983.com/) Datenschutz-Toolbox.

---

## Warum VKT CleanMate?

Die meisten Cleaner sind ein einziger großer „alles löschen"-Knopf. Genau deshalb traut sich kaum jemand, sie einzuschalten: ein Klick, und alle Anmeldungen sind weg. Schlimmer noch — vor dem Klick wissen Sie nicht, ob er 3 Seiten oder 3000 trifft.

VKT CleanMate trennt die Entscheidung von der Ausführung.

| Was andere Cleaner tun | Der Preis |
|---|---|
| Ein Schalter löscht alles | Ein Fehlklick, und Sitzungen, Cookies und Downloadverlauf sind weg |
| Ein Bestätigungsdialog ohne Zahlen | Sie können vorher nicht erkennen, ob 3 oder 3000 Seiten betroffen sind |
| Seitenregeln hinter einem Regex-Feld | Niemand schreibt sie, also wird der „sichere" Modus nie benutzt |

| Was VKT CleanMate tut | Das Ergebnis |
|---|---|
| **Vorschau bei jedem manuellen Lauf** | Echte Zahlen aus dem Browser: gefundene Seiten, Verlaufseinträge, Cookies, aktive Datentypen, Aufbewahrungsfenster |
| **Die kostenlose Stufe kann nicht alles löschen** | Für kostenlose Nutzer gibt es keinen Weg zum versehentlichen Datenverlust — als Design, nicht als Warnung |
| **Zwei Listen in entgegengesetzte Richtungen** | Reinigungsliste („nur diese", kostenlos) und Schutzliste („niemals diese", ebenfalls kostenlos und in beiden Modi wirksam) |
| **Grenzen werden aufgeschrieben** | In der Oberfläche und in dieser README, statt von einem Reviewer entdeckt zu werden |

In einem Satz: **vor dem Löschen sehen, was verschwindet — nach dem Löschen wissen, wohin die Zeit ging.**

---

## Funktionen

### 🆓 Dauerhaft kostenlos

| Funktion | Was sie tut |
|---|---|
| Vorschau | Gefundene Seiten, Verlaufseinträge, Cookies, Datentypen und Aufbewahrung vor jedem manuellen Lauf |
| Gezielter Modus | Löscht nur die Domains Ihrer Reinigungsliste. Unbegrenzt viele Einträge |
| Neun Datentypen | Verlauf, Cache, Cookies, Downloadverlauf, Formulardaten, lokaler Speicher, IndexedDB, Service Worker, gespeicherte Passwörter — je ein eigener Schalter |
| Aufbewahrung | Letzten Tag / 3 Tage / 7 Tage / 30 Tage behalten oder alles |
| Fünf Auslöser | Beim Start, beim Schließen, alle N Minuten, täglich zu fester Zeit, nach N Minuten Inaktivität |
| Umfang pro Auslöser | z. B. alle paar Stunden Verlauf + Cache, beim Schließen ein gründlicher Lauf inklusive Cookies |
| Tastenkombinationen | `Alt+Shift+C` jetzt reinigen · `Alt+Shift+X` reinigen und alle Tabs und Fenster schließen |
| Aufschieben | Den nächsten automatischen Lauf um eine Stunde verschieben |
| Benachrichtigungen | Eine Zusammenfassung nach jedem Lauf |
| Sechs Sprachen | English, 简体中文, 日本語, Deutsch, Español, Français |

### ⭐ Pro (Lizenz erforderlich)

| Funktion | Was sie tut |
|---|---|
| Vollmodus | Alles außer Ihrer Schutzliste löschen |
| Schutzliste | Die Domains, die nie angefasst werden; bei Konflikt gewinnt der Schutz |
| Fokus-Fußabdruck | Echte Fokuszeit pro Domain, 24-Stunden-Verteilung, Rangliste, Vorschläge „lohnt sich zu reinigen" |
| CSV-Export | Der Fußabdruck als CSV, eine Zeile pro Domain |

Eine Lizenz deckt zwei Browser ab. Nach Ablauf einer Lizenz laufen die kostenlosen Funktionen weiter.

---

## Was es kann und was nicht

### ✅ Es kann

- Verlauf, Cache, Cookies, Downloads, Formulardaten, lokalen Speicher, IndexedDB, Service Worker und Passwörter in beliebiger Kombination löschen.
- Einen Lauf auf die von Ihnen genannten Domains begrenzen — inklusive Subdomains, ohne Regex.
- Im Vollmodus die geschützten Domains überspringen.
- Nach Zeitplan reinigen, mit eigenem Datenumfang pro Auslöser.
- Nach jedem Lauf genau berichten, was entfernt wurde.

### ❌ Es kann nicht

- DNS-Caches, Router-Protokolle, Provider-Aufzeichnungen oder serverseitige Logs löschen. Die liegen nicht auf Ihrem Gerät.
- Gelöschten Verlauf wiederherstellen. Chromium bietet keiner Erweiterung eine API, um Verlauf zurückzuschreiben.
- Daten eines anderen Browsers, eines anderen Profils oder einer auf ein anderes Gerät synchronisierten Kopie löschen.
- Verlauf, Downloads, Formulardaten oder Passwörter auf eine einzelne Seite begrenzen. Der Browser gibt das nicht her; diese vier werden nur im Vollmodus gefiltert, und die Oberfläche sagt das neben dem Kästchen.
- Den Auslöser „beim Schließen des Browsers" garantieren. Er ist Best-Effort: ein Absturz, ein erzwungener Neustart oder ein Stromausfall kann diesen Lauf verlieren.
- Löschen, was nie gespeichert wurde. Eine Seite, die Sie nur in einem privaten Fenster gelesen haben, hinterlässt nichts.
- Ein VPN ersetzen oder gegen Überwachung auf Netzwerkebene schützen. Es ist ein Selbstbedienungswerkzeug für Ihren eigenen Browser auf Ihrem eigenen Gerät.

---

## Vorschau

> 📸 Store-Material liegt in [`screenshots/`](../screenshots/) — fünf Bilder in 1280×800 plus je eine Promo-Kachel in 1400×560 und 440×280.

| Bild | Inhalt |
|---|---|
| [`01-popup.png`](../screenshots/01-popup.png) | Popup in der Toolbar, aktuelle Seite bereits in der Reinigungsliste |
| [`02-preview.png`](../screenshots/02-preview.png) | Das Bestätigungsblatt „Before cleaning" |
| [`03-cleaning.png`](../screenshots/03-cleaning.png) | Einstellungen: Modus, Datentypen, Aufbewahrung, Auslöser |
| [`04-lists.png`](../screenshots/04-lists.png) | Einstellungen: Reinigungsliste und Schutzliste |
| [`05-footprint.png`](../screenshots/05-footprint.png) | Fußabdruck-Seite: Summen, Stundenverteilung, Rangliste |

---

## Unterstützte Browser

| Browser | Status |
|---|---|
| Chrome 116+ (Desktop) | ✅ Unterstützt |
| Microsoft Edge 116+ (Desktop) | ✅ Unterstützt |
| Andere Chromium-Browser mit MV3 | ✅ Sollte funktionieren |
| Firefox (Desktop) | ✅ Unterstützt |
| Handy / Tablet | ❌ Nicht unterstützt — dort gibt es keine Toolbar |
| Private Fenster | ⚠️ Nichts zu löschen: Die Daten werden beim Schließen verworfen |

---

## Installation

**Aus dem Store:** Chrome Web Store, Microsoft Edge Add-ons oder Firefox Add-ons (AMO) → „Zu Chrome hinzufügen" → Symbol in der Toolbar anheften.

**Aus dem Quellcode:**

```bash
npm install          # terser, nur für den Build
npm run build        # dist/ + publish/cleanmate-v<version>.zip
```

Dann `chrome://extensions` → Entwicklermodus → „Entpackte Erweiterung laden" → dieser Ordner (oder das entpackte `dist/`).

---

## Benutzung

### Erster Start

Popup öffnen und **Jetzt reinigen** drücken. Weil standardmäßig der gezielte Modus läuft und die Reinigungsliste leer ist, passiert noch nichts — genau das ist der Punkt. Fügen Sie zuerst eine Domain hinzu, im Popup für die aktuelle Seite oder im Tab **Lists**.

### Die Reinigungsliste füllen

- Im Popup: **Aktuelle Seite hinzufügen** trägt die Domain ein, die Sie gerade ansehen.
- Im Tab Lists: `example.com` eintippen und Add drücken. Subdomains sind automatisch abgedeckt, `www.` wird entfernt.
- Auf der Fußabdruck-Seite (Pro): Die Vorschläge „lohnt sich zu reinigen" und die Zeilen der Rangliste haben je einen Knopf, der die Domain einträgt.

### Automatische Läufe einrichten

Im Tab **Cleaning** hat jeder der fünf Auslöser einen eigenen Schalter. Darunter legt ein Dropdown den Datenumfang dieses Auslösers fest — `global` folgt den Kästchen oben, jeder andere Wert beschränkt den Lauf auf eine Voreinstellung (Verlauf + Cache, Cookies + Cache, alles und so weiter).

Ein vernünftiger Anfang: Verlauf + Cache alle 6 Stunden, alles beim Schließen des Browsers, und Start sowie Inaktivität so lange aus, bis Sie sicher sind, dass Sie sie wollen.

### Tastenkombinationen

| Tasten | Aktion |
|---|---|
| `Alt+Shift+C` | Jetzt reinigen, mit den aktuellen Einstellungen |
| `Alt+Shift+X` | Jetzt reinigen und danach alle Tabs und Fenster schließen |

Beide lassen sich unter `chrome://extensions/shortcuts` ändern.

---

## So funktioniert es

1. Ein Auslöser greift, oder Sie drücken Jetzt reinigen.
2. Der Service Worker im Hintergrund bestimmt den Domainumfang: Ihre Reinigungsliste im gezielten Modus, alles minus Schutzliste im Vollmodus.
3. Bei einem manuellen Lauf zählt er, was betroffen wäre — Seiten, Verlaufseinträge, Cookies — und zeigt das Vorschau-Blatt. **Bisher wurde nichts gelöscht.**
4. Nach der Bestätigung wird jeder gewählte Datentyp über `chrome.browsingData` entfernt, in Stapeln von höchstens 50 Origins. Ein geplanter Lauf (Intervall, täglich, im Leerlauf, beim Schließen) lässt das Blatt weg: er führt Ihre Regeln aus und meldet das Ergebnis per Benachrichtigung.
5. Die Domainregeln werden zuerst in echte Origins aufgelöst — `browsingData` akzeptiert Origins (`https://example.com`) statt nackter Hostnamen und expandiert Subdomains nicht selbst.
6. Eine Benachrichtigung meldet das Ergebnis, der Zeitstempel des Laufs wird gespeichert, und das Blatt bleibt im Popup erreichbar.

Ein Detail, das man kennen sollte: `browsingData` beachtet `origins` nur für Cache, Cookies, lokalen Speicher, IndexedDB, Service Worker und Dateisysteme. Verlauf, Downloads, Formulardaten und Passwörter ignorieren die Origin-Liste vollständig — werden diese Typen gewählt, betrifft der Lauf das gesamte Profil. Die Erweiterung schreibt das in die Oberfläche, statt es zu verschweigen.

---

## FAQ

**Löscht das Reinigen meine Lesezeichen?**
Nein. Lesezeichen sind nicht Teil von `browsingData`, und kein Code der Erweiterung berührt sie.

**Meldet mich das Löschen von Cookies überall ab?**
Im gezielten Modus nur für die Domains Ihrer Liste. Deshalb läuft die kostenlose Stufe ausschließlich im gezielten Modus: Ein vollständiger Lauf ist eine bezahlte Entscheidung, bewusst getroffen, mit Schutzliste in der Hand.

**Kann ich den Verlauf nur einer Seite löschen?**
Ja. Dafür ist die optionale Berechtigung `history` nötig, die erst in dem Moment angefragt wird, in dem Sie Verlauf pro Seite prüfen oder löschen — nicht bei der Installation.

**Werden die mit meinem Google-Konto synchronisierten Passwörter gelöscht?**
Wenn Sie **Gespeicherte Passwörter** anhaken, löscht der Browser den lokalen Passwortspeicher, und ein angemeldetes Profil kann diese Löschung weiterreichen. Genau deshalb ist dieser Typ standardmäßig aus und in der Oberfläche rot markiert. Lassen Sie ihn aus, wenn Sie es nicht wirklich meinen.

**Funktioniert es in privaten Fenstern?**
Ein privates Fenster verwirft seine Daten beim Schließen, es bleibt also nichts zu löschen. Die Erweiterung braucht keinen Zugriff auf private Fenster.

**Der Auslöser „beim Schließen" lief nicht.**
Er ist Best-Effort. Er greift, wenn die Fensterzahl null erreicht; beendet sich der Browser mitten in der Aufgabe, wird der Lauf wenige Sekunden nach dem nächsten Start abgeschlossen. Ein Absturz, ein erzwungener Neustart oder ein Stromausfall verliert diesen Lauf.

**Werden andere Browser oder andere Profile gereinigt?**
Nein. Ein Profil, ein Browser, dieses Gerät.

**Warum ist nur der Vollmodus kostenpflichtig?**
Weil „Alles löschen" der einzige Vorgang ist, der Anmeldungen entfernen kann, die Sie noch brauchen – und das Einzige, was ein gezielter Cleaner strukturell nicht kann. Alles andere hier, inklusive Schutzliste und Fokus-Profil, funktioniert ohne Lizenz. Pro verkauft die riskante Operation und die Langzeit-Aufzeichnung, nicht das Recht, Ihre eigenen Daten zu sehen.

---

## Datenschutz

Keine Analyse, keine Telemetrie, keine Werbung, kein Konto. Die Erweiterung liest keine Seiteninhalte, zeichnet keine Tastatureingaben auf und erstellt kein Profil. Einstellungen liegen in `chrome.storage.local`. Der Fokus-Fußabdruck speichert, wenn aktiviert, Domains, Dauern, Besuchszahlen und eine Stundenhäufigkeit in einem rollenden 30-Tage-Fenster — keine URLs, keine Titel. Die einzige Netzwerkanfrage der gesamten Erweiterung ist die Lizenzprüfung gegen `api.annmax1983.com`, und nur wenn Sie einen Schlüssel einfügen.

**[📄 Vollständige Datenschutzerklärung](../privacy-policy.html)**

### Berechtigungen

| Berechtigung | Wozu |
|---|---|
| `browsingData` | Die von Ihnen gewählten Datentypen löschen |
| `storage` | Einstellungen und den optionalen Fußabdruck lokal speichern |
| `alarms` | Zeitpläne plus ein Minuten-Heartbeat für die Fokusmessung |
| `tabs` | Die aktuelle Domain kennen und auf den sichtbaren Tab wirken |
| `windows` | Erkennen, wann das letzte Fenster schließt — Grundlage des Auslösers „beim Schließen" |
| `idle` | Der optionale Auslöser „nach Inaktivität" |
| `notifications` | Die Ergebniszusammenfassung nach einem Lauf |
| `history` *(optional)* | Nur beim Prüfen oder Löschen von Verlauf pro Seite |
| `cookies` *(optional)* | Nur beim Löschen von Cookies pro Seite |
| `api.annmax1983.com` | Ausschließlich Lizenzaktivierung und -prüfung |

Wegen dieser zwei optionalen Berechtigungen erscheint bei einer frischen Installation keine rote Warnung zum Lesen des Verlaufs.

---

## Entwicklung

```bash
npm install                   # terser, nur für den Build
npm run icons                 # icons/*.png neu erzeugen (keine Abhängigkeiten)
npm run build                 # dist/ + publish/cleanmate-v<version>.zip
npm run shoot                 # screenshots/ in Store-Größen neu erzeugen
node tools/check-locales.js   # prüft, ob alle sechs Sprachen denselben Keysatz haben
```

Laden: `chrome://extensions` → Entwicklermodus → „Entpackte Erweiterung laden" → dieser Ordner.

### Projektstruktur

```
manifest.json          MV3, service_worker als ES-Modul
background.js          Zeitpläne, Regelwerk, Löschausführung, Fokusmessung
license.js             Creem-Lizenz (plugin id: cleanmate)
common/                store (Defaults/Merge), Domainabgleich, i18n, Formatierung, ui.css
popup/                 Ein-Klick-Reinigung + Vorschau-Blatt + Aktionen zur aktuellen Seite
options/               Modus, Datentypen, Auslöser, Listen, Fußabdruck-Schalter, Lizenz
insights/              Fußabdruck-Seite — Anzeige kostenlos; Aufzeichnung läuft, solange die Seite offen ist (Daueraufzeichnung ist Pro)
_locales/              en, zh_CN, ja, de, es, fr (je 174 Keys)
languages/             READMEs in allen Sprachen
assets/                gemeinsame UI-Symbole
store-listing/         Store-Texte in sechs Sprachen
index.html             Landingpage (nicht im Erweiterungs-ZIP)
promo.html             Promo-Kachel (Screenshot-Ziel) — 1400×560, `?size=small` ergibt 440×280
screenshots/           Store-Screenshots, neu erzeugt durch `npm run shoot`
tools/make-icons.js    PNG-Icongenerator ohne Abhängigkeiten
tools/check-locales.js prüft den Keysatz aller Sprachen
tools/shoot.js         rendert jede Oberfläche in Store-Größen
tools/harness/         Mock-chrome.* und eine Testseite, nur für tools/shoot.js
```

### Zum Fokus-Tracker

- Standardmäßig aus und Teil der bezahlten Stufe.
- Im Standardmodus wird **nur aufgezeichnet, solange die Fußabdruck-Seite offen ist** (ein langlebiger Port hält sie am Leben). Schließen stoppt die Aufzeichnung.
- Der Service Worker kann kein `setInterval` nutzen — Sitzungen werden bei Tab-/Fenster-Ereignissen abgeschlossen und von einem Minuten-Alarm nachgezogen.
- Gespeichert werden nur `domain`, `duration`, `visits` und eine Stundenhäufigkeit. Keine URLs, keine Titel.
- Kostenlose Nutzer sehen eine Lizenzkarte statt der Seite; es wird kein Port geöffnet, also nichts aufgezeichnet.

---

## Urheberrecht

VKT CleanMate ist ein unabhängiges Werkzeug und steht in keiner Verbindung zu Google, Microsoft oder anderen Browserherstellern. Chrome, Edge und Firefox sind Marken ihrer jeweiligen Inhaber.

Die Erweiterung löscht Daten über die APIs des Browsers. Sie patcht den Browser nicht, verändert keine Systemdateien und installiert nichts außerhalb ihres eigenen Erweiterungsordners.

---

## Hinweis zum Quellcode

Das veröffentlichte Paket enthält lesbares JavaScript — keine Verschleierung. `dist/` ist der gebaute, minimierte Stand; der Quellcode in diesem Repository ist die Eingabe dafür. Nichts wird remote geladen: keine `eval`, keine Remote-Skripte, keine dynamischen Importe außerhalb des eigenen Pakets — erzwungen durch die MV3-Content-Security-Policy in `manifest.json`.

---

## ❤️ Unterstützen

**[👉 Lizenzschlüssel holen](https://annmax1983.com/extensions/cleanmate)** · **[☕ Spendier mir einen Kaffee](https://ko-fi.com/annmax?ref=vkt-clean-mate)** · [Quellcode auf GitHub](https://github.com/annmax1983/vkt-clean-mate) · [Offizielle Website](https://annmax1983.com/)

---

## Lizenz

Copyright © 2026 VKT CleanMate. All rights reserved.
