# Projekt: TBSP - Turn Based Strategy Project (Working Title)

## Ausgangssituation

Wir sollen ein Softwareprojekt planen und umsetzen. Dadurch üben wir folgendes:
Die Planung eines Projekts und die Nutzung unserer Projektmanagement Tools.
Die dabei gewonnene Erfahrung soll uns für unsere künftige Diplomarbeit unterstützen.

---

## Projektziele

TBSP ist ein typisches rundenbasiertes Strategiespiel. Das heißt, dass die Karte wie ein Schachbrett in einzelne Felder unterteilt ist, und die Mitspieler/innen reihum abwechselnd zum Zug kommen. Ist ein/e Spieler/in an der Reihe, kann er/sie (optional) beliebig viele seiner/ihrer Figuren bewegen und (ebenfalls optional) eine Aktion der Figur starten. Aktionen können Angriffe sein, aber auch eine unterstützende Leistung (z.B. Heilung). Nach einer Aktion kann die Spielfigur, die die Aktion ausgeführt hat, nicht mehr bewegt werden. Die Bewegungs- und Angriffsreichweite ist von den Eigenschaften der jeweiligen Figur abhängig, aber auch von den Eigenschaften des Feldes, das für die Aktion relevant ist. So ermöglicht ein Feld vom Typ Straße, eine höhere Reichweite, als beispielsweise ein Feld vom Typ Wald. Allerdings nimmt  eine Spielfigur weniger Schaden, wenn diese auf einem Feld vom Typ Wald attackiert wird, da, wie in der echten Welt, ein Wald Schutz vor gegnerischen Pfeilen bieten kann.
Ziel des Spiels ist es, die vom Level vorgegebenen Einheiten des/der Gegners/Gegnerin zu zerstören.
Das Spiel soll folgende Features unterstützen:

- Lokales Spiel mit mehreren Spielern
Ein Spiel soll, von mehreren Spielern/Spielerinnen, am selben PC gespielt werden können. Da die Spieler/innen abwechselnd an der Reihe sind, kann die Steuerung einfach an die Mitspieler/innen abgegeben werden.

- Lokales Spiel mit KI-Gegnern
Beliebig viele Mitspieler/innen sollen durch eine/n vom PC gesteuerte/n Mitspieler/in ersetzt werden können.

- Multiplayerspiele über Netzwerk (über dedizierten Server)
Ein Spiel soll über einen dedizierten Server miteinander spielbar sein. D.h. Spieler/innen können mit ihrem PC online an einem Match teilnehmen.

- Savegame Management (Spiel laden/speichern)
Der aktuelle Stand eines Spiels, (Position und HP der Spielfiguren, etc.) soll auf der Festplatte gespeichert, und zu einem späteren Zeitpunkt wieder fortgesetzt werden können.

- Unterschiedliche Anzahl Spieler/innen
Ein Spiel muss von mindestens 2 Spielern/Spielerinnen (egal ob Mensch oder CPU gesteuert) gespielt werden. Die maximale Anzahl an Mitspieler/innen wird durch den gespielten Level bestimmt.

- Verschiedene Maps
Es soll möglich sein, unterschiedliche Level/Maps zu spielen. Diese können sich durch Größe, Terrain und Maximale Spieleranzahl unterscheiden.

- Player/Character Progression
Wird online gespielt, werden Charactere 

- Punkte Vergabe um Einheiten auszuwählen bzw. aufzuwerten
- Felder mit unterschiedlichem Terrain und unterschiedlichen Eignschaften

{Meilensteine mit Terminen.)

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
