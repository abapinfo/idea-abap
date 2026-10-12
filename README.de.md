# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Integrierte Entwicklungsumgebung für ABAP

[Español](README.md) · [English](README.en.md) · **Deutsch** · [Français](README.fr.md)

> 💡 Um dieses README in einer anderen Sprache in VS Code zu lesen, führen Sie **IDEA: README anzeigen** (`Ctrl+Shift+P`) aus: Es öffnet sich automatisch in der Sprache Ihres Editors.

---

## Was ist **IDEA**?

**IDEA** macht Visual Studio Code (VS Code) zu einer Arbeitsumgebung mit einem KI-Assistenten, der mit Ihren SAP-Systemen verbunden ist. Mit der Komponente *ADT Ampliado* (Erweitertes ADT) kann die KI recherchieren, analysieren und Maßnahmen und Lösungen auf Basis Ihrer eigenen Daten und Ihres eigenen Codes vorschlagen.

Außerdem ist **IDEA** eine vollständige ABAP-Entwicklungsumgebung, in der die KI:
- Änderungen am Quelltext Ihres SAP-Systems vorschlägt, die Sie prüfen und übernehmen oder ablehnen.
- Am echten System prüft, ob ihre Lösungen gültig sind: ob die Klasse, der Funktionsbaustein oder die Parameter wirklich existieren.
- Informationen mehrerer Systeme vergleicht (Entwicklung, Integration, Produktion…).
- Recherchiert und Ihnen die beste Lösung anbietet.

**IDEA** sorgt dafür, dass Codeänderungen sicher sind und dass die KI niemals Daten Ihres SAP-Systems ändert: Sie kann sie nur abfragen.

Auch die KI-Kosten bleiben unter Kontrolle. Der Assistent, der die Werkzeuge von **IDEA** nutzt (Claude Code, GitHub Copilot…), wird per Abonnement bezahlt, nicht nach Verbrauch. Nur die optionalen Inline-Codevorschläge des Editors können eine nutzungsabhängig abgerechnete API (nach Tokens) verwenden, und sie werden separat konfiguriert. Mit **IDEA** arbeiten also zwei KI-Modelle: eines für die Vorschläge beim Tippen und ein anderes, das Ihres Assistenten, das die Werkzeuge von **IDEA** nutzt.

## KI für Ihr Unternehmen: sicher, kontrolliert und wirtschaftlich

**IDEA** verbindet eine KI mit jedem Ihrer SAP-Systeme, damit sie darauf arbeitet: Sie recherchiert, analysiert und schlägt Maßnahmen und Lösungen vor.

Stellen Sie sich vor, Ihr Unternehmen ist eine Elektronik-Ladenkette und Sie nutzen **IDEA** und die KI, um Fragen wie diese zu beantworten:

**1. Das Unternehmen kennenlernen**
- Was verkauft dieses Unternehmen? Beschreibe den Katalog in zwei Zeilen.
- Wie viele Produkte, Kunden und Aufträge haben wir?
- Welches ist das teuerste und welches das günstigste Produkt?
- Welche Produktkategorien gibt es und wie viele Artikel hat jede?

**2. Vertrieb**
- Wie viel haben wir in jedem Jahr fakturiert? Welches Jahr war das beste?
- Welche 10 Produkte haben am meisten Umsatz gebracht?
- Gibt es Saisonalität? In welchen Monaten verkaufen wir am meisten?
- Wie hoch ist der durchschnittliche Auftragswert? Und der größte Auftrag aller Zeiten?
- Wie viele Aufträge sind bezahlt, noch nicht fakturiert oder storniert?

**3. Kunden und Karte**
- Wer sind unsere 5 besten Kunden und aus welchem Land kommt jeder?
- In welchen Ländern verkaufen wir? Sortiere sie nach Umsatz.
- Welche Kunden haben am längsten nicht mehr bei uns gekauft? (Verlorene Kunden erkennen.)
- Welcher Kunde kauft bei uns immer dasselbe Produkt?

**4. Produkte und Kundenbewertungen**
- Welche Produkte sind in den Kundenbewertungen am besten und am schlechtesten bewertet?
- Fasse zusammen, was die Kunden über das am schlechtesten bewertete sagen.
- Gibt es ein Produkt, das sich gut verkauft, aber schlechte Bewertungen hat?
- Welcher Lieferant liefert die am besten bewerteten Produkte?

**5. Lager**
- Welche Produkte liegen unter dem Mindestbestand? Wie viel müsste nachbestellt werden?
- Gibt es Produkte mit viel Bestand, die sich kaum verkaufen? (Gebundener Bestand.)
- Wer ist für jedes Produkt unter Mindestbestand der Lieferant und wie lautet seine E-Mail?

**6. Schlussfolgern und Daten verknüpfen**
- Wenn wir morgen nicht mehr mit unserem größten Lieferanten zusammenarbeiten würden, welchen Anteil am Umsatz würden wir verlieren?
- Welche Produkte werden häufig zusammen gekauft? (Warenkorbanalyse.)
- Erstelle mir einen Management-Bericht in 5 Punkten über die Lage des Unternehmens.
- Welche drei Maßnahmen empfiehlst du auf Basis der Daten, um im nächsten Jahr mehr zu verkaufen?
- In einem Land sind die Umsätze eingebrochen: Finde es und erkläre, woran es liegen könnte.

## Moderne ABAP-Entwicklung, ohne VS Code zu verlassen

**IDEA** macht VS Code zu einer vollständigen ABAP-Entwicklungsumgebung: in Echtzeit mit Ihrem SAP-System verbunden und bereit, Seite an Seite mit dem KI-Assistenten zu arbeiten, den Sie bereits nutzen (Claude Code, GitHub Copilot, Cursor…).

Schluss mit dem Kopieren und Einfügen von Code zwischen SAP GUI und einem KI-Chat. Schluss damit, den Überblick zu verlieren, welches Objekt gesperrt ist, wer es geändert hat oder ob es noch auf die Aktivierung wartet. Mit IDEA passiert alles direkt im Editor, mit derselben Disziplin bei Sperren, Transportaufträgen und Aktivierung, die Sie aus SAP kennen, aber mit der Geschwindigkeit von VS Code und der Leistung der KI.

**In einem Satz:** Objekt suchen → öffnen → Ihre KI bitten, die Änderung vorzuschlagen (oder sie selbst vornehmen) → sichern und aktivieren. Alles ohne VS Code zu verlassen, alles unter Kontrolle.

**In einem anderen Satz 😉:** Ein IDoc ist fehlgeschlagen? → Ihre KI bitten, es zu analysieren und die Lösung zu nennen → sie anwenden. Alles ohne VS Code zu verlassen, alles unter Kontrolle.

---

## Warum Ihr Team es lieben wird

| | |
|---|---|
| ⚡ **Echte Geschwindigkeit** | Sofortige Suche nach Programmen, Klassen, Interfaces und Dictionary-Objekten, mit Suchverlauf. Ohne Transaktionen oder verschachtelte Menüs. |
| 🤖 **KI mit direktem Zugriff auf SAP** | Integrierter MCP-Server: Ihr KI-Assistent sucht und liest Code und Daten in SAP und schlägt Ihnen die Änderungen im Editor vor, mit den Unterschieden direkt vor Augen. Sie entscheiden, ob Sie sie übernehmen; ohne Sie wird nichts in SAP gesichert. |
| 🌐 **Mehrere Systeme** | Mehrere MCP-Server gleichzeitig, einer pro System: Ihre KI kann in der Entwicklung Änderungen vorschlagen, während sie über eine Nur-Lese-Verbindung Daten der Produktion abfragt. |
| 🔒 **Keine Überraschungen** | Standardmäßig Anzeigemodus, explizite Sperre zum Ändern, Transportaufträge und Aktivierung genau wie im SAP-Standard. |
| 🕘 **Verlauf im Handumdrehen** | Jedes Sichern und jede Aktivierung wird im Editor-Tab festgehalten: Versionen vergleichen oder eine frühere wiederherstellen, ohne den Editor zu verlassen. |
| 🎨 **Formatierung, die Ihre Diffs respektiert** | Eigener Formatierer, der sich auf die geänderten Methoden beschränken lässt, damit nicht versehentlich ganze Klassen umformatiert werden. |
| 🖥️ **Quelltext-Editor wie in der SAP GUI** | In den Tab eingebetteter Editor: Anzeige- und Änderungsmodus, Klassen blockweise oder vollständig, bearbeitbare Beschreibungen, direkter Zugriff auf Textelemente, GUI-Status/-Titel, Dynpros und lokale Includes, sowie volle Kontrolle über die Wartezeiten gegenüber SAP. |
| 🐞 **Integrierter ABAP-Debugger** | Breakpoints aus dem Editor und ein Debugging-Fenster pro Ausführung in SAP, parallel: Breakpoints auf Anweisung, Methode, Funktion, FORM, Ausnahme oder Nachricht, Watchpoints, Ändern von Werten und bearbeitbare interne Tabellen. |
| 🔎 **Verwendungsnachweis** | Verwendungsnachweis des Worts unter dem Cursor (`Ctrl+Shift+F3`) oder jeder Nachricht einer Nachrichtenklasse, mit der Anweisung jeder Verwendung und direktem Sprung zur Zeile. |
| ✉️ **Nachrichtenklassen** | Anlegen und Bearbeiten von Nachrichtenklassen (SE91) in einer Tabelle, mit Langtext und Verwendungsliste. |
| 🧯 **Dumps jedes Datums, ohne Tokens zu verschwenden** *(erweiterte Funktion)* | Ihre KI findet Dumps jedes Datums (nicht nur die der letzten 24 h wie im Standard-ADT): zuerst eine kompakte Liste mit Schlüssel, Fehler und Position jedes Dumps; dann, nur für den relevanten, die ST22-Zusammenfassung und den Aufrufstack. Variablen oder der vollständige Dump nur bei Bedarf. Weniger Text für die KI, weniger Tokens und schnellere Antworten. |
| 🧩 **Mehr als Standard-ADT** *(erweiterte Funktion)* | Bearbeitung von Textelementen (REPT), Data Dictionary, GUI-Status/-Titel und Dynpros: alles, was das SAP-ADT außerhalb der SAP GUI nicht bearbeiten lässt. |

---

## Was IDEA im Vergleich zu anderen Werkzeugen abdeckt

Vergleich auf SAP ECC mit NetWeaver 7.50 zwischen dem SAP-ADT für Eclipse, anderen ABAP-Erweiterungen für VS Code, der ABAP-Komponente *ADT Ampliado* (Erweitertes ADT) und IDEA selbst.

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
| GUI-Status / -Titel <br><sub>`CUAD` · SE41</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Anlegen, Löschen und Bearbeiten von Funktionen, Status und Drucktastenleiste |
| Dynpros <br><sub>`DYNP` · SE51</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Visueller Editor für Felder und Container |
| **RAP und OData** | | | | |
| RAP-Business-Objekte <br><sub>`BDEF · SRVD` · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🟡 Je nach Erweiterung, als Quelltext | 🔴 | 🔴 |
| RAP-Generator <br><sub>Tabelle, CDS, Verhalten und Service in einem Schritt · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| RAP-OData-Services <br><sub>`SRVB` · Service Binding und Fiori-Vorschau · nur NetWeaver 7.54 oder S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| **Lebenszyklus des Objekts** | | | | |
| Objekte suchen | 🟢 | 🟢 | ➖ | 🟢 Mit zuletzt verwendeten und Historie |
| Code-Objekte anlegen <br><sub>Programme, Klassen und Funktionen</sub> | 🟢 | 🟢 | 🟢 Programme und Klassen | 🟡 **AMP** Programme, Klassen und Nachrichtenklassen; keine Funktionen |
| Dictionary-Objekte anlegen <br><sub>`DTEL · DOMA · TABL · TTYP`</sub> | 🟡 Nur Strukturen | 🟡 Nur Strukturen | 🟢 | 🟢 **AMP** |
| Anzeige- / Bearbeitungsmodus <br><sub>Explizite Objektsperre, wie in SE38</sub> | 🟡 Sperrt beim ersten Tippen | 🟡 Sperrt beim ersten Tippen | 🟢 Jedes Objekt, auch Dynpros | 🟢 `Ctrl+F1`, Status immer sichtbar |
| Transportauftrag beim Sichern | 🟢 | 🟢 | 🟢 Offene Aufträge und Anlegen von Aufträgen | 🟢 |
| Aktivierung und inaktive Objekte | 🟢 | 🟢 Massenaktivierung | ➖ | 🟢 Hinweis auf geänderte Teile |
| Auftragsverwaltung <br><sub>Freigeben, Eigentümer ändern, ATC auf dem Auftrag</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Versionen und Vergleich | 🟢 | 🟢 Plus Autorenschaft pro Zeile (blame) | ➖ | 🟡 Sitzungshistorie mit Diff |
| abapGit | 🟢 Plugin | 🟢 | ➖ | 🔴 |
| **Code schreiben** | | | | |
| Autovervollständigung und Gehe zu Definition | 🟢 | 🟢 | ➖ | 🟢 `F2` wie in der SAP GUI |
| Syntaxprüfung | 🟢 | 🟢 | ➖ | 🟢 |
| Formatierung | 🟢 | 🟢 | ➖ | 🟢 SAP-Standard oder eigener der Erweiterung (auf die geänderten Methoden beschränkbar) |
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
| MCP-Server für jeden KI-Assistenten <br><sub>Claude Code, Copilot, Cursor…</sub> | 🔴 | 🟢 Hängt von der Erweiterung ab | ➖ | 🟢 Die KI schlägt Änderungen im Editor vor; der Benutzer übernimmt oder lehnt sie ab |
| Mehrere Systeme gleichzeitig <br><sub>Zum Beispiel Entwicklung und Produktion</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Nur-Lese-Verbindung <br><sub>Für Produktivsysteme</sub> | 🔴 | 🟡 Warnung in Produktion | 🟢 | 🟢 Die KI kann weder Änderungen vorschlagen noch etwas ändern |
| Nicht unterstützte Objekte in der SAP GUI öffnen | - | 🟢 SAP GUI oder Web GUI | ➖ | 🟢 SAP GUI oder Web GUI, direkt zum Objekt |

*Erweitertes ADT* ist kein Editor: Es ist der ABAP-Service, der IDEA das gibt, was das Standard-ADT nicht bereitstellt. Ohne ihn öffnet IDEA die mit **AMP** markierten Objekte in der SAP GUI. In S/4HANA (NetWeaver 7.52 oder höher) bringt das Standard-ADT eigene Editoren für weitere Dictionary-Objekte und für Textelemente mit. Die KI-Funktionen von SAP (Joule) sind in ECC nicht verfügbar. RAP und RAP-OData-Services ebenfalls nicht: In ECC werden OData-Services mit SEGW in der SAP GUI erstellt.

---

## So funktioniert es

1. **Richten Sie Ihre SAP-Verbindungen ein** mit `IDEA: SAP-Verbindungen verwalten`. Legen Sie alle SAP-Systeme an, mit denen Sie arbeiten möchten: So können Sie im KI-Chat angeben, gegen welches System gearbeitet werden soll. Markieren Sie die Verbindungen, deren MCP-Server mit VS Code starten soll (das bewirkt nichts in den SAP-Systemen: Der MCP-Server lauscht lediglich auf Ihrem Rechner), und wählen Sie die Verbindung, die beim Öffnen von VS Code aktiv ist.
2. **Suchen Sie das Objekt**, das Sie brauchen, im Seitenbereich «IDEA».
3. **Bitten Sie Ihre KI**, die Änderung vorzuschlagen, oder nehmen Sie sie selbst vor, mit Autovervollständigung, Formatierung und Navigation zur Definition.
4. **Sichern und aktivieren Sie per Tastenkürzel** (`Ctrl+S` und `Ctrl+F3`). IDEA kümmert sich um Sperre, Transportauftrag und Aktivierung.

Sie müssen das Objekt nicht öffnen, bevor Sie Ihre KI um etwas bitten: Bei aktiver MCP-Verbindung kann sie es selbst suchen, lesen, im Editor öffnen und Ihnen die Änderung vorschlagen.

> Damit Ihre KI das volle Potenzial von IDEA nutzt, bitten Sie sie ausdrücklich, die MCP-Werkzeuge von IDEA zu verwenden, um aus SAP zu lesen und die Änderungen im Editor vorzuschlagen.

---

## Quelltext-Editor: wie in der SAP GUI, aber in VS Code

Ein direkt im Tab eingebetteter Quelltext-Editor (WebView) mit derselben Engine, die auch VS Code verwendet (Monaco), darauf ausgelegt, gegen SAP genau wie in SE24/SE38 zu arbeiten, mit allen Funktionen direkt zur Hand.

**Klassen bearbeiten wie in der SAP GUI**
- **Vollständiger Quelltext oder blockweise** (`Ctrl+Alt+B`): Wechseln Sie zwischen der vollständigen Klasse und nur der Methode, die Sie interessiert, mit ihrer *Deklaration* oben und ihrer *Implementierung* unten, beide bearbeitbar und mit demselben Bildlauf, genau wie in SE24.
- **Beschreibungen**: Bearbeiten Sie in einer eigenen Tabelle die Kurztexte von Attributen, Typen, Methoden, Ereignissen und Parametern der Klasse oder des Interfaces, ohne den Editor zu verlassen; sie werden zusammen mit dem übrigen Quelltext gesichert.
- **Schaltfläche Komponente öffnen**: öffnet die Textelemente (REPT), den GUI-Status/-Titel (CUA) und die Dynpros des Objekts sowie die lokalen Includes der Klasse: Definitionen (`CCDEF`), Implementierungen (`CCIMP`), Makros (`CCMAC`) und ABAP-Unit-Testklassen (`CCAU`), jedes in seinem eigenen Tab.

**Von der KI vorgeschlagene Änderungen**
- Schlägt die KI eine Änderung vor, öffnet sich das Fenster *Von der KI vorgeschlagene Änderung* mit den Unterschieden zwischen dem aktuellen und dem vorgeschlagenen Quelltext, wahlweise als gesamter Quellcode oder nur die Änderungen.
- *Übernehmen* wendet die Änderung im Editor als rückgängig zu machende Bearbeitung an (`Ctrl+Z`), **ohne in SAP zu sichern**: Sie prüfen sie, sichern und aktivieren sie selbst. *Ablehnen* verwirft sie.
- Ein Countdown zeigt die verbleibende Zeit für die Prüfung; bei null werden Sie gefragt, ob Sie die Prüfung fortsetzen oder die Änderung verwerfen.

**Verwendungsnachweis**
- **Schaltfläche Verwendungen** (`Ctrl+Shift+F3`): listet auf, wo der Bezeichner unter dem Cursor verwendet wird: Klasse, Interface, Methode, Attribut, Variable, Programm, Funktion, Typ, Datenelement, Tabelle, Struktur oder Domäne.
- Jede Verwendung zeigt Objekttyp, Namen, Zeile und die vollständige Anweisung; ein Klick auf die Zeile öffnet das Objekt an dieser Stelle.
- Von einem `MESSAGE e001(zklasse)` oder einem `MESSAGE ID 'ZKLASSE' ... NUMBER '001'` navigiert `F2` zur Nachrichtenklasse mit dem Fokus auf dieser Nachricht.

**Debugging aus dem Editor**
- **Schaltfläche Breakpoint** (`F9`): setzt oder entfernt einen Breakpoint in der Cursorzeile; er wird am Rand rot markiert.
- **Schaltfläche Ausführen** (`Ctrl+F8`): öffnet das Objekt in der Web GUI, um es zu starten und an den Breakpoints anzuhalten.

**Volle Kontrolle über die Wartezeiten gegenüber SAP**
- Während gegen SAP gesperrt, gesichert, geprüft, aktiviert oder formatiert wird, sperrt sich der gesamte Editor (eine Ebene zeigt an, was gerade geschieht), damit Sie nicht weiterschreiben oder eine weitere Aktion auslösen können, während SAP antwortet.
- Braucht SAP zu lange, entsperrt sich der Editor von selbst und warnt Sie, statt Sie warten zu lassen, ohne zu wissen, was passiert.
- Der Status des Objekts (*Unverändert*, *Geändert, nicht gesichert* oder *Geändert, nicht aktiviert*) ist immer in der eigenen Leiste des Editors zu sehen.

**Die gesamte Bedienung mit einem Klick, in der eigenen Werkzeugleiste**
- Schaltflächen für Ändern/Anzeigen, Sichern, Prüfen, Aktivieren, Suchen und Ersetzen, Versionshistorie (mit Diff-Vergleich), Änderungen der Sitzung, Beschreibungen, Komponente öffnen, Verwendungen, Meldungen, Maximieren und Schließen, ohne Umweg über die Befehlspalette.
- **Prüfen** (`Ctrl+F2`) prüft die Syntax des aktuellen Quelltexts in SAP, ohne ihn zu sichern.
- **Maximieren** (`Ctrl+K Z`) schaltet den Tab in den Vollbildmodus (Zen-Modus von VS Code) und stellt ihn wieder her.
- **Konfigurierbare Tastenkürzel** je Aktion (Schaltfläche *Tastenkürzel*), mit Konfliktprüfung und einheitlich für alle VS Code-Fenster.
- Snippets, Autovervollständigung gegen SAP und KI-Codevorschläge (Claude, Gemini oder die Modelle von VS Code, etwa Copilot) direkt im Editor.

Auch die Editoren für Textelemente, Dictionary, GUI-Status/-Titel, Dynpros und Nachrichtenklassen haben eine eigene Schaltfläche *Schließen* in der Leiste.

---

## ABAP-Debugger

Debuggen Sie in VS Code die Programme, die in SAP laufen, mit einem eigenen Fenster für jede Ausführung.

1. **IDEA: ABAP-Debugging starten** lässt die aktive Verbindung auf Ausführungen in SAP lauschen.
2. Setzen Sie Breakpoints im Editor mit `F9` (oder mit der Schaltfläche *Breakpoint*).
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
2. `Ctrl+Shift+P` → **IDEA: SAP-Verbindungen verwalten** → legen Sie Ihre SAP-Systeme an.
3. Wählen Sie die aktive Verbindung in der Statusleiste (oder markieren Sie sie als *Autoverbindung*, damit sie beim Öffnen von VS Code automatisch aktiv wird).
4. Verbinden Sie Ihren KI-Assistenten mit dem MCP-Server der Verbindung (siehe *Aktive Verbindung und MCP-Server* in der technischen Referenz).

Fertig: Die Erweiterung sucht, bearbeitet, sichert und aktiviert bereits gegen SAP, und Ihr KI-Assistent kann analysieren, recherchieren und Ihnen Änderungen vorschlagen.

> 💡 So ermitteln Sie die Adresse Ihres SAP-Systems.
- Öffnen Sie die Transaktion SICF und führen Sie sie aus
- Klappen Sie den Baum auf und suchen Sie /default_host/sap/bc/adt
- Führen Sie über das Kontextmenü den Befehl „Service testen“ aus
- Der Webbrowser öffnet sich; die Adresse bzw. URL des SAP-Systems ist der angezeigte `http(s)://Server:Port`

![Transaktion SICF](image.png)

![Adresse bzw. URL des Systems](image-1.png)

---

## MCP-Server: Ihre KI arbeitet direkt in SAP

Der MCP-Server ermöglicht es einem KI-Assistenten, das verbundene SAP-System abzufragen und Änderungen am ABAP-Code vorzuschlagen. Er arbeitet nicht auf lokalen Kopien: Er liest direkt aus SAP, und die vorgeschlagenen Änderungen laufen über den Editor von IDEA, mit denselben Garantien für Sperre, Transportauftrag und Aktivierung wie der Rest der Erweiterung.

**Was die KI tun kann:**
- Abfragen, mit welchem SAP-System sie verbunden ist.
- Objekte nach Namen suchen und ihren Quelltext lesen.
- Ein Objekt im Editor von IDEA öffnen.
- Den Quelltext so lesen, wie er im Editor steht (mit noch nicht gesicherten Änderungen), sowie die Auswahl.
- Eine Änderung im Editor vorschlagen, die Sie übernehmen oder ablehnen.
- Daten aus SAP-Tabellen abfragen und Dumps analysieren *(erweiterte Funktionen)*.

Die KI sichert und aktiviert nicht direkt in SAP: Das tun Sie im Editor, sobald Sie mit der Änderung einverstanden sind.

**Verbindung aus Ihrem MCP-Client:** In VS Code integrierte Clients erkennen ihn automatisch; in externen Clients (Claude Code, Cursor…) fügen Sie einen Server vom Typ `http` hinzu, der auf `http://127.0.0.1:<Port>/mcp` zeigt (Port je Verbindung konfigurierbar, zum Beispiel `4856`).

---

## 🔐 Sicherheit und Kontrolle

- IDEA speichert keinen Quellcode in der Cloud oder in Dateien auf Ihrem Rechner: Alles wird direkt gegen Ihr SAP-System gelesen und gesichert, und der geöffnete Quelltext existiert nur im Editor-Tab, der ihn beim Schließen verwirft.
- Kennwörter und API-Schlüssel werden verschlüsselt im sicheren Speicher von VS Code abgelegt, nie im Klartext oder in den Einstellungen.
- Von der KI vorgeschlagene Änderungen werden immer als Unterschiede angezeigt und nur angewendet, wenn Sie sie übernehmen; auch dann werden sie erst in SAP gesichert, wenn Sie sichern.
- Der MCP-Server lauscht nur auf `127.0.0.1` (Ihr eigener Rechner).
- Datenabfragen sind reine Abfragen: Sie ändern niemals Tabellendaten.
- Wenn Sie bei einer Verbindung «Entwicklung erlaubt» deaktivieren, ist garantiert, dass die KI in diesem System nie etwas ändert: weder Objekte noch Daten.
- Dieselbe Verbindung kann nicht in zwei VS Code-Fenstern gleichzeitig aktiv sein. Und damit keine Version mit einer anderen verwechselt wird, kann dasselbe Objekt nicht gleichzeitig mit zwei verschiedenen Verbindungen im selben Fenster (zum Beispiel Entwicklung und Produktion) bearbeitet werden, noch mit derselben Verbindung in zwei Fenstern. Anzeigen ist immer möglich.

---

## Erweiterte Funktionen (lizenziert)

Mit einer kleinen Komponente in Ihrem SAP-System (konfiguriert in `idea.endpointAmpliacionADT`) schaltet IDEA in VS Code frei, was nicht einmal das Standard-ADT von SAP bietet:

- **Datenabfragen**: Die KI kann SAP-Tabellen abfragen (nur lesend). Erst damit kann die KI ihr volles Potenzial entfalten.
- **Dumps jedes Datums (ST22)**, nicht nur die der letzten 24 Stunden wie im Standard-ADT, und für die KI optimiert: kompakte Liste, Detail nur für den relevanten Dump und vollständige Daten nur bei Bedarf, sodass die KI deutlich weniger Tokens verbraucht.
- **Programme und Klassen anlegen**, mit ihrem leeren Grundgerüst.
- **Beschreibungen von Klassen und Interfaces**: Kurztexte von Attributen, Methoden und Parametern, direkt im Editor bearbeitbar.
- **Textelemente (REPT)** von Programmen, Klassen und Interfaces: direkte Bearbeitung, ohne SE38/SE24.
- **Data Dictionary**: Datenelemente, Strukturen, Tabellen, Domänen und Tabellentypen, mit Querverweis-Navigation zwischen ihnen.
- **GUI-Status / -Titel** von Programmen: Anlegen, Löschen und visuelle Bearbeitung von Funktionen, Status und Drucktastenleiste.
- **Dynpros (SE51)**: visueller Editor für Felder und Container, mit Prüfung beim Sichern.

Ohne diese Komponente bleiben diese Aktionen verfügbar: Sie öffnen das Objekt einfach in der klassischen SAP GUI statt in VS Code.

📩 **Möchten Sie die Volllizenz für Ihr Team oder Ihre Beratung?** Schreiben Sie an [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Technische Referenz

<details>
<summary><strong>📋 Befehle und Tastenkürzel</strong></summary>

**Tastenkürzel des Quelltext-Editors**

Dies sind die Standard-Tastenkürzel. Alle lassen sich über die Schaltfläche *Tastenkürzel* des Editors (oder die Einstellung `idea.editor.atajosWebview`) ändern und haben im Editor Vorrang vor denen von VS Code. Aktionen ohne Standard-Tastenkürzel (Historie, Änderungen, Komponente öffnen, Beschreibungen, Meldungen) sind immer in der Werkzeugleiste erreichbar.

| Aktion | Tastenkürzel | Beschreibung |
|---|---|---|
| Ändern / Anzeigen | `Ctrl+F1` | Wechselt zwischen Bearbeitungsmodus (sperrt das Objekt in SAP) und Anzeigemodus (gibt es frei). |
| Sichern | `Ctrl+S` | Formatiert und sichert in SAP. Ist das Objekt transportierbar, wird der Transportauftrag **vor** dem Sichern abgefragt. |
| Prüfen | `Ctrl+F2` | Prüft die Syntax des aktuellen Quelltexts in SAP, ohne ihn zu sichern. |
| Aktivieren | `Ctrl+F3` | Sichert, falls es Änderungen gibt, und aktiviert das Objekt in SAP. |
| Bearbeitung abbrechen | `Ctrl+Shift+U` | Verwirft nicht gesicherte Änderungen und kehrt in den Anzeigemodus zurück. |
| Formatieren | `Shift+F1` | Formatiert den Quelltext mit der konfigurierten Engine. |
| Editor schließen | `Ctrl+W` | Schließt den Tab; bei nicht gesicherten oder nicht aktivierten Änderungen wird nachgefragt. |
| Kommentieren / Kommentar entfernen | `Ctrl+<` | Kommentiert die ausgewählten Zeilen mit `*` in Spalte 1 im SAP-Stil ein oder aus. |
| Zeilen verbinden | `Ctrl+Shift+J` | Führt mehrere Zeilen zu einer einzigen Anweisung in möglichst wenigen Zeilen zusammen. |
| Anweisung aufteilen | `Ctrl+Shift+K` | Teilt eine lange Anweisung (`SELECT`, `CALL METHOD` usw.) auf mehrere Zeilen auf. |
| DATA / TYPES aufteilen | `Ctrl+Shift+D` | Trennt verkettete `DATA:` / `TYPES:`-Deklarationen in einzelne Anweisungen. |
| Blockliste | `Ctrl+Alt+M` | Filterbare Liste zum Springen zu einer METHOD, einer FORM, einem MODULE oder einem Ereignis des Quelltexts. |
| Zum Blockanfang / -ende | `Ctrl+Shift+↑` / `Ctrl+Shift+↓` | Springt zum Anfang oder Ende des Blocks, in dem der Cursor steht. |
| Blockansicht / vollständiger Quelltext | `Ctrl+Alt+B` | (Klassen) Wechselt zwischen der vollständigen Klasse und der aktuellen Methode. |
| Zur Definition | `F2` | Navigiert zur Definition des Objekts unter dem Cursor, wie in der SAP GUI. |
| Zurück / vorwärts | `Alt+←` / `Alt+→` | Durchläuft die beim Navigieren besuchten Positionen. |
| Suchen / Ersetzen im Editor | `Ctrl+F` / `Ctrl+H` | Schnelles Suchen und Ersetzen des Editors selbst. |
| Suchen und Ersetzen (Fenster) | `Ctrl+Shift+F` | Suchfenster nach ganzem Wort oder Wortteil, im aktuellen Block oder im ganzen Quelltext, mit filterbarer Ergebnisliste und Vorschau der Ersetzung. |
| Verwendungsnachweis | `Ctrl+Shift+F3` | Wo der Bezeichner unter dem Cursor verwendet wird. |
| Fehlermeldungen schließen | `Ctrl+Q` | Schließt alle im Editor sichtbaren Fehlermeldungen. |
| Breakpoint in der Zeile | `F9` | Setzt oder entfernt einen Breakpoint in der Cursorzeile. |
| In der Web GUI ausführen | `Ctrl+F8` | Öffnet das Objekt in der Web GUI, um es auszuführen. |
| Maximieren / wiederherstellen | `Ctrl+K Z` | Schaltet den Tab in den Vollbildmodus (Zen-Modus von VS Code) und stellt ihn wieder her. Nicht konfigurierbar. |

Außerdem: Autovervollständigung gegen SAP (`Ctrl+Space`) und Code-Faltung.

**VS Code-Befehle** (`Ctrl+Shift+P`)

| Befehl | Beschreibung |
|---|---|
| `IDEA: SAP-Verbindungen verwalten` | Fügt verfügbare SAP-Systeme hinzu, bearbeitet oder löscht sie. |
| `IDEA: Aktive Verbindung wechseln` | Wählt, gegen welches SAP-System dieses Fenster arbeitet. Auch per Klick auf die Verbindung in der Statusleiste. |
| `IDEA: Alle Verbindungen schließen` | Schließt die aktive Verbindung und stoppt die MCP-Server dieses Fensters. |
| `IDEA: MCP-Server starten` | Startet den MCP-Server einer Verbindung. |
| `IDEA: MCP-Server stoppen` | Stoppt einen laufenden MCP-Server. |
| `IDEA: ABAP-Debugging starten` | Lässt die aktive Verbindung auf Ausführungen in SAP lauschen; jede, die an einem Breakpoint anhält, öffnet ihr Debugging-Fenster. |
| `IDEA: Breakpoint in der aktuellen Zeile` | Setzt oder entfernt einen Breakpoint in der Cursorzeile (`F9` im Editor). |
| `IDEA: ABAP-Debugging beenden` | Entfernt die in SAP gesetzten Breakpoints, beendet das Lauschen und schließt die Debugging-Fenster. |
| `IDEA: SAP GUI öffnen` | Öffnet ein Fenster der klassischen SAP GUI gegen die gewählte Verbindung. |
| `IDEA: Anthropic-API-Schlüssel speichern` | Speichert verschlüsselt den Schlüssel für KI-Vorschläge mit Claude. |
| `IDEA: Gemini-API-Schlüssel speichern` | Speichert verschlüsselt den Schlüssel für KI-Vorschläge mit Gemini. |
| `IDEA: README anzeigen (VS Code-Sprache)` | Öffnet dieses README in der Sprache des Editors. |

</details>

<details>
<summary><strong>⚙️ Vollständige Konfiguration</strong></summary>

Einstellungen unter `idea.*` (Datei → Einstellungen → Einstellungen, oder im Abschnitt «Konfiguration» des IDEA-Bereichs).

**Formatierung (Pretty Printer)**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (Standard), `sapConfig` | Engine für *Formatieren* und beim Sichern. `extension`: der eigene Formatierer. `sapConfig`: der in SAP konfigurierte Pretty Printer. |
| `idea.prettyprinter.indentation` | `true` (Standard), `false` | Aktiviert oder deaktiviert die automatische Einrückung. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (Standard), `false` | Entfernt doppelte Leerzeichen oder nicht. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (Standard), `lowerKeywords`, `upperAll`, `lowerAll` | Groß-/Kleinschreibung: nur Schlüsselwörter oder der gesamte Code. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (Standard), `modoSe24`, `estandar` | Einrückung von `METHOD` / `ENDMETHOD` (nur Klassen). `auto`: behält vorhandene Leerzeichen bei. `modoSe24`: Spalte 0. `estandar`: eine Ebene (2 Leerzeichen). |
| `idea.prettyprinter.formatScope` | `fullFile` (Standard), `currentMethodOnly` | Umfang der Formatierung in Klassen und Interfaces: der ganze Quelltext oder nur die Methode am Cursor (beim Sichern nur die geänderten Methoden). |

**Quelltext-Editor**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (Standard), `false` | Beim Einfügen eines Methoden- oder Funktionsaufrufs mit `Ctrl+Space` wird der Kommentar jedes Parameters mit eingefügt. Bei `false` nur die Parameter. |
| `idea.editor.sugerenciasIa.proveedor` | `desactivado` (Standard), `vscode`, `anthropic`, `gemini` | Inline-KI-Codevorschläge (Geistertext; `Tab` übernimmt sie), nur im Bearbeitungsmodus und nach 500 ms ohne Tippen. `vscode`: die in VS Code bereits verfügbaren Modelle (zum Beispiel Copilot), ohne eigenen Schlüssel. `anthropic` und `gemini`: die jeweilige API mit Ihrem Schlüssel. |
| `idea.editor.sugerenciasIa.modelo` | Modellname (standardmäßig leer) | Modell für die Vorschläge. Bei `vscode` die Modellfamilie; bei `anthropic` oder `gemini` die Modell-ID. Leer: das Standardmodell des Anbieters. |
| `idea.editor.atajosWebview` | Objekt Aktion → Tastenkombination | Tastenkürzel des Quelltext-Editors, die vom Standard abweichen (leere Zeichenkette = kein Tastenkürzel). Änderung über die Schaltfläche *Tastenkürzel* des Editors. |

**Verbindungen und MCP-Server**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.mcpServer.connections` | Liste der SAP-Systeme | Verfügbare Systeme. Bearbeitung mit «IDEA: SAP-Verbindungen verwalten». Das Kennwort wird **nicht** hier gespeichert: Es wird abgefragt und verschlüsselt im sicheren Speicher von VS Code abgelegt. Felder jeder Verbindung in der folgenden Tabelle. |
| `idea.mcpServer.config` → `mcpInicial` | Name einer Verbindung (standardmäßig leer) | Verbindung, die beim Öffnen von VS Code **aktiv** ist. Leer = keine. |
| `idea.mcpServer.confirmWrites` | `true` (Standard), `false` | Fragt (mit Diff) nach Bestätigung, bevor die KI direkt in SAP sichert oder aktiviert. Diese Werkzeuge werden der KI derzeit nicht bereitgestellt: Ihre Änderungen kommen immer als Vorschlag im Editor an. |

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
| Entwicklung erlaubt | Nein (`true`) | Wenn deaktiviert, ist die Verbindung **nur lesend**: Die KI kann nur suchen, lesen, im Anzeigemodus öffnen, Daten abfragen und Dumps analysieren; sie kann weder Änderungen vorschlagen noch sichern oder aktivieren. Gedacht für Produktivsysteme. |
| Automatischer Start | Nein (`false`) | Startet den MCP-Server dieser Verbindung beim Öffnen von VS Code ohne Nachfrage. Mehrere Verbindungen können markiert werden, damit mehrere Server gleichzeitig laufen. |

**Debugger**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.depuracion.atajos` | Objekt Aktion → Tastenkombination | Tastenkürzel des Debugging-Fensters, die vom Standard abweichen: `F5` Einzelschritt, `F6` Ausführen, `F7` Return, `F8` Weiter, `F9` Breakpoint, `Shift+F9` weitere Breakpoints, `Shift+F4` Watchpoint, `F2` Variable hinzufügen, `F12` zur Anweisung springen, `F10` Layout. Sie lassen sich auch über die Schaltfläche *Tastenkürzel* des Panels ändern. |

**Erweiterte Funktionen und SAP GUI**

| Option | Werte | Wirkung |
|---|---|---|
| `idea.endpointAmpliacionADT` | Servicepfad (standardmäßig leer), z. B. `/sap/serviciosazure/` | Aktiviert die erweiterten Funktionen (Datenabfragen, Dumps jedes Datums, Beschreibungen, Textelemente, Dictionary, GUI-Status/-Titel, Dynpros). Bleibt es leer, öffnen diese Aktionen das Objekt in der SAP GUI. |
| `idea.sapGui.sapshcutPath` | Pfad zu `sapshcut.exe` (standardmäßig leer) | Nur, wenn die SAP GUI nicht an einem Standardort oder im PATH liegt. |
| `idea.navigation.gui` | `sapGui` (Standard), `webGui` | Beim Navigieren zu einem Objekt, das die Erweiterung nicht bearbeitet: klassische SAP GUI (`sapshcut.exe`; benötigt die *SAP-System-ID*) oder Web GUI im Browser. |

</details>

<details>
<summary><strong>🔌 Aktive Verbindung und MCP-Server</strong></summary>

IDEA unterscheidet zwei Begriffe:

- **Aktive Verbindung**: das SAP-System, gegen das *dieses Fenster* von VS Code arbeitet (Suche, Bearbeitung, Aktivierung). Sie wird in der Statusleiste angezeigt und gewechselt. Beim Öffnen von VS Code wird die in `mcpInicial` angegebene aktiviert. Dieselbe Verbindung kann nicht in zwei Fenstern gleichzeitig aktiv sein. Beim Wechsel der Verbindung schließt IDEA zuerst alles, was von der vorherigen geöffnet ist (mit Rückfrage bei nicht gesicherten Änderungen).
- **MCP-Server**: einer pro Verbindung, jeder auf seinem eigenen Port. Mehrere können gleichzeitig laufen, sodass die KI parallel in DEV arbeiten und QAS abfragen kann.

**Ihren MCP-Client verbinden:**
- **In VS Code integrierte Clients**: IDEA veröffentlicht automatisch den Server der aktiven Verbindung (`IDEA – <Verbindung>`); nichts zu konfigurieren.
- **Externe Clients** (Claude Code, Cursor…): Fügen Sie einen Server vom Typ `http` hinzu, der auf `http://127.0.0.1:<Port>/mcp` zeigt, mit dem *MCP-Port* der Verbindung. Einen pro Verbindung, die Sie nutzen möchten.

**Für die KI verfügbare MCP-Werkzeuge**

| Werkzeug | Wirkung | Nur lesend |
|---|---|:---:|
| `abap_connection_info` | Gibt an, mit welchem SAP-System der Server verbunden ist. | ✅ |
| `abap_search_object` | Sucht Objekte nach Namen (`*` als Platzhalter). | ✅ |
| `abap_read_object_source` | Liest den Quelltext eines Objekts aus SAP. | ✅ |
| `abap_open_object` | Öffnet ein Objekt im Quelltext-Editor von IDEA. | ✅ |
| `abap_editor_get_fuente` | Liest den Quelltext so, wie er im Editor steht, mit noch nicht gesicherten Änderungen, und seinen Zustand: Modus, aktueller Block, Cursor und Auswahl. | ✅ |
| `abap_editor_get_seleccion` | Liest den im Editor ausgewählten Text und seine Position. | ✅ |
| `abap_editor_proponer_cambio` | Schlägt eine Änderung am im Editor geöffneten Quelltext vor: Der Benutzer sieht die Unterschiede und übernimmt oder lehnt sie ab. Bei Übernahme wird sie im Editor angewendet (rückgängig zu machen), ohne in SAP zu sichern. | — |
| `abap_editor_esperar_propuesta` | Wartet weiter auf die Entscheidung des Benutzers zu einer vorgeschlagenen Änderung, wenn die Prüfung länger dauert, als der MCP-Client in einem einzigen Aufruf warten lässt. | — |
| `abap_get_datos` | Greift schreibgeschützt auf das SAP-System zu, um dessen Daten zu lesen *(erweiterte Funktion)*. | ✅ |
| `abap_list_dumps_24h` | Listet Laufzeitfehler der letzten 24 Stunden auf (Standard-ADT-Feed). | ✅ |
| `abap_list_dumps` | Listet Laufzeitfehler jedes Datums auf (entspricht ST22), in kompakter Form *(erweiterte Funktion)*. | ✅ |
| `abap_get_dump_detalle` | Liefert das Detail eines Dumps: ST22-Zusammenfassung und Aufrufstack; Variablen oder der vollständige Dump nur auf Anfrage *(erweiterte Funktion)*. | ✅ |

Die Spalte *Nur lesend* zeigt die Werkzeuge, die bei Verbindungen mit deaktiviertem **Entwicklung erlaubt** verfügbar sind.

Aus Sicherheitsgründen werden die Werkzeuge, die direkt in SAP sicherten oder aktivierten (`abap_write_object_source`, `abap_activate_object` und `abap_llamar_herramienta_desarrollo`), der KI nicht bereitgestellt: Die KI schlägt vor, und Sie prüfen, sichern und aktivieren im Editor.

</details>

<details>
<summary><strong>🖥️ Der Seitenbereich «IDEA» im Detail</strong></summary>

Das IDEA-Symbol in der Aktivitätsleiste öffnet zwei Abschnitte. Codesuche und Versionshistorie befinden sich im Quelltext-Editor selbst (Schaltflächen *Suchen* und *Historie*).

**1. SAP-Objektsuche**: sucht Objekte im SAP-System der aktiven Verbindung und öffnet sie in VS Code (erfordert den laufenden MCP-Server der Verbindung). Der Name akzeptiert `*` als Platzhalter.
- **Programm / Report**, **Klasse** und **Funktionsbaustein**: werden im Quelltext-Editor im Anzeigemodus geöffnet.
- **Klassen**: Schaltflächen zum Öffnen ihrer lokalen Includes: `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` und `<TEST>` (ABAP-Unit-Testklassen).
- **Funktionsgruppen**: zeigt ihren Baum (Funktionsbausteine, Includes und weitere Teile), um jedes Teil einzeln zu öffnen.
- **Datenelement**, **Struktur / Tabelle**, **Domäne** und **Tabellentyp**: werden im Dictionary-Editor geöffnet *(erweiterte Funktion)*.
- **Schaltflächen REPT, CUA und DYNP** (je nach Objekttyp): öffnen die Editoren für Textelemente, GUI-Status/-Titel und Dynpros *(erweiterte Funktionen)*.
- **Nachrichtenklasse**: öffnet sich im Editor für Nachrichtenklassen (über das Standard-ADT, ohne erweiterte Komponente).
- **Schaltfläche Neu**: legt ein Programm, eine Klasse, eine Nachrichtenklasse oder ein Dictionary-Objekt (Datenelement, Domäne, Struktur/Tabelle, Tabellentyp) mit Name und Paket an. Ohne die erweiterte Komponente können nur Nachrichtenklassen angelegt werden.
- Liefert die Suche ein einziges Ergebnis, wird es direkt geöffnet. Speichert **zuletzt verwendete** und **historische** Suchen.
- Objekte, die die Erweiterung nicht bearbeiten kann, werden in der klassischen SAP GUI (oder in der Web GUI, je nach `idea.navigation.gui`) geöffnet.

**2. Konfiguration**: schneller Zugriff, ohne den Bereich zu verlassen, auf:
- SAP-Verbindungen: Tabelle mit *Name*, *Auto-Start* (ihr MCP-Server startet beim Öffnen von VS Code), *Autoverbindung* (die beim Öffnen von VS Code aktive) und *Entwicklung* (ob Entwicklung erlaubt ist); die übrigen Angaben (URL, Mandant, Benutzer, MCP-Port) erscheinen beim Überfahren der Zeile mit der Maus. Schaltfläche *Verbindungen verwalten…*.
- Pretty Printer: Engine, Umfang, Einrückung, doppelte Leerzeichen, Groß-/Kleinschreibung und Einrückung von `METHOD`.
- MCP-Server: Startverbindung und Schreibbestätigung.
- Navigation und SAP GUI: wo nicht bearbeitbare Objekte geöffnet werden, Pfad zu `sapshcut.exe` und ADT-Erweiterungsservice.
- Autovervollständigung und KI-Vorschläge: Parameterkommentare, Anbieter, Modell und API-Schlüssel.

**Versionshistorie** (Schaltfläche *Historie* des Editors): speichert eine Version des Objekts bei jedem Sichern oder Aktivieren einer echten Änderung und auch, wenn erkannt wird, dass das Objekt direkt in SAP geändert wurde. Sie gehört nur zum Tab: Beim Schließen geht sie verloren.
- Tabelle mit der neuesten Version oben, der Uhrzeit der Änderung, ob sie aktiviert wurde, ihrer Herkunft (*Lokal* oder *In SAP geändert*) und der Anzahl der Änderungen gegenüber der letzten Aktivierung und der vorherigen Version.
- *Änderungen anzeigen* zwischen zwei Versionen (Inline-Ansicht oder nebeneinander) und *Gesamtänderungen anzeigen* zwischen der Anfangs- und der aktuellen Version.
- *Version wiederherstellen*: überträgt ihren Inhalt in den Editor, ohne ihn zu sichern (rückgängig zu machen).

</details>

<details>
<summary><strong>🧩 Erweiterte Funktionen im Detail</strong></summary>

**Datenabfragen.** Sie ermöglichen der KI, die Daten Ihres SAP-Systems mit schreibgeschützten Abfragen zu untersuchen. Ohne sie sieht die KI den Code, aber nicht die Daten, und verliert einen Großteil ihrer Analysefähigkeit.

**Textelement-Editor (REPT).** Über die Schaltfläche *REPT* in der «SAP-Objektsuche» (oder *Komponente öffnen* im Editor), für ein Programm, eine Klasse oder ein Interface:
- Öffnet sich im Anzeigemodus (blauer Hintergrund).
- *Bearbeiten* sperrt das Objekt in SAP (bernsteinfarbener Hintergrund); bei Änderung einer Zelle erscheint 🔴 auf dem Tab.
- *Sichern und aktivieren* lädt die Texte nach SAP hoch (fragt bei Bedarf nach einem Transportauftrag) und behält die Sperre bei, um weiter zu bearbeiten.
- Beim Zurückkehren in den Anzeigemodus oder Schließen des Tabs wird die Sperre freigegeben.
- *Kopieren* überträgt die gesamte Texttabelle in die Zwischenablage.

**Dictionary-Editor.** Datenelemente, Strukturen / Tabellen, Domänen und Tabellentypen: Kopf, technische Optionen und Liste der Felder oder Werte. Öffnet sich im Anzeigemodus; *Bearbeiten* sperrt das Objekt und erlaubt, es mit derselben Transportauftragsverwaltung wie der Rest zu ändern und zu aktivieren. Der Kopf der Feldtabelle bleibt beim Scrollen fixiert; Spalten sind sortier- und filterbar. Aus den Zellen navigiert man zu anderen Datenelementen und Domänen.

**GUI-Status / -Titel (CUA).** Anlegen, Löschen und Bearbeiten von Titeln, Funktionen, Status und Standard-Drucktastenleiste.

**Dynpros (SE51).** Visueller Editor für Felder und Container (Rahmen, Subscreens, Tabstrips, Table Controls): Anlegen durch Platzieren des Elements per Klick, Erkennung von Überlappungen und Prüfung beim Sichern.

Alle folgen derselben Disziplin bei Sperre, Transportauftrag und Aktivierung wie die übrigen Objekte.

</details>

---

## Lizenz

Die Erweiterung ist unter der MIT-Lizenz frei nutzbar.

Wenn Sie an den erweiterten Funktionen interessiert sind, die die ABAP-Komponente *ADT Ampliado* (Erweitertes ADT) erfordern, wenden Sie sich für Bedingungen und Preise an Marcos Almeida Santolaria unter [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

[Español](README.md) · [English](README.en.md) · **Deutsch** · [Français](README.fr.md)
