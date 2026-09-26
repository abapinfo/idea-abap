# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Integrierte Entwicklungsumgebung für ABAP

[Español](README.md) · [English](README.en.md) · **Deutsch** · [Français](README.fr.md)

> 💡 Um dieses README in einer anderen Sprache in VS Code zu lesen, führen Sie **IDEA: README anzeigen** (`Ctrl+Shift+P`) aus: Es öffnet sich automatisch in der Sprache Ihres Editors.

---

## Moderne ABAP-Entwicklung, ohne VS Code zu verlassen

**IDEA** macht Visual Studio Code zu einer vollständigen ABAP-Entwicklungsumgebung: in Echtzeit mit Ihrem SAP-System verbunden und bereit, Seite an Seite mit dem KI-Assistenten zu arbeiten, den Sie bereits nutzen (Claude Code, GitHub Copilot, Cursor…).

Schluss mit dem Kopieren und Einfügen von Code zwischen SAP GUI und einem KI-Chat. Schluss damit, den Überblick zu verlieren, welches Objekt gesperrt ist, wer es geändert hat oder ob es noch auf die Aktivierung wartet. Mit IDEA passiert alles direkt im Editor, mit derselben Disziplin bei Sperren, Transportaufträgen und Aktivierung, die Sie aus SAP kennen — aber mit der Geschwindigkeit von VS Code und der Leistung der KI.

**In einem Satz:** Objekt suchen → öffnen → Ihre KI bitten, es zu ändern (oder selbst bearbeiten) → aktivieren. Alles ohne VS Code zu verlassen, alles unter Kontrolle.

**In einem anderen Satz 😉:** Ein IDoc ist fehlgeschlagen? → Ihre KI bitten, es zu analysieren und die Lösung zu nennen → beheben. Alles ohne VS Code zu verlassen, alles unter Kontrolle.

---

## Warum Ihr Team es lieben wird

| | |
|---|---|
| ⚡ **Echte Geschwindigkeit** | Sofortige Suche nach Programmen, Klassen, Interfaces und Dictionary-Objekten, mit Suchverlauf. Ohne Transaktionen oder verschachtelte Menüs. |
| 🤖 **KI mit direktem Zugriff auf SAP** | Integrierter MCP-Server: Ihr KI-Assistent liest, schreibt und aktiviert ABAP-Code direkt in SAP und zeigt vor jeder Änderung immer einen Bestätigungs-Diff. |
| 🌐 **Mehrere Systeme** | Mehrere MCP-Server gleichzeitig, einer pro System: Ihre KI kann in DEV schreiben, während sie über eine schreibgeschützte Verbindung Daten in PRD abfragt. |
| 🔒 **Keine Überraschungen** | Standardmäßig Anzeigemodus, explizite Sperre zum Bearbeiten, Transportaufträge und Aktivierung genau wie im SAP-Standard. |
| 🕘 **Verlauf im Handumdrehen** | Jedes Speichern und jede Aktivierung wird in der Sitzung festgehalten: Versionen vergleichen oder eine frühere wiederherstellen, ohne den Editor zu verlassen. |
| 🎨 **Formatierung, die Ihre Diffs respektiert** | Eigener Formatierer, der nur die vom Entwickler geänderten Zeilen anfasst — kein versehentliches Umformatieren ganzer Dateien. |
| 🖥️ **Quelltext-Editor wie in der SAP GUI** | In den Tab eingebetteter Editor: Anzeige- oder Bearbeitungsmodus, Klassen blockweise oder vollständig, bearbeitbare Beschreibungen, direkte Navigation zu REPT/CUA/Dynpros und lokalen Includes, sowie volle Kontrolle über die Wartezeiten gegenüber SAP. |
| 🧩 **Mehr als Standard-ADT** *(erweiterte Funktion)* | Bearbeitung von Textelementen (REPT), Data Dictionary, GUI-Status/-Titel und Dynpros — alles, was das SAP-ADT außerhalb der SAP GUI nicht bearbeiten lässt. |

---

## So funktioniert es

1. **Richten Sie Ihre SAP-Verbindungen ein** mit `IDEA: SAP-Verbindungen verwalten` — Definieren Sie alle Verbindungen zu den SAP-Systemen, mit denen Sie arbeiten möchten, damit Sie im KI-Chat angeben können, gegen welche Umgebung gearbeitet werden soll; beim Start von VS Code werden die MCP-Server für jedes System verbunden (das bewirkt nichts in den Systemen, der MCP-Server lauscht lediglich). Legen Sie eine der Verbindungen so fest, dass sie mit VS Code automatisch startet.
2. **Suchen Sie das Objekt**, das Sie brauchen, im Seitenbereich «IDEA».
3. **Bitten Sie Ihre KI**, es zu ändern, oder bearbeiten Sie es selbst mit Autovervollständigung, Formatierung und Navigation zur Definition.
4. **Aktivieren Sie es per Tastenkürzel** (`Ctrl+F3`). IDEA kümmert sich um Sperre, Transportauftrag und Aktivierung.

Sie müssen das Objekt nicht manuell öffnen, bevor Sie Ihre KI um etwas bitten: Bei aktiver MCP-Verbindung kann sie es selbst suchen, lesen und direkt in SAP ändern.

> Damit Ihre KI das volle Potenzial von IDEA nutzt, bitten Sie sie ausdrücklich, die MCP-Werkzeuge von IDEA zum Lesen und Schreiben in SAP zu verwenden, statt das Objekt im Editor von Hand zu bearbeiten.

---

## Anzeigemodus / Bearbeitungsmodus

Aus der «SAP-Objektsuche» geöffnete Objekte starten im **Anzeigemodus** (bläulicher Hintergrund): Sie sperren das Objekt in SAP nicht und verhindern versehentliches Tippen.

1. `Ctrl+F1` wechselt in den **Bearbeitungsmodus**: sperrt das Objekt in SAP.
2. Bearbeiten und speichern mit `Ctrl+S`; jedes Speichern im Bearbeitungsmodus lädt den Code auch nach SAP hoch.
3. `Ctrl+F3` formatiert und aktiviert das Objekt.
4. Erneut `Ctrl+F1` oder `Ctrl+Shift+U` zum Verwerfen der Änderungen kehrt in den Anzeigemodus zurück und gibt die Sperre frei. Auch das Schließen des Tabs gibt die Sperre frei.

Ein 🔴-Symbol auf dem Tab weist darauf hin, dass gespeicherte Änderungen noch aktiviert werden müssen.

---

## WebView-Quelltexteditor: wie in der SAP GUI, aber in VS Code

Ein Quelltext-Editor, der direkt im Tab eingebettet ist, mit derselben Engine, die auch VS Code selbst verwendet (Monaco), und darauf ausgelegt, gegen SAP genau wie in SE24/SE38 zu arbeiten – mit viel Bedienkomfort direkt zur Hand.

**Klassen bearbeiten wie in der SAP GUI**
- **Vollständiger Quelltext oder blockweise**: wechseln Sie zwischen der vollständigen Klasse oder nur der Methode, die Sie interessiert, mit ihrer *Deklaration* oben und ihrer *Implementierung* unten, beide bearbeitbar und mit demselben Bildlauf — genau wie in SE24.
- **Beschreibungen**: bearbeiten Sie in einer eigenen Tabelle die Kurztexte von Attributen, Typen, Methoden, Ereignissen und Parametern der Klasse oder des Interfaces, ohne den Editor zu verlassen; sie werden zusammen mit dem übrigen Quelltext gespeichert.
- **Schaltfläche Navigieren**: springt direkt zu den Textelementen (REPT), zum GUI-Status/-Titel (CUA) und zu den Dynpros des Objekts sowie zu den lokalen Includes der Klasse — Definitionen (`CCDEF`), Implementierungen (`CCIMP`), Makros (`CCMAC`) und ABAP-Unit-Testklassen (`CCAU`) —, jedes in seinem eigenen Tab.

**Volle Kontrolle über die Wartezeiten gegenüber SAP**
- Während gegen SAP gesperrt, gespeichert, aktiviert oder formatiert wird, sperrt sich der gesamte Editor (eine Ebene zeigt an, was gerade geschieht), damit Sie nicht weiterschreiben oder eine weitere Aktion auslösen können, während SAP antwortet.
- Braucht SAP zu lange, entsperrt sich der Editor von selbst und warnt Sie, statt Sie warten zu lassen, ohne zu wissen, was passiert.
- Der Status des Objekts — *Unverändert*, *Geändert, nicht gesichert* oder *Geändert, nicht aktiviert* — ist immer in der eigenen Leiste des Editors zu sehen.

**Die gesamte Bedienung mit einem Klick über die eigene Werkzeugleiste**
- Schaltflächen für Ändern/Anzeigen, Sichern, Aktivieren, Suchen und Ersetzen, Versionshistorie (mit integriertem Diff-Vergleich), Änderungen der Sitzung, Beschreibungen, Navigieren und Nachrichten — ohne über die Befehlspalette zu gehen.
- **Konfigurierbare Tastenkürzel** je Aktion, mit Konfliktprüfung und einheitlich für alle VS Code-Fenster.
- Snippets, Autovervollständigung gegen SAP und KI-Codevorschläge direkt im Editor integriert.

---

## Schnellstart

1. Installieren Sie die Erweiterung und laden Sie VS Code neu.
2. `Ctrl+Shift+P` → **IDEA: SAP-Verbindungen verwalten** → legen Sie Ihre SAP-Systeme oder -Umgebungen an.
3. Legen Sie in den Einstellungen einen lokalen Ordner für temporäre Dateien fest (`idea.mcpServer.tempFilesPath`).
4. Laden Sie das Fenster neu (**Entwickler: Fenster neu laden**).

Fertig: Die Erweiterung sucht, bearbeitet und aktiviert bereits gegen SAP, und Ihr KI-Assistent kann analysieren, untersuchen, ändern… was immer Ihnen hilft.

---

## MCP-Server: Ihre KI arbeitet direkt in SAP

Der MCP-Server ermöglicht es einem KI-Assistenten, ABAP-Code direkt im verbundenen SAP-System zu lesen und zu ändern. Er arbeitet nicht auf lokalen Kopien: Alles geht gegen SAP, mit denselben Garantien für Sperren und Aktivierung wie der Rest der Erweiterung.

**Für die KI verfügbare Entwicklungsaktionen:**
- Abfragen, mit welchem SAP-System sie verbunden ist.
- Objekte nach Namen suchen.
- Den Code eines Objekts lesen.
- Ein Objekt in VS Code unter Kontrolle der Erweiterung öffnen.
- Den Code eines Objekts schreiben (mit Bestätigung).
- Ein Objekt aktivieren.

**Verbindung aus Ihrem MCP-Client:** Fügen Sie einen Server vom Typ `http` hinzu, der auf `http://127.0.0.1:<Port>` zeigt (konfigurierbarer Port, zum Beispiel `4856`).

---

## 🔐 Sicherheit und Kontrolle

- IDEA speichert keinen Quellcode in der Cloud: Alles wird direkt gegen Ihr SAP-System gelesen und geschrieben. Der geöffnete Quellcode wird in temporären Dateien auf Ihrem Rechner abgelegt, die gelöscht werden, sobald Sie das Bearbeitungsfenster schließen.
- Kennwörter werden verschlüsselt im sicheren Speicher von VS Code abgelegt, nie im Klartext oder in den Einstellungen.
- Mit `idea.mcpServer.confirmWrites` (standardmäßig aktiv) erfordert jedes von der KI vorgeschlagene Schreiben oder Aktivieren eine vorherige Bestätigung. Außerdem wird es vor der Anwendung als Diff angezeigt.
- Der MCP-Server lauscht nur auf `127.0.0.1` (Ihr eigener Rechner).
- Datenabfragen sind reine Abfragen, SELECT. Sie ändern niemals Tabellendaten.
- Wenn Sie bei der Verbindung "Entwicklung erlaubt" auf false setzen, ist garantiert, dass die KI im System nie etwas ändert, weder Objekte noch Daten.

---

## Erweiterte Funktionen (lizenziert)

Mit einer kleinen Komponente in Ihrem SAP-System (konfiguriert in `idea.endpointAmpliacionADT`) schaltet IDEA in VS Code frei, was nicht einmal das Standard-ADT von SAP bietet:

- **Datenabfragen** Die KI kann SAP-Tabellen abfragen (nur lesend). Das ist es, was der KI ihr volles Potenzial ermöglicht.
- **Leeres Grundgerüst einer Klasse, eines Programms oder eines Interfaces anlegen**
- **Textelemente (REPT)** von Programmen, Klassen und Interfaces — direkte Bearbeitung, ohne SE38/SE24.
- **Data Dictionary**: Datenelemente, Strukturen, Domänen und Tabellentypen, mit Querverweis-Navigation zwischen ihnen.
- **GUI-Status / -Titel** von Programmen: Anlegen, Löschen und visuelle Bearbeitung von Funktionen, Status und Drucktastenleiste.
- **Dynpros (SE51)**: Visueller Editor für Felder und Container, mit Prüfung beim Speichern.

Ohne diese Komponente bleiben diese Aktionen verfügbar: Sie öffnen das Objekt einfach in der klassischen SAP GUI statt in VS Code.

📩 **Möchten Sie die Volllizenz für Ihr Team oder Ihre Beratung?** Schreiben Sie an [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Technische Referenz

<details>
<summary><strong>📋 Befehle und Tastenkürzel</strong></summary>

**Bearbeiten, Speichern und Aktivieren**

| Befehl | Tastenkürzel | Beschreibung |
|---|---|---|
| `IDEA: Bearbeitungs-/Anzeigemodus umschalten` | `Ctrl+F1` | Wechselt zwischen Bearbeitungsmodus (sperrt das Objekt in SAP) und Anzeigemodus (gibt es frei). |
| `IDEA: ABAP-Objekt speichern` | `Ctrl+S` | Speichert lokal und in SAP. Ist das Objekt transportierbar, wird der Transportauftrag **vor** dem Speichern abgefragt. |
| `IDEA: ABAP-Objekt aktivieren` | `Ctrl+F3` | Formatiert das Objekt und aktiviert es in SAP. |
| `IDEA: Änderungen verwerfen und zur Anzeige zurückkehren` | `Ctrl+Shift+U` | Verwirft ungespeicherte Änderungen und kehrt in den Anzeigemodus zurück. |
| `IDEA: Seit der letzten Aktivierung geänderte Blöcke anzeigen` | — | (Klassen und Interfaces) Listet die seit der letzten Aktivierung geänderten Methoden und Abschnitte auf und springt zum gewählten. Auch über die Schaltfläche «N Änderungen» in der Statusleiste. |
| `IDEA: Dokument formatieren` | `Shift+F1` | Formatiert das Objekt mit der konfigurierten Engine. |

**Code schreiben**

| Befehl | Tastenkürzel | Beschreibung |
|---|---|---|
| `IDEA: Zeilenkommentar umschalten (* in Spalte 1)` | `Ctrl+<` | Kommentiert die ausgewählten Zeilen mit `*` in Spalte 1 im SAP-Stil ein oder aus. |
| `IDEA: Anweisung in möglichst wenige Zeilen zusammenführen` | `Ctrl+Shift+J` | Führt mehrere Zeilen zu einer einzigen Anweisung zusammen. |
| `IDEA: Anweisung in Zeilen aufteilen` | `Ctrl+Shift+K` | Teilt eine lange Anweisung (`SELECT`, `CALL METHOD` usw.) auf mehrere Zeilen auf. |
| `IDEA: Deklarative Anweisung in Zeilen aufteilen` | `Ctrl+Shift+D` | Trennt verkettete `DATA:` / `TYPES:`-Deklarationen in einzelne Anweisungen. |

**Navigation und Suche**

| Befehl | Tastenkürzel | Beschreibung |
|---|---|---|
| `IDEA: Codeblock suchen und dorthin navigieren` | `Ctrl+Alt+M` / `Ctrl+Shift+Z` | Schnellliste zum Springen zu einer METHOD / FORM / MODULE / einem Ereignis der Datei. |
| `IDEA: Zum Blockanfang springen` | `Ctrl+Shift+↑` / `Ctrl+Alt+Bild↑` | Springt zum Anfang des Blocks, in dem der Cursor steht. |
| `IDEA: Zum Blockende springen` | `Ctrl+Shift+↓` / `Ctrl+Alt+Bild↓` | Springt zum Ende des Blocks, in dem der Cursor steht. |
| Zur Definition wechseln | `F2` / `F12` / `Ctrl+Click` | Navigiert zur Definition des Objekts unter dem Cursor. In ABAP-Dateien ersetzt `F2` «Umbenennen» (wie in der SAP GUI). |
| `IDEA: Suchen und ersetzen` | `Ctrl+Shift+F` | Öffnet den Bereich «Codesuche» mit dem Fokus im Suchfeld. Funktioniert immer, nicht nur im ABAP-Editor. |

**Verbindungen, MCP-Server und SAP GUI**

| Befehl | Tastenkürzel | Beschreibung |
|---|---|---|
| `IDEA: SAP-Verbindungen verwalten` | — | Fügt verfügbare SAP-Systeme hinzu, bearbeitet oder löscht sie. |
| `IDEA: Aktive Verbindung wechseln` | — | Wählt, gegen welches SAP-System dieses Fenster arbeitet. Auch per Klick auf die Verbindung in der Statusleiste. |
| `IDEA: Alle Verbindungen schließen` | — | Schließt die aktive Verbindung und stoppt die MCP-Server dieses Fensters. |
| `IDEA: MCP-Server starten` | `Ctrl+Alt+S` | Startet den MCP-Server einer Verbindung. |
| `IDEA: MCP-Server stoppen` | — | Stoppt einen laufenden MCP-Server. |
| `IDEA: SAP GUI öffnen` | — | Öffnet ein Fenster der klassischen SAP GUI gegen die gewählte Verbindung. |
| `IDEA: README anzeigen (VS Code-Sprache)` | — | Öffnet dieses README in der Sprache des Editors. |

Außer `Ctrl+Shift+F` gelten die Tastenkürzel, wenn der ABAP-Editor den Fokus hat. In Nicht-ABAP-Dateien behält `Ctrl+F3` seine ursprüngliche VS Code-Funktion («Nächste Auswahl suchen»). Außerdem: **Dokument formatieren** (`Shift+Alt+F`), Autovervollständigung (`Ctrl+Space`) und Code-Faltung.

</details>

<details>
<summary><strong>⚙️ Vollständige Konfiguration</strong></summary>

Einstellungen unter `idea.*` (Datei → Einstellungen → Einstellungen, oder im Bereich «Konfiguration» von IDEA).

**Formatierung (Pretty Printer)**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (Standard), `sapConfig` | Engine für «Dokument formatieren» und vor dem Aktivieren. `extension`: der eigene Formatierer. `sapConfig`: der in SAP konfigurierte Pretty Printer (nur aus der «SAP-Objektsuche» geöffnete Objekte). |
| `idea.prettyprinter.indentation` | `true` (Standard), `false` | Aktiviert oder deaktiviert die automatische Einrückung. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (Standard), `false` | Entfernt doppelte Leerzeichen oder nicht. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (Standard), `lowerKeywords`, `upperAll`, `lowerAll` | Groß-/Kleinschreibung: nur Schlüsselwörter oder der gesamte Code. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (Standard), `modoSe24`, `estandar` | Einrückung von `METHOD` / `ENDMETHOD` (nur Klassen). `auto`: behält vorhandene Leerzeichen bei. `modoSe24`: Spalte 0. `estandar`: eine Ebene (2 Leerzeichen). |
| `idea.prettyprinter.formatScope` | `fullFile` (Standard), `currentMethodOnly` | Beim Formatieren per Tastenkürzel (nur Klassen): die ganze Datei oder nur die Methode, in der der Cursor steht. |

**Autovervollständigung**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (Standard), `false` | Beim Einfügen eines Methoden- oder Funktionsaufrufs mit `Ctrl+Space` wird der Kommentar jedes Parameters mit eingefügt. Bei `false` nur die Parameter. |

**Verbindungen und MCP-Server**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.mcpServer.connections` | Liste der SAP-Systeme | Verfügbare Systeme. Bearbeitung mit «IDEA: SAP-Verbindungen verwalten». Das Kennwort wird **nicht** hier gespeichert: Es wird abgefragt und verschlüsselt im sicheren Speicher von VS Code abgelegt. Felder jeder Verbindung in der folgenden Tabelle. |
| `idea.mcpServer.config` → `mcpInicial` | Name einer Verbindung (standardmäßig leer) | Verbindung, die beim Öffnen von VS Code **aktiv** ist. Leer = keine. |
| `idea.mcpServer.confirmWrites` | `true` (Standard), `false` | Fragt (mit Diff) nach Bestätigung, bevor die KI Code in SAP schreibt oder aktiviert. |
| `idea.mcpServer.tempFilesPath` | Ordnerpfad (standardmäßig leer) | Ordner, in dem die temporären `.abap`-Dateien der «SAP-Objektsuche» angelegt werden. **Pflicht**, um Objekte suchen und öffnen zu können. Die Dateien werden beim Schließen ihres Tabs oder von VS Code gelöscht. |

**Felder jeder Verbindung**

| Feld | Pflicht | Wirkung |
|---|---|---|
| Name | Ja | Kennung des Systems (z. B. `DEV`, `QAS`). Unter diesem Namen verweisen die KI und die Statusleiste darauf. |
| URL | Ja | Basis-URL des SAP-Systems (z. B. `https://meinserver.meinedomain.com:44300`). |
| Mandant | Ja | SAP-Mandant (z. B. `100`). |
| Benutzer | Ja | SAP-Benutzer. |
| MCP-Port | Ja | Lokaler Port (`127.0.0.1`) des MCP-Servers dieser Verbindung. Muss für jede Verbindung unterschiedlich sein. |
| Sprache | Nein | SAP-Anmeldesprache. Ändert nicht die Sprache der Erweiterung, die immer der von VS Code folgt. |
| Nicht vertrauenswürdige Zertifikate zulassen | Nein (`false`) | Akzeptiert selbstsignierte TLS-Zertifikate für dieses System. |
| SAP-System-ID (SID) | Nein | SID wie in Ihrem SAP Logon. Erforderlich, um die klassische SAP GUI zu öffnen. |
| Entwicklung erlaubt | Nein (`true`) | Wenn deaktiviert, ist die Verbindung **nur lesend**: Die KI kann nur suchen, lesen, im Anzeigemodus öffnen, Daten abfragen und Dumps auflisten; sie kann weder schreiben noch aktivieren. Gedacht für Produktivsysteme. |
| Automatischer Start | Nein (`false`) | Startet den MCP-Server dieser Verbindung beim Öffnen von VS Code ohne Nachfrage. Mehrere Verbindungen können markiert werden, damit mehrere Server gleichzeitig laufen. |

**Erweiterte Funktionen und SAP GUI**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.endpointAmpliacionADT` | Servicepfad (standardmäßig leer), z. B. `/sap/serviciosazure/` | Aktiviert die erweiterten Funktionen (Datenabfragen, REPT-Textelemente, Dictionary, GUI-Status/-Titel, Dynpros). Bleibt es leer, öffnen diese Aktionen das Objekt in der SAP GUI. |
| `idea.sapGui.sapshcutPath` | Pfad zu `sapshcut.exe` (standardmäßig leer) | Nur, wenn die SAP GUI nicht an einem Standardort oder im PATH liegt. |
| `idea.navigation.gui` | `sapGui` (Standard), `webGui` | Beim Navigieren zur Definition eines Objekts, das die Erweiterung nicht bearbeitet: klassische SAP GUI (`sapshcut.exe`, benötigt die *SAP-System-ID*) oder Web GUI im Browser. |

</details>

<details>
<summary><strong>🔌 Aktive Verbindung und MCP-Server</strong></summary>

IDEA unterscheidet zwei Begriffe:

- **Aktive Verbindung**: das SAP-System, gegen das *dieses Fenster* von VS Code arbeitet (Suche, Bearbeitung, Aktivierung). Sie wird in der Statusleiste angezeigt und gewechselt. Beim Öffnen von VS Code wird die in `mcpInicial` angegebene aktiviert. Dieselbe Verbindung kann nicht in zwei Fenstern gleichzeitig aktiv sein. Beim Wechsel der Verbindung schließt IDEA zuerst alles, was von der vorherigen geöffnet ist (mit Rückfrage bei ungespeicherten Änderungen).
- **MCP-Server**: einer pro Verbindung, jeder auf seinem eigenen Port. Mehrere können gleichzeitig laufen, sodass die KI parallel in DEV arbeiten und QAS abfragen kann.

**Ihren MCP-Client verbinden:**
- **In VS Code integrierte Clients**: IDEA veröffentlicht automatisch den Server der aktiven Verbindung (`IDEA – <Verbindung>`); nichts zu konfigurieren.
- **Externe Clients** (Claude Code, Cursor…): Fügen Sie einen Server vom Typ `http` hinzu, der auf `http://127.0.0.1:<Port>/mcp` zeigt, mit dem *MCP-Port* der Verbindung. Einen pro Verbindung, die Sie nutzen möchten.

**Für die KI verfügbare MCP-Werkzeuge**

| Werkzeug | Wirkung | Nur lesend |
|---|---|:---:|
| `abap_connection_info` | Gibt an, mit welchem SAP-System der Server verbunden ist. | ✅ |
| `abap_search_object` | Sucht Objekte nach Namen. | ✅ |
| `abap_read_object_source` | Liest den Quellcode eines Objekts. | ✅ |
| `abap_open_object` | Öffnet ein Objekt in VS Code unter Kontrolle der Erweiterung. | ✅ |
| `abap_execute_query` | Führt eine schreibgeschützte `SELECT`-Abfrage auf der Datenbank aus *(erweiterte Funktion)*. | ✅ |
| `abap_list_dumps` | Listet Laufzeitfehler auf (entspricht ST22). | ✅ |
| `abap_write_object_source` | Schreibt den Quellcode eines Objekts (mit Diff und Bestätigung). | — |
| `abap_activate_object` | Aktiviert ein Objekt (mit Bestätigung). | — |
| `abap_llamar_herramienta_desarrollo` | Operationen der erweiterten Komponente: Sperren, Transportaufträge, Textelemente… (mit Bestätigung) *(erweiterte Funktion)*. | — |

Die Spalte *Nur lesend* zeigt die Werkzeuge, die bei Verbindungen mit deaktiviertem **Entwicklung erlaubt** verfügbar sind.

</details>

<details>
<summary><strong>🖥️ Der Seitenbereich «IDEA» im Detail</strong></summary>

Das IDEA-Symbol in der Aktivitätsleiste öffnet vier Abschnitte.

**1. Codesuche**: sucht und ersetzt Text in der im Editor geöffneten ABAP-Datei. *Suchart*: Teilwort oder ganzes Wort. *Bereich*: aktueller Block oder ganze Datei. Ergebnisse zeigen die Zeilennummer (Klick zum Springen) und lassen sich filtern. *Ersetzen* bietet eine Vorschau vor dem Bestätigen. Speichert einen aktuellen Verlauf.

**2. SAP-Objektsuche**: sucht Objekte im SAP-System der aktiven Verbindung und öffnet sie in VS Code (erfordert den laufenden MCP-Server und konfiguriertes `idea.mcpServer.tempFilesPath`). Der Name akzeptiert `*` als Platzhalter.
- **Programm / Report**, **Klasse** und **Funktionsbaustein**: werden als bearbeitbare temporäre Datei im Anzeigemodus geöffnet; beim Schließen des Tabs gelöscht.
- **Klassen**: Schaltflächen zum Öffnen ihrer lokalen Includes: `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` und `<TEST>` (ABAP-Unit-Testklassen).
- **Funktionsgruppen**: zeigt ihren Baum (Funktionsbausteine, Includes und weitere Teile), um jedes Teil einzeln zu öffnen.
- **Datenelement**, **Struktur / Tabelle**, **Domäne**, **Tabellentyp**: werden im Dictionary-Editor geöffnet *(erweiterte Funktion)*.
- **Schaltflächen REPT, CUA und DYNP** (je nach Objekttyp): öffnen die Editoren für Textelemente, GUI-Status/-Titel und Dynpros *(erweiterte Funktionen)*.
- **Schaltfläche Neu**: legt ein Programm, eine Klasse oder ein Dictionary-Objekt (Datenelement, Domäne, Struktur/Tabelle, Tabellentyp) mit Name und Paket an.
- Liefert die Suche ein einziges Ergebnis, wird es direkt geöffnet. Speichert **zuletzt verwendete** und **historische** Suchen.
- Objekte, die die Erweiterung nicht bearbeiten kann, werden in der klassischen SAP GUI (oder Web GUI, je nach `idea.navigation.gui`) geöffnet.

**3. Änderungsverlauf der Sitzung**: speichert Kopien des Objekts bei jedem Speichern oder Aktivieren einer echten Änderung und auch, wenn erkannt wird, dass das Objekt direkt in SAP geändert wurde. Gilt nur für die aktuelle Sitzung: wird beim Schließen des Tabs gelöscht und nicht über Neustarts hinweg aufbewahrt.
- *Versionen laden*: Tabelle mit der neuesten oben, der Uhrzeit der Änderung, ob sie aktiviert wurde, ihrer Herkunft (*Lokal* oder *In SAP geändert*) und der Anzahl der Änderungen gegenüber der letzten Aktivierung und der vorherigen Version.
- **Zwei** Versionen markieren und *Änderungen anzeigen*: öffnet den Diff-Viewer von VS Code.
- *Gesamtänderungen anzeigen*: vergleicht die Anfangsversion mit der aktuellen.
- **Eine** markieren und *Version wiederherstellen*: überträgt ihren Inhalt in den Editor (speichert nicht automatisch).

**4. Konfiguration**: schneller Zugriff, ohne den Bereich zu verlassen, auf:
- SAP-Verbindungen: Tabelle mit *Name*, *Auto-Start* (ihr MCP-Server startet beim Öffnen von VS Code), *Autoverbindung* (die beim Öffnen von VS Code aktive) und *Entwicklung* (ob Entwicklung erlaubt ist); die übrigen Angaben (URL, Mandant, Benutzer, MCP-Port) erscheinen beim Überfahren der Zeile mit der Maus. Schaltfläche *Verbindungen verwalten…*.
- Pretty Printer: Engine, Bereich, Einrückung, doppelte Leerzeichen, Groß-/Kleinschreibung und Einrückung von `METHOD`.
- MCP-Server: Startverbindung, Schreibbestätigung und Ordner für temporäre Dateien.
- Navigation und SAP GUI: wo nicht bearbeitbare Objekte geöffnet werden, Pfad zu `sapshcut.exe` und ADT-Erweiterungsservice.

</details>

<details>
<summary><strong>🧩 Erweiterte Funktionen im Detail</strong></summary>

**Datenabfragen.** Ermöglicht der KI, die Daten Ihres SAP-Systems mit schreibgeschützten `SELECT`-Abfragen zu untersuchen (ohne `INSERT`/`UPDATE`/`DELETE` oder DDL). Ohne sie sieht die KI den Code, aber nicht die Daten, und verliert einen Großteil ihrer Analysefähigkeit.

**Textelement-Editor (REPT).** Über die Schaltfläche *REPT* in der «SAP-Objektsuche», für ein Programm, eine Klasse oder ein Interface:
- Öffnet sich im Anzeigemodus (blauer Hintergrund).
- *Bearbeiten* sperrt das Objekt in SAP (bernsteinfarbener Hintergrund); bei Änderung einer Zelle erscheint 🔴 auf dem Tab.
- *Speichern und aktivieren* lädt die Texte nach SAP hoch (fragt bei Bedarf nach einem Transportauftrag) und behält die Sperre bei, um weiter zu bearbeiten.
- Beim Zurückkehren in den Anzeigemodus oder Schließen des Tabs wird die Sperre freigegeben.
- *Kopieren* überträgt die gesamte Texttabelle in die Zwischenablage.

**Dictionary-Editor.** Datenelemente, Strukturen / Tabellen, Domänen und Tabellentypen: Kopf, technische Optionen und Liste der Felder oder Werte. Öffnet sich im Anzeigemodus; *Bearbeiten* sperrt das Objekt und erlaubt, es mit derselben Transportauftragsverwaltung wie der Rest zu ändern und zu aktivieren. Der Kopf der Feldtabelle bleibt beim Scrollen fixiert; Spalten sind sortier- und filterbar. Aus den Zellen navigiert man zu anderen Datenelementen und Domänen.

**GUI-Status / -Titel (CUA).** Anlegen, Löschen und Bearbeiten von Titeln, Funktionen, Status und Standard-Drucktastenleiste.

**Dynpros (SE51).** Visueller Editor für Felder und Container (Rahmen, Subscreens, Tabstrips, Table Controls): Anlegen durch Platzieren des Elements per Klick, Erkennung von Überlappungen und Prüfung beim Speichern.

Alle folgen derselben Disziplin bei Sperre, Transportauftrag und Aktivierung wie die übrigen Objekte.

</details>

---

## Lizenz

Die Erweiterung ist unter der MIT-Lizenz frei nutzbar.

Wenn Sie an den erweiterten Funktionen interessiert sind, die die ABAP-Komponente „ADT Ampliado“ (Erweitertes ADT) erfordern, wenden Sie sich für Bedingungen und Preise an Marcos Almeida Santolaria unter [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

[Español](README.md) · [English](README.en.md) · **Deutsch** · [Français](README.fr.md)
