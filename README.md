# Manning Guide · mamu hospitality

Interaktives Tool zur Berechnung des Personalbedarfs eines Hotels. Aus einem Beispiel-Dienstplan für einen Tag wird der Bedarf für ein ganzes Jahr hochgerechnet.

## Was das Tool berechnet

| Kennzahl | Bedeutung |
|---|---|
| **Heads** | Intern besetzte Schichten pro Tag, ohne Fremdfirmen |
| **IDEAL** | Jahresbedarf an Köpfen inkl. Urlaub, freier Tage, Feiertage und Krankheit (über Arbeitstage) |
| **FTE** | Vollzeitäquivalente über die Jahresarbeitsstunden |
| **Spinde** | Positionen mit Spind, ohne Executive-Team, inkl. Fremdfirmen |
| **Mitarbeiter je Zimmer** | IDEAL ÷ Zimmeranzahl |

## Funktionen

- **Parameter:** Urlaubs-, Feier-, Krankheits- und freie Tage, Betriebstage, FTE-Basis
- **Pausenregeln je Land:** Österreich (AZG § 11), Deutschland (ArbZG § 4), Schweiz (ArG Art. 15), Italien (D.Lgs. 66/2003 Art. 8), Kroatien (Zakon o radu čl. 73) oder eigene Regel
- **Tagesdienstplan:** Schichten per Ziehen auf dem Zeitstrahl ändern (15-Minuten-Raster)
- **Beschäftigungsausmaß:** Vollzeit, Teilzeit und Part Timer werden automatisch aus der Dienstzeit errechnet
- **FTE-Haken je Position:** 5-Tage-Woche (1 : 1) oder 7-Tage-Bedarf (hochgerechnet)
- **F&B-Öffnungszeiten:** pro Outlet, Wochentag und Zeitfenster; ein neues Outlet legt automatisch einen Bereich im Dienstplan an
- **Abdeckungsprüfung:** zeigt Lücken, in denen ein Outlet geöffnet, aber nicht besetzt ist
- **Housekeeping:** Zimmermädchen automatisch aus Zimmern, Auslastung und Zimmern je Mitarbeiter
- **Export:** PDF mit allen Seiten, Excel-Datei; Import der Manning-Guide-Excel-Vorlage

## Nutzung

Die Datei `index.html` ist das komplette Tool. Sie läuft ohne Installation im Browser, entweder über GitHub Pages oder lokal per Doppelklick.

**Speicherung:** Projekte werden im Browser gespeichert (lokaler Speicher). Sie sind damit an Gerät und Browser gebunden. Mit **Sichern** werden alle Projekte als JSON-Datei heruntergeladen, mit **Importieren** wieder geladen.

**Externe Bibliotheken** werden zur Laufzeit von CDNs geladen: SheetJS (cdnjs) für Excel, jsPDF und jsPDF-AutoTable (jsDelivr) für den PDF-Export sowie Google Fonts.

---

© mamu hospitality · Schönbrunner Straße 179 · AT-1120 Vienna · [mamuhospitality.com](https://www.mamuhospitality.com)
