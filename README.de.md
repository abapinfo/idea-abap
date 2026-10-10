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
| 🐞 **Integrierter ABAP-Debugger** | Breakpoints aus dem Editor und ein Debugging-Fenster pro Ausführung in SAP, parallel: Breakpoints auf Anweisung, Methode, Funktion, FORM, Ausnahme oder Nachricht, Watchpoints, Ändern von Werten und bearbeitbare interne Tabellen. |
| 🔎 **Verwendungsnachweis** | Verwendungsnachweis des Worts unter dem Cursor (`Ctrl+Shift+F3`) oder jeder Nachricht einer Nachrichtenklasse, mit der Anweisung jeder Verwendung und direktem Sprung zur Zeile. |
| ✉️ **Nachrichtenklassen** | Anlegen und Bearbeiten von Nachrichtenklassen (SE91) in einer Tabelle, mit Langtext und Verwendungsliste. |
| 🧯 **Dumps jedes Datums, ohne Tokens zu verschwenden** *(erweiterte Funktion)* | Ihre KI findet Dumps jedes Datums (nicht nur die der letzten 24 h wie im Standard-ADT): zuerst eine kompakte Liste mit Schlüssel, Fehler und Position jedes Dumps; dann, nur für den relevanten, die ST22-Zusammenfassung und den Aufrufstack. Variablen oder der vollständige Dump nur bei Bedarf. Weniger Text für die KI, weniger Tokens und schnellere Antworten. |
| 🧩 **Mehr als Standard-ADT** *(erweiterte Funktion)* | Bearbeitung von Textelementen (REPT), Data Dictionary, GUI-Status/-Titel und Dynpros — alles, was das SAP-ADT außerhalb der SAP GUI nicht bearbeiten lässt. |

---

## Was IDEA im Vergleich zu anderen Werkzeugen abdeckt

Vergleich auf SAP ECC mit NetWeaver 7.50 zwischen dem SAP-ADT für Eclipse, anderen ABAP-Erweiterungen für VS Code, der ABAP-Komponente „ADT Ampliado“ (Erweitertes ADT) und IDEA selbst.

🟢 Abgedeckt · 🟡 Teilweise · 🔴 Nicht verfügbar · ➖ Erledigt das Standard-ADT · **AMP** Erfordert Erweitertes ADT

| Funktion | SAP ADT | Andere Erweiterungen | Erweitertes ADT | IDEA |
|---|---|---|---|---|
| **Objekte mit Quelltext** | | | | |
| Programme, Includes und Reports | 🟢 | 🟢 | ➖ | 🟢 |
| Klassen und Interfaces | 🟢 | 🟢 | ➖ | 🟢 Blockweise (Methode für Methode) oder vollständig, wie in SE24 |
| Lokale Klassen-Includes <br><sub>`CCDEF · CCIMP · CCMAC · CCAU`</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Funktionsgruppen und -bausteine | 🟢 | 🟢 | ➖ | 🟢 Baum der Gruppe; ohne Anlegen |
| Klassenbeschreibungen <br><sub>Kurztexte von Methoden, Attributen und Parametern</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Bearbeitbare Tabelle im Editor |
| CDS-Views und Typgruppen <br><sub>`DDLS · TYPE`</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Nachrichtenklassen <br><sub>`MSAG`</sub> | 🟢 | 🟢 | ➖ | 🟢 Anlegen, Bearbeitung in Tabelle, Langtext und Verwendungsnachweis jeder Nachricht |
| **Data Dictionary** | | | | |
| Datenelemente <br><sub>`DTEL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Domänen <br><sub>`DOMA`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Inklusive Festwerte |
| Strukturen <br><sub>`TABL`</sub> | 🟢 | 🟢 Als Quelltext | 🟢 | 🟢 **AMP** Feldeditor mit Navigation |
| Datenbanktabellen <br><sub>`TABL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Tabellentypen <br><sub>`TTYP`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| **Texte und klassische Oberfläche** | | | | |
| Textelemente <br><sub>`REPT` · Textsymbole und Selektionstexte</sub> | 🟡 Je nach Release | 🟡 Je nach Release | 🟢 | 🟢 **AMP** |
| GUI-Status / -Titel <br><sub>`CUAD` · SE41</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Anlegen, Löschen und Bearbeiten von Funktionen, Status und Leiste |
| Dynpros <br><sub>`DYNP` · SE51</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Visueller Editor für Felder und Container |
| **RAP und OData** | | | | |
| RAP-Business-Objekte <br><sub>`BDEF · SRVD` · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🟡 Je nach Erweiterung, als Quelltext | 🔴 | 🔴 |
| RAP-Generator <br><sub>Tabelle, CDS, Verhalten und Service in einem Schritt · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| RAP-OData-Services <br><sub>`SRVB` · Service Binding und Fiori-Vorschau · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| **Lebenszyklus des Objekts** | | | | |
| Objekte suchen | 🟢 | 🟢 | ➖ | 🟢 Mit zuletzt verwendeten und Historie |
| Code-Objekte anlegen <br><sub>Programme, Klassen und Funktionen</sub> | 🟢 | 🟢 | 🟢 Programme und Klassen | 🟡 **AMP** Programme, Klassen und Nachrichtenklassen; keine Funktionen |
| Dictionary-Objekte anlegen <br><sub>`DTEL · DOMA · TABL · TTYP`</sub> | 🟡 Nur Strukturen | 🟡 Nur Strukturen | 🟢 | 🟢 **AMP** |
| Anzeige- / Bearbeitungsmodus <br><sub>Explizite Objektsperre, wie in SE38</sub> | 🟡 Sperrt beim ersten Tippen | 🟡 Sperrt beim ersten Tippen | 🟢 Jedes Objekt, auch Dynpros | 🟢 Ctrl+F1, Status immer sichtbar |
| Transportauftrag beim Sichern | 🟢 | 🟢 | 🟢 Offene Aufträge und Anlegen von Aufträgen | 🟢 |
| Aktivierung und inaktive Objekte | 🟢 | 🟢 Massenaktivierung | ➖ | 🟢 Hinweis auf geänderte Teile |
| Auftragsverwaltung <br><sub>Freigeben, Eigentümer ändern, ATC auf dem Auftrag</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Versionen und Vergleich | 🟢 | 🟢 Plus Autorenschaft pro Zeile (blame) | ➖ | 🟡 Sitzungshistorie mit Diff |
| abapGit | 🟢 Plugin | 🟢 | ➖ | 🔴 |
| **Code schreiben** | | | | |
| Autovervollständigung und Gehe zu Definition | 🟢 | 🟢 | ➖ | 🟢 F2 wie in der SAP GUI |
| Syntaxprüfung | 🟢 | 🟢 | ➖ | 🟢 |
| Formatierung | 🟢 | 🟢 | ➖ | 🟢 SAP-Standard oder eigener der Erweiterung (nur die geänderten Zeilen) |
| Verwendungsnachweis | 🟢 | 🟢 | ➖ | 🟢 Des Worts unter dem Cursor und jeder Nachricht; mit der Anweisung jeder Verwendung |
| Refactoring <br><sub>Umbenennen, Methode extrahieren</sub> | 🟢 | 🟡 Schnellkorrekturen | ➖ | 🔴 |
| Hilfsfunktionen im SAP-GUI-Stil <br><sub>Mit * kommentieren, Anweisungen verbinden und teilen, zwischen Blöcken springen</sub> | 🟡 | 🔴 | ➖ | 🟢 |
| KI-Vorschläge im Editor | 🔴 | 🟢 GitHub Copilot | ➖ | 🟢 Claude, Gemini oder GitHub Copilot |
| **Testen und analysieren** | | | | |
| Debugger | 🟢 | 🟢 | ➖ | 🟢 Mehrere Sitzungen parallel; Breakpoints aller Art, Watchpoints, konfigurierbares Layout und Tastenkürzel |
| ABAP Unit | 🟢 | 🟢 | ➖ | 🔴 |
| ATC / Code Inspector | 🟢 | 🟢 | ➖ | 🔴 |
| Performance-Traces | 🟢 | 🟢 | ➖ | 🔴 |
| Dumps der letzten 24 Stunden <br><sub>ST22 · Standard-ADT-Feed</sub> | 🟢 | 🟢 | ➖ | 🟡 Ohne Bildschirm: holt die Dumps über das Standard-ADT, um sie der KI zu geben |
| Dumps beliebigen Datums <br><sub>ST22 · zwischen zwei Daten, mit vollständigem Detail und Aufrufstack</sub> | 🔴 Nur die letzten 24 Stunden | 🔴 Nur die letzten 24 Stunden | 🟢 | 🟡 **AMP** Ohne Bildschirm: Liste und Detail über das Erweiterte ADT, optimiert, um KI-Tokens zu sparen |
| Datenabfragen <br><sub>SELECT, nur lesend</sub> | 🟢 Einfache Abfragen | 🟢 Einfache Abfragen | 🟢 Komplexe Abfragen | 🟢 **AMP** Komplexe Abfragen, für die KI |
| **KI und mehrere Systeme** | | | | |
| MCP-Server für jeden KI-Assistenten <br><sub>Claude Code, Copilot, Cursor…</sub> | 🔴 | 🟢 Hängt von der Erweiterung ab | ➖ | 🟢 |
| Mehrere Systeme gleichzeitig <br><sub>Zum Beispiel Entwicklung und Produktion</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Nur-Lese-Verbindung <br><sub>Für Produktivsysteme</sub> | 🔴 | 🟡 Warnung in Produktion | 🟢 | 🟢 Die KI kann weder schreiben noch aktivieren |
| Nicht unterstützte Objekte in der SAP GUI öffnen | - | 🟢 SAP GUI oder Web GUI | ➖ | 🟢 SAP GUI oder Web GUI, direkt zum Objekt |

*Erweitertes ADT* ist kein Editor: Es ist der ABAP-Service, der IDEA das gibt, was das Standard-ADT nicht bereitstellt. Ohne ihn öffnet IDEA die mit **AMP** markierten Objekte in der SAP GUI. In S/4HANA (NetWeaver 7.52 oder höher) bringt das Standard-ADT eigene Editoren für weitere Dictionary-Objekte und für Textelemente mit. Die KI-Funktionen von SAP (Joule) sind in ECC nicht verfügbar. RAP und RAP-OData-Services ebenfalls nicht: In ECC werden OData-Services mit SEGW in der SAP GUI erstellt.

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

**Verwendungsnachweis**
- **Schaltfläche Referenzen** (`Ctrl+Shift+F3`): listet auf, wo der Bezeichner unter dem Cursor verwendet wird — Klasse, Interface, Methode, Attribut, Variable, Programm, Funktion, Typ, Datenelement, Tabelle, Struktur oder Domäne.
- Jede Verwendung zeigt Objekttyp, Namen, Zeile und die vollständige Anweisung; ein Klick auf die Zeile öffnet das Objekt an dieser Stelle.
- Von einem `MESSAGE e001(zklasse)` oder einem `MESSAGE ID 'ZKLASSE' ... NUMBER '001'` navigiert `F2` zur Nachrichtenklasse mit dem Fokus auf dieser Nachricht.

**Debugging aus dem Editor**
- **Schaltfläche Breakpoint** (`F9`): setzt oder entfernt einen Breakpoint in der Cursorzeile; er wird am Rand rot markiert.
- **Schaltfläche Ausführen** (`Ctrl+F8`): öffnet das Objekt in der Web GUI, um es zu starten und an den Breakpoints anzuhalten.

**Volle Kontrolle über die Wartezeiten gegenüber SAP**
- Während gegen SAP gesperrt, gespeichert, aktiviert oder formatiert wird, sperrt sich der gesamte Editor (eine Ebene zeigt an, was gerade geschieht), damit Sie nicht weiterschreiben oder eine weitere Aktion auslösen können, während SAP antwortet.
- Braucht SAP zu lange, entsperrt sich der Editor von selbst und warnt Sie, statt Sie warten zu lassen, ohne zu wissen, was passiert.
- Der Status des Objekts — *Unverändert*, *Geändert, nicht gesichert* oder *Geändert, nicht aktiviert* — ist immer in der eigenen Leiste des Editors zu sehen.

**Die gesamte Bedienung mit einem Klick über die eigene Werkzeugleiste**
- Schaltflächen für Ändern/Anzeigen, Sichern, Aktivieren, Suchen und Ersetzen, Versionshistorie (mit integriertem Diff-Vergleich), Änderungen der Sitzung, Beschreibungen, Navigieren und Nachrichten — ohne über die Befehlspalette zu gehen.
- **Konfigurierbare Tastenkürzel** je Aktion, mit Konfliktprüfung und einheitlich für alle VS Code-Fenster.
- Snippets, Autovervollständigung gegen SAP und KI-Codevorschläge direkt im Editor integriert.

---

## ABAP-Debugger

Debuggen Sie in VS Code die Programme, die in SAP laufen, mit einem eigenen Fenster für jede Ausführung.

1. **IDEA: ABAP-Debugging starten** lässt die aktive Verbindung auf Ausführungen in SAP lauschen.
2. Setzen Sie Breakpoints im Editor mit `F9` (oder der Schaltfläche *Breakpoint*).
3. Führen Sie das Programm in SAP aus (zum Beispiel mit der Schaltfläche *Ausführen* des Editors, die es in der Web GUI öffnet).
4. Erreicht die Ausführung einen Breakpoint, öffnet sich ein Debugging-Fenster. Kommen mehrere Ausführungen an, öffnet sich für jede ein eigenes Fenster, parallel (bis zu 4; darüber hinaus werden sie ohne Fenster freigegeben).
5. **IDEA: ABAP-Debugging beenden** entfernt die in SAP gesetzten Breakpoints und schließt die Sitzungen.

**Das Debugging-Fenster**
- **Werkzeugleiste**: Einzelschritt (`F5`), Ausführen (`F6`), Return (`F7`), Weiter (`F8`), Breakpoint in der Zeile (`F9`), weitere Breakpoints (`Shift+F9`), Watchpoint (`Shift+F4`), Liste der Breakpoints und Watchpoints, Layout (`F10`) und Tastenkürzel.
- **Feste Kopfzeile**: Programm, Include, Blocktyp und -name, Zeile, `SY-SUBRC` und `SY-TABIX`.
- **Code**: immer im Anzeigemodus; Methoden werden wie im Editor blockweise angezeigt. Doppelklick auf die Zeilennummer setzt oder entfernt einen Breakpoint; Doppelklick oder `F2` auf eine Variable fügt sie zu *Variablen* hinzu; `F12` springt zur Anweisung am Cursor.
- **Variablen, Lokale und Globale**: Name, Wert, technischer Typ, absoluter Typ und Hexadezimalwert. Werte werden mit dem Stift geändert; Strukturen lassen sich aufklappen; interne Tabellen werden seitenweise angezeigt, mit Einfügen und Löschen von Zeilen. Alles lässt sich in die Zwischenablage kopieren, um es in eine Tabellenkalkulation einzufügen.
- **Navigation**: der Aufrufstapel (Ebene, Ereignistyp und Ereignis, Programm, Include und Zeile); Doppelklick, um eine andere Ebene anzuzeigen.
- **Weitere Breakpoints**: auf ABAP-Anweisung, Methode (globaler oder lokaler Klasse), Funktion, FORM, klassenbasierte Ausnahme, Nachricht oder Quelltext, mit optionaler Bedingung. Sie werden gemerkt und bei der nächsten Ausführung des Programms erneut gesetzt.
- **Watchpoints**: halten an, wenn sich eine Variable ändert, mit optionaler Bedingung.
- **Konfigurierbares Bildschirmlayout**: Sie legen fest, wie viele Zeilen und Spalten es gibt und welcher Frame in jede Zelle kommt (Code, Navigation, Variablen, Lokale, Globale). Layouts werden mit Namen gespeichert und gelten für alle Fenster; die Größe jedes Frames ändern Sie durch Ziehen der Trennbalken.
- **Konfigurierbare Tastenkürzel** für alle Aktionen, im Panel selbst (Schaltfläche *Tastenkürzel*) oder über die Einstellung `idea.depuracion.atajos`.

---

## Nachrichtenklassen (SE91)

Über die «SAP-Objektsuche» (Typ *Nachrichtenklasse*) oder per `F2` aus einem `MESSAGE` öffnet sich die Klasse in einer bearbeitbaren Tabelle. Sie läuft vollständig über das Standard-ADT, ohne die erweiterte Komponente.

- Sie öffnet sich im Anzeigemodus; *Bearbeiten* sperrt die Klasse und *Sichern* speichert sie und fragt bei Bedarf nach dem Transportauftrag.
- Tabelle mit Nummer, Text, Länge und Kennzeichen „selbsterklärend“; sie lässt sich pro Spalte filtern und vollständig in die Zwischenablage kopieren.
- Anlegen und Löschen von Nachrichten, mit Prüfung beim Sichern (eindeutige 3-stellige Nummern, Pflichttexte und Maximallänge).
- Für jede Nachricht: **Langtext** anzeigen, **Verwendungsnachweis** (mit direktem Sprung zu jeder Verwendung) oder in SE91 öffnen.
- Mit der Schaltfläche *Neu* der «SAP-Objektsuche» wird eine leere Nachrichtenklasse angelegt und im Bearbeitungsmodus geöffnet.

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
- **Dumps jedes Datums (ST22)**, nicht nur die der letzten 24 Stunden wie im Standard-ADT, und für die KI optimiert: kompakte Liste, Detail nur für den relevanten Dump und vollständige Daten nur bei Bedarf — so verbraucht die KI deutlich weniger Tokens.
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

**Debugging**

| Befehl | Tastenkürzel | Beschreibung |
|---|---|---|
| `IDEA: ABAP-Debugging starten` | — | Lässt die aktive Verbindung auf Ausführungen in SAP lauschen; jede, die an einem Breakpoint anhält, öffnet ihr Debugging-Fenster. |
| `IDEA: Breakpoint in der aktuellen Zeile` | `F9` | Setzt oder entfernt einen Breakpoint in der Cursorzeile. |
| `IDEA: ABAP-Debugging beenden` | — | Entfernt die in SAP gesetzten Breakpoints, beendet das Lauschen und schließt die Debugging-Fenster. |
| Verwendungsnachweis | `Ctrl+Shift+F3` | (Quelltext-Editor) Wo der Bezeichner unter dem Cursor verwendet wird. |
| In der Web GUI ausführen | `Ctrl+F8` | (Quelltext-Editor) Öffnet das Objekt in der Web GUI, um es auszuführen. |

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

**Debugger**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.depuracion.atajos` | Objekt Aktion → Taste | Tastenkürzel des Debugging-Fensters. Standard: `F5` Einzelschritt, `F6` Ausführen, `F7` Return, `F8` Weiter, `F9` Breakpoint, `Shift+F9` weitere Breakpoints, `Shift+F4` Watchpoint, `F2` Variable hinzufügen, `F12` zur Anweisung springen, `F10` Layout. Sie lassen sich auch über die Schaltfläche *Tastenkürzel* des Panels ändern. |

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
| `abap_list_dumps_24h` | Listet Laufzeitfehler der letzten 24 Stunden auf (Standard-ADT-Feed). | ✅ |
| `abap_list_dumps` | Listet Laufzeitfehler jedes Datums auf (entspricht ST22), in kompakter Form *(erweiterte Funktion)*. | ✅ |
| `abap_get_dump_detalle` | Liefert das Detail eines Dumps: ST22-Zusammenfassung und Aufrufstack; Variablen oder der vollständige Dump nur auf Anfrage *(erweiterte Funktion)*. | ✅ |
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
- **Nachrichtenklasse**: öffnet sich im Editor für Nachrichtenklassen (über das Standard-ADT, ohne erweiterte Komponente).
- **Schaltfläche Neu**: legt ein Programm, eine Klasse, eine Nachrichtenklasse oder ein Dictionary-Objekt (Datenelement, Domäne, Struktur/Tabelle, Tabellentyp) mit Name und Paket an. Ohne die erweiterte Komponente können nur Nachrichtenklassen angelegt werden.
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
