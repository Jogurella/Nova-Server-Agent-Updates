# Nova Server Agent – Updates

Öffentliche Windows-Updatepakete, Setups und Prüfsummen für Nova Server Agent.

**Aktueller Prüfstand:** 0.7.17 wird zunächst als Prüfversion bereitgestellt. 0.7.16 wurde nach einem im Liveversuch gefundenen Dienstwechsel-Fehler als Pre-Release zurückgestellt. Der stabile Kanal bleibt bis zur abgeschlossenen Liveabnahme bei 0.7.15. Eine bestandene isolierte Prüfung ist kein Nachweis einer Installation auf einem anderen PC.

## Windows-Client aktualisieren

1. **Reparaturen & Updates → Windows-Client aktualisieren → Quelle & Kanal** öffnen. Bei älteren Clients heißt der Bereich **Nova Server Agent aktualisieren → Windows-Client**.
2. Repository `Jogurella/Nova-Server-Agent-Updates`, Kanal **Stabil** und die regelmäßige Prüfung aktivieren, Quelle bestätigen und speichern.
3. **Jetzt prüfen** wählen und das im gewählten Kanal freigegebene Clientupdate bestätigen.

Die neue Oberfläche zeigt ausschließlich Clientupdates. Standardmäßig erscheint die neueste passende, noch nicht installierte Version. Weitere Versionen und der begrenzte Updateverlauf lassen sich aufklappen beziehungsweise filtern. Falls ein alter Client weiterhin kein Update findet, kann das vollständige Client-Setup aus dem jeweiligen Release die vorhandene Installation aktualisieren. Kopplungen und Einstellungen bleiben erhalten.

## Connector aktualisieren

Die Connectorquelle wird separat am Server-PC eingerichtet. Die neue Connector-Statusanzeige besitzt den Bereich **Connectorupdates**. Dort dasselbe Repository wählen und eine automatische Quelle bewusst aktivieren. Dadurch werden weder KI-Autonomie noch zusätzliche KI-Rechte eingeschaltet.

Für den ersten Wechsel aus einem älteren Connector alle **Nova-Clients über ihr Infobereich-Menü → Beenden** und die alte **Connector-Statusanzeige → Statusanzeige beenden** vorübergehend schließen. **Minecraft bleibt geöffnet.** Der bisher installierte Updatehelfer ist bis zum ersten erfolgreichen Wechsel noch aktiv. Ist der Connector-Dienst nach einem vorherigen Fehlversuch bereits gestoppt, muss ausschließlich dieser eigene Dienst mit Windows-Administratorrechten wieder gestartet werden. Dafür ist kein Minecraft-Starttask erforderlich.

Die geschützte Softwarepipeline sichert die Programmdateien, prüft das Paket und verwendet die Brokerübergabe. Laufende Wartungsaufträge und Not-Aus bleiben Sperren. Eine aktivierte automatische Quelle kann anschließend freigegebene neue Connectorversionen selbst installieren.

## Version 0.7.17 – Prüfversion

- Offene WSS-Sitzungen werden beim Beginn des Host-Shutdowns beendet; der Updatehelfer wartet länger als das maximal erlaubte Hostbudget.
- Dienststeuerung bindet die konkrete Programmdatei, Konfiguration und ursprüngliche PID samt Geburtszeit.
- Bereits begonnene oder unklare Dienststopps behalten das Broker-Ticket; ein später Helferfehler darf es nicht versehentlich freigeben.
- Begrenzte, scrollbar dargestellte Update- und Suchlisten mit Versions-, Namens-, Ordner- und Statusfiltern.
- Bestehende Anzeigen, Fokus, Eingaben, Details und Scrollpositionen bleiben beim Aktualisieren erhalten.
- Beobachtete Server zeigen die geprüfte tatsächliche Instanz und Umgebung. Abgelaufene Zuordnungen erscheinen ausdrücklich ungeprüft.
- Neue Minecraft-Chatzeilen werden ereignisgesteuert über die authentifizierte Verbindung übertragen; der Client hält höchstens 300 Zeilen und ergänzt den Stand nach einer Wiederverbindung.
- Die Taskleisten- und Maximierungskorrekturen bleiben enthalten.

Passive Beobachtung ist keine vollständige Prozesssteuerung. Spielerchat bleibt unbestätigter Text ohne Befehlswirkung. Das Programmupdate aktiviert weder eine externe Serversteuerung noch eine Chatvorstellung und beauftragt keinen Minecraft-Stopp oder -Neustart.

## Dateien

- `ServerAgent-client-win-x64.zip`: Paket für den eingebauten Clientupdater.
- `ServerAgent-connector-win-x64.zip`: Paket für den eingebauten Connectorupdater.
- `SHA256SUMS`: SHA-256 der veröffentlichten Pakete und Setups; die ZIP-Manifeste enthalten zusätzlich SHA-256 je Datei.
- `Nova-Server-Agent-Client-Setup-0.7.17-2026-10-31.exe`: vollständiges Client-Setup dieser Prüfversion.
- `Nova-Server-Agent-Connector-Setup-0.7.17-2026-10-31.exe`: vollständiges Connector-Setup dieser Prüfversion.

[Prüfversion 0.7.17](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/tag/v0.7.17) · [Stabiler Kanal](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/latest)
