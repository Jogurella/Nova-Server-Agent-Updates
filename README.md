# Nova Server Agent – Updates

Öffentliche Updatepakete und Prüfsummen für Nova Server Agent.

## Client und Connector online aktualisieren

1. Im Client **Reparaturen & Updates → Nova Server Agent aktualisieren** öffnen.
2. Bei der gewünschten Komponente **Quelle & Kanal** wählen und `Jogurella/Nova-Server-Agent-Updates` eintragen. Client und Connector haben getrennte Einstellungen.
3. Kanal **Stabil**, **Beim Start und alle 6 Stunden prüfen** aktivieren, Quelle bestätigen und speichern.
4. **Jetzt prüfen** bzw. ab 0.7.15 **Update prüfen** bei der jeweiligen Komponente wählen und das Update bestätigen.

Die Einstellung **Neue Versionen automatisch installieren** ist optional. Kopplungen und persönliche Einstellungen bleiben beim Update erhalten.

## Version 0.7.15

- Maximierte Client- und Connector-Fenster respektieren die Monitor-Arbeitsfläche und die Taskleiste.
- Client- und Connector-Updateprüfungen arbeiten unabhängig; Fehler eines Connectors verdecken kein Clientupdate.
- Eigene Prüfschaltflächen, sichtbarer Aktivierungsstatus und sofortige Prüfung nach dem Speichern der Quelle.
- Die Flackerkorrekturen aus 0.7.14 bleiben enthalten: bestehende Anzeigen, Scrollpositionen, Eingaben und Details bleiben bei Statusabfragen erhalten.

Der Connector wird über seine geschützte Softwarepipeline mit Sicherung und Rückfall aktualisiert. Der Windows-Dienst wechselt dabei kurz. Ein Minecraft-Neustart ist für dieses Programmupdate nicht vorgesehen; Wartungs- und Spielerprüfungen bleiben wirksam.

## Dateien

- `ServerAgent-client-win-x64.zip`: Clientpaket mit `update.json` und SHA-256 je Datei.
- `ServerAgent-connector-win-x64.zip`: Connectorpaket mit `update.json` und SHA-256 je Datei.
- `SHA256SUMS`: SHA-256 der veröffentlichten Pakete.
- `Nova-Server-Agent-Client-Setup-0.7.15-2026-10-31.exe`: vollständiger Clientinstaller; kann auch eine ältere Installation bei Problemen mit deren Updateprüfung aktualisieren.

[Aktuelles Release und Downloads](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/latest)
