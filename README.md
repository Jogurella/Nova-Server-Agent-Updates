# Nova Server Agent – Updates

Öffentliche Windows-Updatepakete, Setups und Prüfsummen für Nova Server Agent.

## Windows-Client aktualisieren

1. **Reparaturen & Updates → Windows-Client aktualisieren → Quelle & Kanal** öffnen. Bei älteren Clients heißt der Bereich **Nova Server Agent aktualisieren → Windows-Client**.
2. Repository `Jogurella/Nova-Server-Agent-Updates`, Kanal **Stabil** und die regelmäßige Prüfung aktivieren, Quelle bestätigen und speichern.
3. **Jetzt prüfen** wählen und das angebotene Clientupdate bestätigen.

Ab 0.7.16 zeigt der Client ausschließlich Clientupdates. Standardmäßig erscheint die neueste Paketversion. Weitere Versionen und der begrenzte Updateverlauf lassen sich aufklappen beziehungsweise filtern. Falls ein alter Client weiterhin kein Update findet, kann das vollständige Client-Setup aus dem Release die vorhandene Installation aktualisieren. Kopplungen und Einstellungen bleiben erhalten.

## Connector aktualisieren

Die Connectorquelle wird separat am Server-PC eingerichtet. Ab 0.7.16 besitzt die Connector-Statusanzeige den Bereich **Connectorupdates**. Dort dasselbe Repository und **Stabil** wählen und **Automatisch aktualisieren** bewusst aktivieren. Dadurch wird keine KI-Autonomie eingeschaltet und es werden keine zusätzlichen KI-Rechte vergeben.

Für ein erstes Update von Connector 0.7.12 dessen alte **Statusanzeige** über das Nova-Symbol im Infobereich → **Statusanzeige beenden** schließen. Der Dienst und Minecraft sollen dabei weiterlaufen. Das Update kann über die bisherige Connector-Updatefunktion eines älteren Clients oder über das vollständige Connector-Setup erfolgen. Die neue Statusanzeige hat anschließend ihre eigene Updatebedienung.

Die geschützte Softwarepipeline sichert die Programmdateien, prüft das Paket und verwendet die Brokerübergabe. Der Connector-Dienst wechselt kurz; ein Minecraft-Stopp oder -Neustart wird für das Programmupdate nicht beauftragt. Laufende Wartungsaufträge und Not-Aus bleiben Sperren. Eine aktivierte Automatik kann zukünftige neue Connectorversionen selbst installieren.

## Version 0.7.16

- Begrenzte, scrollbar dargestellte Update- und Suchlisten mit Versions-, Namens-, Ordner- und Statusfiltern.
- Bestehende Anzeigen, Fokus, Eingaben, Details und Scrollpositionen bleiben beim Aktualisieren erhalten.
- Beobachtete Server zeigen die geprüfte tatsächliche Instanz und Umgebung. Abgelaufene Zuordnungen erscheinen ausdrücklich ungeprüft.
- Neue Minecraft-Chatzeilen werden ereignisgesteuert über die authentifizierte Verbindung übertragen; der Client hält höchstens 300 Zeilen und ergänzt den Stand nach einer Wiederverbindung.
- Die Taskleisten- und Maximierungskorrekturen aus 0.7.15 sind enthalten.

Passive Beobachtung ist keine vollständige Prozesssteuerung. Spielerchat bleibt unbestätigter Text ohne Befehlswirkung. Das Programmupdate aktiviert weder eine externe Serversteuerung noch eine Chatvorstellung.

## Dateien

- `ServerAgent-client-win-x64.zip`: Paket für den eingebauten Clientupdater.
- `ServerAgent-connector-win-x64.zip`: Paket für den eingebauten Connectorupdater.
- `SHA256SUMS`: SHA-256 der veröffentlichten Pakete und Setups; die ZIP-Manifeste enthalten zusätzlich SHA-256 je Datei.
- `Nova-Server-Agent-Client-Setup-0.7.16-2026-10-31.exe`: vollständiges Client-Setup.
- `Nova-Server-Agent-Connector-Setup-0.7.16-2026-10-31.exe`: vollständiges Connector-Setup für Einrichtung beziehungsweise Aktualisierung.

[Aktuelles Release und Downloads](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/latest)
