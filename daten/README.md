# Streckendaten für die App „Bahn GPS“

Dieser Ordner enthält die Streckendaten, die die App über „Einstellungen → Streckendaten aktualisieren“
herunterladen kann.

- `daten-update.json` – Beschreibung des aktuellen Datenstands (Version, Prüfsumme, Größe), digital
  unterschrieben (Ed25519). Die App übernimmt nur Daten mit gültiger Unterschrift.
- `bahn-ortung-app-<Version>.db` – Streckendatenbank (SQLite).

## Quelle und Lizenz

Streckendaten: © DB InfraGO AG, Infrastrukturdaten (GovData/Mobilithek),
Lizenz [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.de).

Änderungen: Für die App aufbereitet – Streckenabschnitte mit Anfangs- und Endkilometer in eine
SQLite-Datenbank übertragen, für die App nicht benötigte Felder entfernt, exakt doppelte Zeilen
(gleiche Linie für Richtung und Gegenrichtung) entfernt, je Abschnitt ein Begrenzungsrechteck mit
räumlichem Suchindex und die Längenabweichung berechnet. Es wurden keine Daten aus anderen Quellen
hinzugefügt.

Die Daten beschreiben die Streckenachse (Mittellinie zwischen den Gleisen). Sie sind kein Nachweis über
Sicherheitsräume, Zugänge, Betretbarkeit oder betriebliche Verhältnisse.
