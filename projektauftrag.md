# Projekt: TBSP - Turn Based Strategy Project (Working Title)

## Ausgangssituation

Wir sollen ein Softwareprojekt planen und umsetzen. Dadurch üben wir folgendes:
Die Planung eines Projekts und die Nutzung unserer Projektmanagement Tools.
Die dabei gewonnene Erfahrung soll uns für unsere künftige Diplomarbeit unterstützen.

---

## Projektziele

Ein rundenbasiertes Strategiespiel:
{Beschreibung des Spiels hier einfügen}

- Lokales Spiel mit mehreren Spielern
- Lokales Spiel mit KI-Gegnern
- Multiplayerspiele über Netzwerk (Client zu Client Verbindung, ohne dedizierten Server)
- Savegame Management (Spiel laden/speichern)
- Unterschiedliche Anzahl Spieler
- Verschiedene Maps
- Player/Character Progression
- Punkte Vergabe um Einheiten auszuwählen bzw. aufzuwerten
- Felder mit unterschiedlichem Terrain und unterschiedlichen Eignschaften

## Nicht-Ziele

- Spiel darf normalen Netzwerkverkehr nicht unnötig stören.
- Spiel darf lokale Ressourcen nicht so stark ausnutzen, dass es die Benutzung des PCs einschränkt.
- Spiel darf nicht zu lange dauern.

---

## Projektinhalte

- Spielbrett Erstellung planen (Framework oder selbst machen)
- Spielbrett erstellen
- Spieler Steuerung erstellen/umsetzen
- Kampfsystem erstellen
- Character Eigenschaften erstellen
- Terrain Eigenschaften implementieren
- Spielelogik/Ablauf programmieren (Start/Siegesbedingungen)
- Auswahlmenü (Anzahl Spieler, KI/Mensch, etc.)
- Menü für Character Auswahl
- Menü für Progression
- Menü für online Login
- KI Gegner erstellen
- Current State import/export (Für Savegame und Netzwerk Synchronisation)
- Spiel speichern und laden implementieren
- Server: Websocket Kommunikation erstellen
- Server: Session Handling
- Server: Login erstellen
- Server: Progression speichern
- Client: Kommunikation mit Server implementieren
- Laden von unterschiedlichen Maps ermöglichen
- Spielablauf mit Animationen verbessern

---

## Kritische Erfolgsfaktoren

- Ein Spiel muss mit mehreren Spielern lokal spielbar bis zum Ende sein.

## Termine

- Projektende: **genaues Datum unbekannt**

---

## Kosten

- TBS Framework: ? €
- Map Design Assets: ? €
- Figuren Assets: ? €

Verwendete Technologien: C#, Unity Engine, Go
Verwendete Werkzeuge: Visual Studio, Goland, Rider, Unity.

---

## Projektorganisation

| **Projektauftraggeber**   | **Projektleiter**                 |
| :------------------------ | :-------------------------------- |
| David Klewein             | Christoph Rechtlehner             |
| **Projektteammitglieder** | **Punktuelle Projektmitarbeiter** |
| Bammer Bernhard           |                                   |
| Qi Tong Zheng             |                                   |
| Christoph Rechtlehner     |                                   |
