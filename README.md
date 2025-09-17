# click-TT Q-TTR Scraper (Weg 1)

Dieses Tool ermöglicht das Auslesen und Exportieren von Q-TTR-Werten aus click-TT für eine bestimmte Gruppe, Saison und Runde. Die grafische Oberfläche erlaubt eine einfache Bedienung und den Export der Daten als JSON, CSV oder Markdown.

## Features

- **Eingabemaske** für Base-URL, Saison, Runde, Group-ID, Sprache und Datenformat
- **Abruf & Parsing** der Q-TTR-Daten (mittels `requests` und `BeautifulSoup`)
- **Vorschau** der Daten in einer Tabelle
- **Export** als JSON, CSV oder Markdown
- **Team-Mittelwerte** werden berechnet und angezeigt
- **Plattform:** Windows (andere Plattformen möglich)

## Voraussetzungen

- Python 3.7 oder neuer
- Benötigte Pakete:
  - `requests`
  - `beautifulsoup4`

Installiere die Abhängigkeiten mit:

```
pip install requests beautifulsoup4
```

## Nutzung

1. Starte das Programm:

   ```
   python start
   ```

2. Gib die gewünschten Parameter ein:
   - **Base-URL:** z.B. `https://ttbw.click-tt.de`
   - **Saison:** z.B. `TTBW 2025/26` (achte auf die Schreibweise wie in der echten URL)
   - **Runde:** `vorrunde` oder `rueckrunde`
   - **Group-ID:** z.B. `494514`
   - **Sprache:** Deutsch oder Englisch
   - **Datenformat:** JSON, CSV oder Markdown

3. Klicke auf **"Abrufen"**, um die Daten zu laden.
4. Die Daten werden in der Tabelle angezeigt. Team-Mittelwerte erscheinen im Statusfeld.
5. Klicke auf **"Speichern ..."**, um die Daten zu exportieren.

## Hinweise

- Die Nutzung erfolgt auf eigene Verantwortung. Bitte beachte die Nutzungsbedingungen und Rate-Limits der jeweiligen click-TT-Portale.
- Bei Problemen mit fehlenden Paketen siehe Abschnitt "Voraussetzungen".

## Lizenz

Dieses Projekt ist Open Source.