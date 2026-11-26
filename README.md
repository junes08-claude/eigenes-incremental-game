# Myzel

Ein Incremental-Game über ein Pilzgeflecht, das unter dem Waldboden wächst.
Du klickst, um Nährstoffe aufzunehmen, baust Hyphen, Fruchtkörper und Pakte mit Bäumen,
entwickelst Mutationen und startest per **Sporenflug** neu, mit dauerhaftem Bonus.

## Spielen

`web/index.html` im Browser öffnen. Keine Installation, keine Abhängigkeiten.
Der Spielstand liegt im `localStorage` des Browsers, im Reiter *Statistik* lässt er sich als Code exportieren.

## Was drin ist

- Klicken für Nährstoffe, 8 Produzenten mit steigenden Kosten (×1.15 pro Kauf), Kaufmengen ×1/×10/Max
- Mutationen: Klick-Boni, Verdopplungen pro Produzent (bei 1/10/25/50/100 Stück), globale Multiplikatoren
- Regentropfen als Zufallsereignis (30 s dreifache Produktion)
- Sporenflug (Prestige): ab 1 Mio. Nährstoffen, jede Spore +10 % Produktion
- Offline-Fortschritt (50 %, max. 8 h), Autosave alle 10 s

## Balancing

Alle Zahlen stehen oben im Script in den Tabellen `GENS`, `UPS` und `TIERS`.
Zum Feintuning reicht es, dort Werte zu ändern.

## Weg zu Steam

Das Spiel ist reines HTML/JS. Für Steam wird es später in eine Desktop-App verpackt,
z. B. mit [Electron](https://www.electronjs.org/) oder [Tauri](https://tauri.app/),
und mit [Steamworks](https://partner.steamgames.com/) (z. B. über `steamworks.js`) für Achievements und Cloud-Saves verbunden.
