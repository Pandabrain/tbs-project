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

Wird online gespielt, können durch Siege und andere Aktionen, wie das zerstören von gegnerischen Spielfiguren, Punkte gesammelt werden. Diese Punkte können die Eigenschaften der eigenen Spielfiguren verbessern. In einem Spiel mit menschlichen Mitspielern muss jedoch eine Option für ein faires Spiel gegeben werden, denn ein/e Spieler/in mit mehr Punkten als seine Mitspieler/innen hätte sonst einen unfairen Vorteil. Die konkrete Umsetzung wird durch das Projketteam während der Umsetzung bestimmt. Eine Möglichkeit wäre, die Progression in einem Spiel nur gegen CPU Gegner nutzen zu können.

- Punkte Vergabe um Einheiten auszuwählen bzw. aufzuwerten

Ein Punkte System soll erstellt werden, durch das ein Spieler vor Beginn eines Spiels seine Spielfiguren kaufen oder aufwerten kann. Durch diese Variation wird der Wiederspielwert der Levels erhöht. Das Feature Player Progression kann hierauf aufbauen und beispielsweise die Menge an zu vergebenden Punkten erhöhen. Das Projektteam muss hierbei während der Entwicklung eine sinnvolle Umsetzug dieses Features bestimmen.

- Felder mit unterschiedlichem Terrain und unterschiedlichen Eignschaften

Felder sollen einem bestimmten Typ angehören und dementsprechende Eigenschaften besitzen. 

Beispiele:

Wald: Verringerte Bewegungsreichweite wenn eine Spielfigur durch dieses Feld bewegt wird. Wird eine hier positionierte Spielfigur angegriffen nimmt sie weniger Schaden. 

Straße: Normale Bewegungsreichweite. Ein Angriff durch den Gegner erfolgt in voller Stärke, wenn die Spielfigur auf diesem Feld attackiert wird.

Krankenhaus: Einheiten, die auf diesem Feld platziert werden, bekommen am Ende der Runde X Gesundheitspunkte zurück.

Die tatsächlich verfügbaren Arten von Terrain, Gebäuden und deren Eigenschaften sollen durch das Projektteam während der Entwicklung sinnvol gewählt werden.


## Nicht-Ziele

- Spiel darf normalen Netzwerkverkehr nicht unnötig stören.
- Spiel darf lokale Ressourcen nicht so stark ausnutzen, dass es die Benutzung des PCs einschränkt.
- Runde darf nicht zu lange dauern um die Mitspieler nicht zu demotivieren.

---

## Projektinhalte

- Spielbrett Erstellung planen (bzw. Framework lernen)
- Spielbrett erstellen
- Spieler Steuerung erstellen/umsetzen
- Kampfsystem erstellen
- Character Eigenschaften erstellen
- Terrain Eigenschaften implementieren
- Spielelogik/Ablauf programmieren (Start/Siegesbedingungen)
- Auswahlmenü (Anzahl Spieler, KI/Mensch, etc.)
- HUD und Statsanzeige der Spielfigueren
- Menü für Character Auswahl
- Menü für Progression
- Menü für online Login
- KI Gegner erstellen
- Current State import/export (Für Savegame und Netzwerk Synchronisation)
- Spiel speichern und laden implementieren
- Laden von unterschiedlichen Maps ermöglichen
- Spielablauf mit Animationen verbessern
- Server: Websocket Kommunikation erstellen
- Server: Datenbank implementieren. (Sqlite für lokalen Service, PostgreSQL für online Server)
- Server: Login erstellen
- Server: Session Handling (Session speichern/laden, 
- Server: Sync bei Client disconnect/reconnect ermöglichen
- Server: Progression speichern
- Client: Kommunikation mit Server implementieren
- Client/Server: Backend als lokalen Service starten, um ohne dedizierten Server ein Netzwerkspiel spielen zu können.
- Server sync: Steigt/fällt der Host aus, soll ein anderer Host übernehmen können.
- Client: Lokales Profil für Player Progression ermöglichen -> Progression lokal speichern (auch wenn online gespielt wurde), aber sync mit lokalen Einträgen und Serverseitiger Plausibilitätsprüfung

---

## Kritische Erfolgsfaktoren

- Ein Spiel muss mit mehreren Spielern lokal spielbar bis zum Ende sein.

## Termine und Meilensteine

**Client:**
- 26.02.2023 Proof of concept Build fertiggestellt. (Durch Framework bereitgestelltes Grundgerüst eingesetzt.)
- 26.03.2023 Grundlegendes Gameplay fertig gestellt: Eigenschaften der Spielfiguren und des Terrains implementiert, Kampsystem einsetzbar. 
- 16.04.2023 Alpha Version: Spiel grundlegend spielbar: Menüs und HUD existieren, Sigesbedingung ist implementiert, Player Progression ist implementiert.
- 14.05.2023 Spiel gegen KI Gegner möglich. Speichern und laden möglich.
- 28.05.2023 Spiel fertig gestellt. Es gibt unterschiedliche Maps/Level zur Auswahl.

**Server:**
- 19.02.2023 Client kann mit Server kommunizieren. Datenbankgrundgerüst aufgebaut.
- 19.03.2023 Spielzüge werden zwischen Clients kommuniziert.
- 09.04.2023 Profilverwaltung fertig. Spieler können sich registrieren, anmelden und ihr Fortschritt wird online synchronisiert.
- 07.05.2023 Online Spielesessions sind vollständig implementiert: Spiele können online gespeichert und fortgesetzt werden. Ausfallende Teilnehmer können  wiedereinsteigen.
- 04.06.2023 Client zu Client Verbindung fertiggestellt. Spiel kann ohne dedizierten Server über Netzwerk gespielt werden.

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

Aufgabenbereiche:
Entwicklung des Unity Game Clients: Bammer Bernhard, Qi Tong Zheng
Entwicklung des Server Backends sowie Implementierung der Serverkommunikation im Client: Christoph Rechtlehner
Level und Game Design: Bammer Bernhard, Qi Tong Zheng, Christoph Rechtlehner  
