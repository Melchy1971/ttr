# click-TT Q-TTR Scraper (Weg 1, groupPools) – GUI

Dieses Tool ermöglicht das komfortable Auslesen und Exportieren von Q-TTR-Werten aus click-TT für beliebige Gruppen, Saisons und Runden. Die grafische Oberfläche erlaubt eine einfache Bedienung und den Export der Daten als JSON, CSV, Markdown oder Excel.

---

## Features

- **Einfache GUI**: Übersichtliche Oberfläche für alle Einstellungen und Aktionen
- **Fenster startet immer maximiert**
- **Gruppenverwaltung**: Gruppen (Name & ID) können komfortabel verwaltet und in einer frei wählbaren Datei gespeichert werden (`gruppen.json`)
- **Konfigurationsspeicherung**: Alle Einstellungen (inkl. Gruppen-Dateipfad) werden in `config.json` gespeichert und beim Start automatisch geladen
- **Abruf & Parsing**: Q-TTR-Daten werden robust abgerufen (mit HTTP-Retry & Cache) und geparst
- **Sortierbare Tabelle**: Vorschau der Daten mit Sortierfunktion
- **Export**: Datenexport als JSON, CSV, Markdown oder XLSX (inkl. Team-Statistiken und Top-10)
- **Team-Mittelwerte**: Automatische Berechnung und Anzeige der Team-Durchschnitte
- **Druckfunktion**: Über den Button **"Drucken"** kann eine PDF erzeugt und direkt gedruckt werden (inkl. Vorschau und Optionen)
- **Plattformneutral**: Läuft unter Windows, Linux und macOS
- **Exit-Button**: Beendet das Programm sauber

---

## Voraussetzungen

- **Python 3.7+**
- Benötigte Pakete:
  - `requests`
  - `requests_cache`
  - `beautifulsoup4`
  - `openpyxl`
  - `platformdirs`
  - `reportlab`

Installiere die Abhängigkeiten mit:

```
pip install requests requests_cache beautifulsoup4 openpyxl platformdirs reportlab
```

---

## Nutzung

1. **Starten**  
   Im Terminal:
   ```
   python start
   ```

2. **Parameter eingeben**
   - **Base-URL:** z.B. `https://ttbw.click-tt.de`
   - **Saison:** z.B. `TTBW 2025/26`
   - **Runde:** `vorrunde` oder `rueckrunde`
   - **Gruppe:** Auswahl aus Dropdown (Bezeichnung) oder eigene ID
   - **Sprache:** Deutsch oder Englisch
   - **Datenformat:** JSON, CSV, Markdown oder XLSX

3. **Gruppen verwalten**  
   Über den Button **"Gruppen …"** können Gruppen (Name & ID) hinzugefügt, geändert oder gelöscht werden.  
   Der Speicherort der Gruppen-Datei (`gruppen.json`) ist frei wählbar und wird in der Konfiguration gemerkt.

4. **Abrufen & Exportieren**
   - Mit **"Abrufen"** werden die Daten geladen und in der Tabelle angezeigt.
   - Mit **"Speichern …"** können die Daten im gewählten Format exportiert werden.

5. **Drucken**
   - Über den Button **"Drucken"** kann eine PDF erzeugt und direkt gedruckt werden (inkl. Vorschau und Optionen).

6. **Konfiguration speichern**  
   Über **"Einstellung"** kann die aktuelle Konfiguration als Standard gespeichert werden (`config.json`).

7. **Beenden**
   - Über den **"Exit"**-Button wird das Programm sauber geschlossen.

---

## Hinweise

- Die Nutzung erfolgt auf eigene Verantwortung. Bitte beachte die Nutzungsbedingungen und Rate-Limits der jeweiligen click-TT-Portale.
- Bei Problemen mit fehlenden Paketen siehe Abschnitt "Voraussetzungen".
- Die Konfigurationsdatei (`config.json`) und die Gruppen-Datei (`gruppen.json`) werden im Benutzer-Konfigurationsordner gespeichert (plattformabhängig).

---

## Lizenz

Dieses Projekt ist Open Source. Siehe [LICENSE](LICENSE) für Details.