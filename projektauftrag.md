# Projekt: TBSP - Turn Based Strategy Project (Working Title)

## Ausgangssituation

Wir sollen ein Softwareprojekt planen und umsetzen. Dadurch üben wir folgendes:
Die Planung eines Projekts und die Nutzung unserer Projektmanagement Tools.
Die dabei gewonnene Erfahrung soll uns für unsere künftige Diplomarbeit unterstützen.

---

## Projektziele

TBSP ist ein typisches rundenbasiertes Strategiespiel. Das heißt, dass die Karte wie ein Schachbrett in einzelne Felder unterteilt ist, und die Mitspieler/innen reihum abwechselnd zum Zug kommen. Ist ein/e Spieler/in an der Reihe, kann er/sie (optional) beliebig viele seiner/ihrer Figuren bewegen und (ebenfalls optional) eine Aktion der Figur starten. Aktionen können Angriffe sein, aber auch eine unterstützende Aktion (z.B. Heilung). Nach einer Aktion kann die Spielfigur, die die Aktion ausgeführt hat, nicht mehr bewegt werden. Die Bewegungs- und Angriffsreichweite ist von den Eigenschaften der jeweiligen Figur abhängig, aber auch von den Eigenschaften des Feldes, das für die Aktion relevant ist. So ermöglicht ein Feld vom Typ Straße, eine höhere Reichweite, als beispielsweise ein Feld vom Typ Wald. Allerdings nimmt  eine Spielfigur weniger Schaden, wenn diese auf einem Feld vom Typ Wald attackiert wird, da, wie in der echten Welt, ein Wald Schutz vor gegnerischen Pfeilen bieten kann.
Ziel des Spiels ist es, die vom Level vorgegebenen Einheiten des Gegners zu zerstören.

{Projektbeschreibung fertigstellen.}
{Meilensteine mit Terminen.)

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
