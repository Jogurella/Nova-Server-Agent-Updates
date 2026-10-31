# Nova Server Agent – Updates

Öffentliche Updatepakete und Prüfsummen für Nova Server Agent.

## Windows-Client online aktualisieren

1. Im Client **Reparaturen & Updates → Nova Server Agent aktualisieren** öffnen.
2. Beim **Windows-Client → Quelle & Kanal** das Repository `Jogurella/Nova-Server-Agent-Updates` eintragen.
3. Kanal **Stabil**, **Beim Start und alle 6 Stunden prüfen** aktivieren und die Quelle speichern.
4. **Jetzt prüfen** und das angebotene Clientupdate bestätigen.

Die Einstellung **Neue Versionen automatisch installieren** ist optional. Die Kopplung und die persönlichen Einstellungen bleiben beim Update erhalten.

## Version 0.7.14

Die Oberfläche aktualisiert bestehende Anzeigen an Ort und Stelle. Ladeabfragen starten die Einblendanimationen bereits sichtbarer Listen nicht erneut. Scrollpositionen, Eingaben und aufgeklappte Details bleiben erhalten. Auch bei langsamen oder fehlgeschlagenen Abfragen bleiben die bisherigen Daten sichtbar.

Das Release enthält ein Windows-Clientupdate. Der bereits laufende Connector liefert weiter die Serverdaten. Für das Clientupdate ist kein Neustart eines Minecraft-Servers nötig.

## Dateien

- `ServerAgent-client-win-x64.zip`: Paket für den eingebauten Clientupdater, mit `update.json` und SHA-256 je Datei.
- `SHA256SUMS`: SHA-256 der veröffentlichten Pakete.
- `Nova-Server-Agent-Client-Setup-0.7.14-2026-10-31.exe`: vollständiger Clientinstaller für Windows x64.

[Releases und Downloads](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases)
