# Nova Server Agent – Updates

Öffentliche Windows-Updatepakete, Setups und Prüfsummen für Nova Server Agent.

**Windows-Client: 0.7.20 · Connector: 0.7.19.** Die Fensterkorrektur ist ein eigenständiges Clientupdate; der Connector bleibt bei der bereits live abgenommenen Version 0.7.19. Die Zwischenversionen 0.7.16–0.7.18 bleiben historische Prüfversionen.

## Windows-Client aktualisieren

1. **Reparaturen & Updates → Windows-Client aktualisieren → Quelle & Kanal** öffnen. Bei älteren Clients heißt der Bereich **Nova Server Agent aktualisieren → Windows-Client**.
2. Repository `Jogurella/Nova-Server-Agent-Updates`, Kanal **Stabil** und die regelmäßige Prüfung aktivieren, Quelle bestätigen und speichern.
3. **Jetzt prüfen** wählen und das Update auf **0.7.20** bestätigen.

Der Client zeigt ausschließlich Client-Softwareupdates. Standardmäßig erscheint die neueste passende, noch nicht installierte Version. Ältere Versionen sind über **Alle Versionen** erreichbar; bereits installierte oder ältere Pakete werden nicht als neues Installationsangebot dargestellt. Paketlisten sind scrollbar begrenzt, Verläufe standardmäßig eingeklappt und neueste Einträge zuerst sortiert. Auch im gemeinsamen Serverpakete-Eingang erscheinen keine Connector-Softwarepakete.

Das Clientupdate muss auf dem jeweiligen Client-PC installiert werden. Falls dessen alte Updateprüfung nicht funktioniert, kann das vollständige Client-Setup aus diesem Release die vorhandene Installation aktualisieren. Kopplungen und Einstellungen bleiben erhalten.

## Connector aktualisieren

Die Connectorquelle wird separat am Server-PC unter **Connectorupdates** eingerichtet. Dort dasselbe Repository, Kanal **Stabil**, regelmäßige Prüfung und die gewünschte Automatik wählen. Eine bewusst aktivierte automatische Quelle schaltet keine KI-Autonomie oder zusätzlichen KI-Rechte ein.

Die geschützte Softwarepipeline sichert die Programmdateien, prüft das Paket und übergibt laufende Spielprozesse geordnet. Der Connector-Dienst wechselt kurz; das Programmupdate beauftragt keinen Minecraft-Stopp oder -Neustart. Laufende Wartungsaufträge und Not-Aus bleiben Sperren. Die tatsächlich durchgeführte automatische Aktualisierung wurde mit offener authentifizierter Liveverbindung und unveränderter Minecraft-Instanz geprüft.

Beim ersten Wechsel aus einem alten Connector die **Nova-Clients über das Infobereich-Menü → Beenden** und dessen alte **Statusanzeige → Statusanzeige beenden** vorübergehend schließen. **Minecraft bleibt geöffnet.** Ist der eigene Connector-Dienst nach einem älteren Fehlversuch bereits gestoppt, benötigt ausschließlich dessen Wiederstart gegebenenfalls Windows-Administratorrechte. Dafür keinen Minecraft-Starttask ausführen.

## Windows-Client 0.7.20

- Der Fensterinhalt passt zur nativen Außenkante: keine zweite eingerückte Rundung und kein dunkler Doppelrand.
- Maximiert schließt die Oberfläche bündig ab; die Taskleiste bleibt berücksichtigt.
- Wiederherstellen und Größenänderung über die Fensterecken bleiben bedienbar. Die Startanimation hinterlässt keine ausgeschnittenen Ecken.

Geprüft: 92 veröffentlichte Client-/UI-Prüfungen, 37 native Client-Installerprüfungen und sämtliche 697 Nutzdateien mit dem ursprünglichen Updateleser 0.7.12. Dieses Release enthält ausschließlich Clientpaket, Client-Setup und Prüfsummen. Der Connectorupdater überspringt es und verwendet weiterhin das separate Connectorrelease 0.7.19.

## Version 0.7.19

- Anzeigen und Listen bleiben während langsamer oder fehlgeschlagener Statusabfragen erhalten; Eingaben, Fokus, Details und Scrollpositionen werden bewahrt.
- Die Serversuche besitzt eine begrenzte Trefferliste mit Namens-, Ordner- und Statusfiltern.
- Beobachtete laufende Server zeigen die geprüfte tatsächliche Instanz und Umgebung; abgelaufene Zuordnungen erscheinen ungeprüft.
- Neue Minecraft-Chatzeilen werden über Dateisystemereignisse und die authentifizierte Liveverbindung übertragen. Mehrteilige Ranglabels, Unicode und ranglose Namen bleiben im selben Verlauf erhalten. Maximal 300 Zeilen, mit Ergänzung nach einer Wiederverbindung.
- Maximierte Fenster berücksichtigen die Arbeitsfläche des Monitors und die Taskleiste.

Ranglabels und Spielerchat bleiben unbestätigter Klartext ohne Befehlswirkung oder UUID-Rollen. Passive Beobachtung ist keine vollständige Prozesssteuerung. Externe Serversteuerung und Chatvorstellung werden durch dieses Programmupdate nicht aktiviert.

Geprüft: 343 Infrastruktur-, 95 Refresh-/Update-/Livechat-Browser-, 80 Software-/Broker-, 92 veröffentlichte Client-/UI- und 46 Desktopprüfungen. Beide Installer einschließlich 55 Reparatur- und 37 nativer Client-Installerprüfungen bestanden. Alle elf Clientreiter wurden zusätzlich am tatsächlichen Connector geöffnet; Serverumgebung, Rangchat, Filter, Wiederverbindung und Fenstersteuerung wurden live abgenommen. Die neue echte Spielnachricht wurde im unveränderten Chatpfad von 0.7.18 mit rund 272 ms vom Logdatei-Ereignis bis zum Liveempfänger gemessen; der isolierte 100-Zeilen-Burst kam vollständig in 372 ms an. Dies misst keine Zeit vom Tastendruck bis zur Anzeige.

Beide öffentlichen ZIP-Downloads wurden mit dem ursprünglichen 0.7.12-Updater vollständig validiert: 696 Client- und 1.895 Connectordateien. Der stabile Kanal bietet dieselben geprüften Paketdateien auch den Versionen 0.7.12 und 0.7.14 an.

## Dateien

- `ServerAgent-client-win-x64.zip`: Paket für den eingebauten Clientupdater.
- `ServerAgent-connector-win-x64.zip`: Paket für den eingebauten Connectorupdater.
- `SHA256SUMS`: SHA-256 der veröffentlichten Pakete und Setups; die ZIP-Manifeste enthalten zusätzlich SHA-256 je Datei.
- `Nova-Server-Agent-Client-Setup-0.7.20-2026-11-01.exe`: vollständiges Client-Setup.
- `Nova-Server-Agent-Connector-Setup-0.7.19-2026-10-31.exe`: vollständiges Connector-Setup.

[Client 0.7.20](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/tag/v0.7.20) · [Connector 0.7.19](https://github.com/Jogurella/Nova-Server-Agent-Updates/releases/tag/v0.7.19)
