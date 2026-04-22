# DB Lab 5 – Gadget-Verwaltung mit Java & Oracle DB

Java-Swing-Anwendung zur Verwaltung und Bewertung von Gadgets. Entwickelt im Rahmen des Datenbank-Praktikums (Labor 5) an der HS Offenburg.

## Funktionen

- Gadgets aus einer Oracle-Datenbank laden und durchblättern (Navigation: First / Prev / Next / Last)
- Gadget-Bilder als BLOB in der Datenbank speichern und anzeigen
- Gadgets suchen, anlegen und löschen
- Nutzer registrieren und einloggen
- Bewertungen und Kommentare zu Gadgets speichern (MERGE INTO)
- Datenbankverbindung über Connection Pool (Apache Commons DBCP2)

## Voraussetzungen

- Java 11+
- Oracle Database XE (lokal auf Port 1521)
- Apache Commons DBCP2 (als Library eingebunden)
- Oracle JDBC Driver (`ojdbc*.jar`)
- IntelliJ IDEA (Projektstruktur vorhanden)

## Konfiguration

Datenbankverbindung in `src/edu/hsog/db/Globals.java` anpassen:

```java
static String url      = "jdbc:oracle:thin:@//localhost:1521/XE";
static String username = "dein_nutzer";
static String passwd   = "dein_passwort";

