# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Integrated Development Environment for ABAP

[Español](README.md) · **English** · [Deutsch](README.de.md) · [Français](README.fr.md)

> 💡 To read this README in another language inside VS Code, run **IDEA: Show README** (`Ctrl+Shift+P`): it opens automatically in your editor's language.

---

## Modern ABAP development, without leaving VS Code

**IDEA** turns Visual Studio Code into a complete ABAP development environment: connected in real time to your SAP system and ready to work side by side with the AI assistant you already use (Claude Code, GitHub Copilot, Cursor…).

No more copying and pasting code between SAP GUI and an AI chat. No more losing track of which object is locked, who touched it or whether it is still waiting to be activated. With IDEA everything happens inside the editor itself, with the same discipline of locks, transport requests and activation you already know from SAP — but with the speed of VS Code and the power of AI.

**In one sentence:** find an object → open it → ask your AI to change it (or edit it yourself) → activate it. All without leaving VS Code, all under control.

**In another sentence 😉:** An IDoc failed? → ask your AI to analyse it and tell you the fix → fix it. All without leaving VS Code, all under control.

---

## Why your team will love it

| | |
|---|---|
| ⚡ **Real speed** | Instant search for programs, classes, interfaces and dictionary objects, with search history. No transactions or nested menus. |
| 🤖 **AI with direct access to SAP** | Built-in MCP server: your AI assistant reads, writes and activates ABAP code directly in SAP, always showing a confirmation diff before touching anything. |
| 🌐 **Multi-system** | Several MCP servers running at once, one per system: your AI can write in DEV while querying data in PRD through a read-only connection. |
| 🔒 **Zero surprises** | Display mode by default, explicit lock to edit, transport requests and activation handled exactly as in standard SAP. |
| 🕘 **On-the-fly history** | Every save and every activation is recorded in the session: compare versions or restore an earlier one without leaving the editor. |
| 🎨 **Formatting that respects your diffs** | Its own formatter only touches the lines the developer has changed — no more accidentally reformatting whole files. |
| 🖥️ **Source editor just like SAP GUI** | Editor embedded right in the tab: display or edit mode, classes by block or in full, editable descriptions, direct navigation to REPT/CUA/Dynpros and local includes, and total control over the waits against SAP. |
| 🐞 **Built-in ABAP debugger** | Breakpoints from the editor and one debugging window per execution in SAP, in parallel: statement, method, function, FORM, exception or message breakpoints, watchpoints, value changes and editable internal tables. |
| 🔎 **Where-used** | Where-used list of the word under the cursor (`Ctrl+Shift+F3`) or of each message of a message class, with the statement of each use and a direct jump to the line. |
| ✉️ **Message classes** | Create and edit message classes (SE91) in a table, with their long text and their list of uses. |
| 🧯 **Dumps from any date, without burning tokens** *(extended feature)* | Your AI finds dumps from any date (not just the last 24 h that standard ADT returns): first a compact list with the key, error and position of each dump; then, only for the one that matters, the ST22 summary and the call stack. Variables or the full dump only when needed. Less text for the AI, fewer tokens and faster answers. |
| 🧩 **Beyond standard ADT** *(extended feature)* | Editing of text elements (REPT), data dictionary, GUI Status/Title screens and Dynpros — everything SAP's ADT won't let you touch outside SAP GUI. |

---

## What IDEA covers compared with other tools

Comparison on SAP ECC with NetWeaver 7.50 between SAP's ADT for Eclipse, other ABAP extensions for VS Code, the ABAP component “ADT Ampliado” (Extended ADT) and IDEA itself.

🟢 Covered · 🟡 Partial · 🔴 Not available · ➖ Handled by standard ADT · **AMP** Requires Extended ADT

| Feature | SAP ADT | Other extensions | Extended ADT | IDEA |
|---|---|---|---|---|
| **Objects with source code** | | | | |
| Programs, includes and reports | 🟢 | 🟢 | ➖ | 🟢 |
| Classes and interfaces | 🟢 | 🟢 | ➖ | 🟢 By blocks (method by method) or whole, as in SE24 |
| Local class includes <br><sub>`CCDEF · CCIMP · CCMAC · CCAU`</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Function groups and modules | 🟢 | 🟢 | ➖ | 🟢 Group tree; no creation |
| Class descriptions <br><sub>Short texts of methods, attributes and parameters</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Editable table in the editor |
| CDS views and type groups <br><sub>`DDLS · TYPE`</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Message classes <br><sub>`MSAG`</sub> | 🟢 | 🟢 | ➖ | 🟢 Creation, table editing, long text and where-used of each message |
| **Data dictionary** | | | | |
| Data elements <br><sub>`DTEL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Domains <br><sub>`DOMA`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Fixed values included |
| Structures <br><sub>`TABL`</sub> | 🟢 | 🟢 As source code | 🟢 | 🟢 **AMP** Field editor with navigation |
| Database tables <br><sub>`TABL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Table types <br><sub>`TTYP`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| **Texts and classic UI** | | | | |
| Text elements <br><sub>`REPT` · text symbols and selection texts</sub> | 🟡 Depends on release | 🟡 Depends on release | 🟢 | 🟢 **AMP** |
| GUI Status / Title <br><sub>`CUAD` · SE41</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Create, delete and edit functions, statuses and toolbar |
| Dynpros <br><sub>`DYNP` · SE51</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Visual editor for fields and containers |
| **RAP and OData** | | | | |
| RAP business objects <br><sub>`BDEF · SRVD` · NetWeaver 7.54 or S/4HANA only</sub> | 🟢 | 🟡 Depending on the extension, as source code | 🔴 | 🔴 |
| RAP generator <br><sub>Table, CDS, behaviour and service in one step · NetWeaver 7.54 or S/4HANA only</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| RAP OData services <br><sub>`SRVB` · service binding and Fiori preview · NetWeaver 7.54 or S/4HANA only</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| **Object lifecycle** | | | | |
| Search objects | 🟢 | 🟢 | ➖ | 🟢 With recent items and history |
| Create code objects <br><sub>Programs, classes and functions</sub> | 🟢 | 🟢 | 🟢 Programs and classes | 🟡 **AMP** Programs, classes and message classes; no functions |
| Create dictionary objects <br><sub>`DTEL · DOMA · TABL · TTYP`</sub> | 🟡 Structures only | 🟡 Structures only | 🟢 | 🟢 **AMP** |
| Display / Edit mode <br><sub>Explicit object lock, as in SE38</sub> | 🟡 Locks when you start typing | 🟡 Locks when you start typing | 🟢 Any object, dynpros too | 🟢 Ctrl+F1, state always visible |
| Transport request on save | 🟢 | 🟢 | 🟢 Open requests and request creation | 🟢 |
| Activation and inactive objects | 🟢 | 🟢 Mass activation | ➖ | 🟢 Warning about modified parts |
| Transport management <br><sub>Release, change owner, ATC on the request</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Versions and comparison | 🟢 | 🟢 Plus line authorship (blame) | ➖ | 🟡 Session history with diff |
| abapGit | 🟢 Plugin | 🟢 | ➖ | 🔴 |
| **Writing code** | | | | |
| Code completion and go to definition | 🟢 | 🟢 | ➖ | 🟢 F2 as in SAP GUI |
| Syntax check | 🟢 | 🟢 | ➖ | 🟢 |
| Formatting | 🟢 | 🟢 | ➖ | 🟢 SAP standard or the extension's own (only the modified lines) |
| Where-used list | 🟢 | 🟢 | ➖ | 🟢 Of the word under the cursor and of each message; with the statement of each use |
| Refactoring <br><sub>Rename, extract method</sub> | 🟢 | 🟡 Quick fixes | ➖ | 🔴 |
| SAP GUI-style utilities <br><sub>Comment with *, join and split statements, jump between blocks</sub> | 🟡 | 🔴 | ➖ | 🟢 |
| AI suggestions in the editor | 🔴 | 🟢 GitHub Copilot | ➖ | 🟢 Claude, Gemini or GitHub Copilot |
| **Testing and analysis** | | | | |
| Debugger | 🟢 | 🟢 | ➖ | 🟢 Several sessions in parallel; all kinds of breakpoints, watchpoints, configurable layout and shortcuts |
| ABAP Unit | 🟢 | 🟢 | ➖ | 🔴 |
| ATC / Code Inspector | 🟢 | 🟢 | ➖ | 🔴 |
| Performance traces | 🟢 | 🟢 | ➖ | 🔴 |
| Dumps from the last 24 hours <br><sub>ST22 · standard ADT feed</sub> | 🟢 | 🟢 | ➖ | 🟡 No screen: gets the dumps through standard ADT to hand them to the AI |
| Dumps from any date <br><sub>ST22 · between dates, with full detail and call stack</sub> | 🔴 Last 24 hours only | 🔴 Last 24 hours only | 🟢 | 🟡 **AMP** No screen: list and detail through Extended ADT, optimised to save AI tokens |
| Data queries <br><sub>Read-only SELECT</sub> | 🟢 Simple queries | 🟢 Simple queries | 🟢 Complex queries | 🟢 **AMP** Complex queries, for the AI |
| **AI and multiple systems** | | | | |
| MCP server for any AI assistant <br><sub>Claude Code, Copilot, Cursor…</sub> | 🔴 | 🟢 Depends on the extension | ➖ | 🟢 |
| Several systems at once <br><sub>For example, development and production</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Read-only connection <br><sub>For production systems</sub> | 🔴 | 🟡 Warning in production | 🟢 | 🟢 The AI cannot write or activate |
| Open unsupported objects in SAP GUI | - | 🟢 SAP GUI or Web GUI | ➖ | 🟢 SAP GUI or Web GUI, straight to the object |

*Extended ADT* is not an editor: it is the ABAP service that gives IDEA what standard ADT does not expose. Without it, IDEA opens the objects marked **AMP** in SAP GUI. On S/4HANA (NetWeaver 7.52 or later) standard ADT ships its own editors for more dictionary objects and for text elements. SAP's AI capabilities (Joule) are not available on ECC. Neither are RAP and RAP OData services: on ECC, OData services are built with SEGW in SAP GUI.

---

## How it works

1. **Set up your SAP connections** with `IDEA: Manage SAP Connections` — Define all the connections to the SAP systems you want to work with, so that from the AI chat you can say which environment it should work against; when VS Code starts, the MCP servers for each system will be connected (this does nothing in the systems, it just leaves the MCP server listening). Set one of the connections to start automatically with VS Code.
2. **Find the object** you need from the «IDEA» side panel.
3. **Ask your AI** to change it, or edit it yourself with code completion, formatting and go-to-definition.
4. **Activate it with a shortcut** (`Ctrl+F3`). IDEA handles the lock, the transport request and the activation for you.

There is no need to open the object manually before asking your AI for something: with the MCP connection active, it can find, read and change it directly in SAP by itself.

> To get the most out of IDEA, explicitly ask your AI to use IDEA's MCP tools to read and write in SAP, instead of editing the object by hand in the editor.

---

## Display mode / Edit mode

Objects opened from «SAP object search» start in **Display mode** (bluish background): they don't lock the object in SAP and won't let you type by mistake.

1. `Ctrl+F1` switches to **Edit mode**: locks the object in SAP.
2. Edit and save with `Ctrl+S`; every save in Edit mode also uploads the code to SAP.
3. `Ctrl+F3` formats and activates the object.
4. `Ctrl+F1` again, or `Ctrl+Shift+U` to discard changes, returns to Display mode and releases the lock. Closing the tab also releases the lock.

A 🔴 badge on the tab warns that there are saved changes pending activation.

---

## WebView source editor: just like SAP GUI, but in VS Code

A source code editor embedded right in the tab, with the same engine VS Code itself uses (Monaco), built to work against SAP just like in SE24/SE38 with plenty of built-in operations.

**Edit classes just like in SAP GUI**
- **Full source or by blocks**: switch between the whole class or just the method you care about, with its *declaration* on top and its *implementation* below, both editable and sharing the same scroll — just like in SE24.
- **Descriptions**: edit the short texts of attributes, types, methods, events and parameters of the class or interface in their own table, without leaving the editor; they are saved together with the rest of the source.
- **Navigate button**: jump straight to the object's text elements (REPT), GUI Status/Title (CUA) and screens (Dynpros), and to the class's local includes — definitions (`CCDEF`), implementations (`CCIMP`), macros (`CCMAC`) and ABAP Unit test classes (`CCAU`) — each one in its own tab.

**Where-used**
- **References button** (`Ctrl+Shift+F3`): lists where the identifier under the cursor is used — class, interface, method, attribute, variable, program, function, type, data element, table, structure or domain.
- Each use shows the object type, its name, the line and the full statement; click the row to open the object at that line.
- From a `MESSAGE e001(zclass)` or a `MESSAGE ID 'ZCLASS' ... NUMBER '001'`, `F2` navigates to the message class with the focus on that message.

**Debugging from the editor**
- **Breakpoint button** (`F9`): sets or removes a breakpoint on the cursor line; it is marked in red in the margin.
- **Run button** (`Ctrl+F8`): opens the object in Web GUI to launch it and stop at the breakpoints.

**Total control over the waits against SAP**
- While locking, saving, activating or formatting against SAP, the whole editor locks up (a layer shows what's happening) so you can't keep typing or launch another action while SAP is responding.
- If SAP takes too long, the editor unlocks itself and warns you, instead of leaving you waiting without knowing what's going on.
- The object's status — *Unmodified*, *Modified, not saved* or *Modified, not activated* — is always visible right in the editor's own bar.

**All the operations, one click away in its own toolbar**
- Buttons for Edit/Display, Save, Activate, Search and replace, Version history (with a built-in diff viewer), Session changes, Descriptions, Navigate and Messages — no need for the command palette.
- **Configurable keyboard shortcuts** per action, with conflict validation and shared across every VS Code window.
- Snippets, SAP code completion and AI code suggestions built right into the editor.

---

## ABAP debugger

Debug in VS Code the programs that run in SAP, with a window of its own for each execution.

1. **IDEA: Start ABAP debugging** makes the active connection listen for executions in SAP.
2. Set breakpoints in the editor with `F9` (or the *Breakpoint* button).
3. Run the program in SAP (for example, with the editor's *Run* button, which opens it in Web GUI).
4. When the execution reaches a breakpoint, a debugging window opens. If several executions arrive, one window opens for each, in parallel (up to 4; beyond that they are released without opening a window).
5. **IDEA: Stop ABAP debugging** removes the breakpoints set in SAP and closes the sessions.

**The debugging window**
- **Toolbar**: Step into (`F5`), Step over (`F6`), Return (`F7`), Continue (`F8`), breakpoint on the line (`F9`), other breakpoints (`Shift+F9`), watchpoint (`Shift+F4`), list of breakpoints and watchpoints, layout (`F10`) and shortcuts.
- **Fixed header**: program, include, block type and name, line, `SY-SUBRC` and `SY-TABIX`.
- **Code**: always in display mode; methods are shown by blocks as in the editor. Double-click the line number to set or remove a breakpoint; double-click or `F2` on a variable adds it to *Variables*; `F12` jumps to the statement at the cursor.
- **Variables, Locals and Globals**: name, value, technical type, absolute type and hexadecimal value. Values are changed with the pencil; structures expand; internal tables are shown by pages, with row insertion and deletion. Everything can be copied to the clipboard to paste into a spreadsheet.
- **Navigation**: the call stack (level, event type and event, program, include and line); double-click to view another level.
- **Other breakpoints**: ABAP statement, method (of a global or local class), function, FORM, class-based exception, message or source code, with an optional condition. They are remembered and set again on the program's next execution.
- **Watchpoints**: stop when a variable changes, with an optional condition.
- **Configurable screen layout**: you decide how many rows and columns and which frame goes in each cell (Code, Navigation, Variables, Locals, Globals). Layouts are saved by name and apply to all windows; the size of each frame is changed by dragging the bars between them.
- **Configurable keyboard shortcuts** for every action, from the panel itself (*Shortcuts* button) or with the `idea.depuracion.atajos` setting.

---

## Message classes (SE91)

From «SAP object search» (type *Message class*), or navigating with `F2` from a `MESSAGE`, the class opens in an editable table. It works entirely through standard ADT, without the extended component.

- It opens in Display mode; *Edit* locks the class and *Save* saves it, asking for the transport request when needed.
- Table with number, text, length and self-explanatory flag; it can be filtered by column and copied whole to the clipboard.
- Create and delete messages, with validation on save (unique 3-digit numbers, mandatory texts and maximum length).
- For each message: view its **long text**, see **where it is used** (with a direct jump to each use) or open it in SE91.
- With the *New* button of «SAP object search» an empty message class is created and opened in Edit mode.

---

## Quick start

1. Install the extension and reload VS Code.
2. `Ctrl+Shift+P` → **IDEA: Manage SAP Connections** → add your SAP systems or environments.
3. In the settings, define a local folder for temporary files (`idea.mcpServer.tempFilesPath`).
4. Reload the window (**Developer: Reload Window**).

Done: the extension now searches, edits and activates against SAP, and your AI assistant is ready to analyse, investigate, modify… whatever helps you.

---

## MCP server: your AI, working directly in SAP

The MCP server lets an AI assistant read and change ABAP code directly in the connected SAP system. It does not work on local copies: everything goes against SAP, with the same locking and activation guarantees as the rest of the extension.

**Development actions available to the AI:**
- Check which SAP system it is connected to.
- Search objects by name.
- Read an object's source code.
- Open an object in VS Code under the extension's control.
- Write an object's source code (with confirmation).
- Activate an object.

**Connecting from your MCP client:** add an `http` server pointing to `http://127.0.0.1:<port>` (configurable port, for example `4856`).

---

## 🔐 Security and control

- IDEA does not store source code in the cloud: everything is read and written directly against your SAP system. The source it opens is kept in temporary files on your computer, which are deleted as soon as you close the editing window.
- Passwords are stored encrypted in VS Code's secure storage, never in plain text or in the settings.
- With `idea.mcpServer.confirmWrites` (on by default), every write or activation proposed by the AI requires prior confirmation. It is also shown as a diff before being applied.
- The MCP server only listens on `127.0.0.1` (your own machine).
- Data queries are queries only, SELECT. They never modify table data.
- If you set the connection's "Allows development" to false, you are guaranteed that the AI will never change anything in the system, neither objects nor data.

---

## Extended features (licensed)

With a small component installed in your SAP system (configured in `idea.endpointAmpliacionADT`), IDEA unlocks inside VS Code what not even SAP's standard ADT offers:

- **Data queries** The AI can query SAP tables (read-only). This is what lets the AI reach its full potential.
- **Dumps from any date (ST22)**, not just the last 24 hours offered by standard ADT, and optimised for the AI: a compact list, detail only for the dump that matters and full data only when needed, so the AI spends far fewer tokens.
- **Create the empty skeleton of a class, program or interface**
- **Text elements (REPT)** of programs, classes and interfaces — direct editing, without SE38/SE24.
- **Data dictionary**: Data elements, structures, domains and table types, with cross-navigation between them.
- **GUI Status / Title** of programs: Create, delete and visually edit functions, statuses and the toolbar.
- **Dynpros (SE51)**: Visual editor for fields and containers, with validation on save.

Without this component configured, these actions are still available: they simply open the object in classic SAP GUI instead of VS Code.

📩 **Want the full license for your team or consultancy?** Write to [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Technical reference

<details>
<summary><strong>📋 Commands and keyboard shortcuts</strong></summary>

**Editing, saving and activation**

| Command | Shortcut | Description |
|---|---|---|
| `IDEA: Toggle Edit / Display Mode` | `Ctrl+F1` | Switches between Edit mode (locks the object in SAP) and Display mode (releases it). |
| `IDEA: Save ABAP object` | `Ctrl+S` | Saves locally and in SAP. If the object is transportable, asks for the transport request **before** saving anything. |
| `IDEA: Activate ABAP object` | `Ctrl+F3` | Formats the object and activates it in SAP. |
| `IDEA: Cancel changes and return to Display mode` | `Ctrl+Shift+U` | Discards unsaved changes and returns to Display mode. |
| `IDEA: Show blocks modified since the last activation` | — | (Classes and interfaces) Lists the methods and sections touched since the last activation and jumps to the chosen one. Also from the «N changes» button in the status bar. |
| `IDEA: Format Document` | `Shift+F1` | Formats the object with the configured engine. |

**Writing code**

| Command | Shortcut | Description |
|---|---|---|
| `IDEA: Toggle line comment (* in column 1)` | `Ctrl+<` | Comments or uncomments the selected lines with `*` in column 1, SAP style. |
| `IDEA: Join statement into as few lines as possible` | `Ctrl+Shift+J` | Joins several lines into a single statement. |
| `IDEA: Split Statement into Lines` | `Ctrl+Shift+K` | Splits a long statement (`SELECT`, `CALL METHOD`, etc.) into several lines. |
| `IDEA: Split declarative statement into Lines` | `Ctrl+Shift+D` | Splits chained `DATA:` / `TYPES:` declarations into individual statements. |

**Navigation and search**

| Command | Shortcut | Description |
|---|---|---|
| `IDEA: Find and Navigate to code block` | `Ctrl+Alt+M` / `Ctrl+Shift+Z` | Quick list to jump to a METHOD / FORM / MODULE / event in the file. |
| `IDEA: Go to block start` | `Ctrl+Shift+↑` / `Ctrl+Alt+PgUp` | Jumps to the start of the block the cursor is in. |
| `IDEA: Go to block end` | `Ctrl+Shift+↓` / `Ctrl+Alt+PgDn` | Jumps to the end of the block the cursor is in. |
| Go to definition | `F2` / `F12` / `Ctrl+Click` | Navigates to the definition of the object under the cursor. In ABAP files, `F2` replaces «Rename» (as in SAP GUI). |
| `IDEA: Find and replace` | `Ctrl+Shift+F` | Opens the «Code search» panel with focus on the search field. Always works, not only in the ABAP editor. |

**Debugging**

| Command | Shortcut | Description |
|---|---|---|
| `IDEA: Start ABAP debugging` | — | Makes the active connection listen for executions in SAP; each one that stops at a breakpoint opens its debugging window. |
| `IDEA: Breakpoint on the current line` | `F9` | Sets or removes a breakpoint on the cursor line. |
| `IDEA: Stop ABAP debugging` | — | Removes the breakpoints set in SAP, stops listening and closes the debugging windows. |
| Where-used list | `Ctrl+Shift+F3` | (Source editor) Where the identifier under the cursor is used. |
| Run in Web GUI | `Ctrl+F8` | (Source editor) Opens the object in Web GUI to run it. |

**Connections, MCP server and SAP GUI**

| Command | Shortcut | Description |
|---|---|---|
| `IDEA: Manage SAP Connections` | — | Adds, edits or deletes the available SAP systems. |
| `IDEA: Switch Active Connection` | — | Chooses which SAP system this window works against. Also by clicking the connection in the status bar. |
| `IDEA: Close All Connections` | — | Closes the active connection and stops this window's MCP servers. |
| `IDEA: Start MCP Server` | `Ctrl+Alt+S` | Starts the MCP server of a connection. |
| `IDEA: Stop MCP Server` | — | Stops a running MCP server. |
| `IDEA: Open SAP GUI` | — | Opens a classic SAP GUI window against the connection you choose. |
| `IDEA: Show README (VS Code language)` | — | Opens this README in the editor's language. |

Except for `Ctrl+Shift+F`, the shortcuts apply with the ABAP editor focused. In non-ABAP files, `Ctrl+F3` keeps its original VS Code function («Find next selection»). Also: **Format Document** (`Shift+Alt+F`), code completion (`Ctrl+Space`) and code folding.

</details>

<details>
<summary><strong>⚙️ Full configuration</strong></summary>

Settings under `idea.*` (File → Preferences → Settings, or from IDEA's «Settings» panel).

**Formatting (Pretty Printer)**

| Option | Values | What it does |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (default), `sapConfig` | Engine used by «Format Document» and before activating. `extension`: the built-in formatter. `sapConfig`: the Pretty Printer configured in SAP (only objects opened from «SAP object search»). |
| `idea.prettyprinter.indentation` | `true` (default), `false` | Enables or disables automatic indentation. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (default), `false` | Removes double spaces or not. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (default), `lowerKeywords`, `upperAll`, `lowerAll` | Upper/lower case: keywords only, or all code. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (default), `modoSe24`, `estandar` | Indentation of `METHOD` / `ENDMETHOD` (classes only). `auto`: keeps existing spaces. `modoSe24`: column 0. `estandar`: one level (2 spaces). |
| `idea.prettyprinter.formatScope` | `fullFile` (default), `currentMethodOnly` | When formatting via shortcut (classes only): the whole file or only the method where the cursor is. |

**Code completion**

| Option | Values | What it does |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (default), `false` | When inserting a method or function call with `Ctrl+Space`, includes each parameter's comment. With `false` only the parameters are inserted. |

**Connections and MCP server**

| Option | Values | What it does |
|---|---|---|
| `idea.mcpServer.connections` | List of SAP systems | Available systems. Edited with «IDEA: Manage SAP Connections». The password is **not** stored here: it is requested and stored encrypted in VS Code's secure storage. Fields of each connection in the next table. |
| `idea.mcpServer.config` → `mcpInicial` | Name of a connection (empty by default) | Connection that is **active** when VS Code opens. Empty = none. |
| `idea.mcpServer.confirmWrites` | `true` (default), `false` | Asks for confirmation (showing a diff) before the AI writes or activates code in SAP. |
| `idea.mcpServer.tempFilesPath` | Folder path (empty by default) | Folder where the temporary `.abap` files of «SAP object search» are created. **Required** to search and open objects. Files are deleted when their tab or VS Code is closed. |

**Fields of each connection**

| Field | Required | What it does |
|---|---|---|
| Name | Yes | System identifier (e.g. `DEV`, `QAS`). It is the name the AI and the status bar use to refer to it. |
| URL | Yes | Base URL of the SAP system (e.g. `https://myserver.mydomain.com:44300`). |
| Client | Yes | SAP client (e.g. `100`). |
| User | Yes | SAP user. |
| MCP port | Yes | Local port (`127.0.0.1`) of this connection's MCP server. Must be different for each connection. |
| Language | No | SAP logon language. Does not change the extension's language, which always follows VS Code. |
| Allow untrusted certificates | No (`false`) | Accepts self-signed TLS certificates for this system. |
| SAP system ID (SID) | No | SID as it appears in your SAP Logon. Needed to open classic SAP GUI. |
| Allows development | No (`true`) | If unchecked, the connection is **query-only**: the AI can only search, read, open in Display mode, query data and list dumps; it cannot write or activate. Intended for production systems. |
| Silent startup | No (`false`) | Starts this connection's MCP server when VS Code opens, without asking. Several connections can be checked to have several servers running at once. |

**Debugger**

| Option | Values | What it does |
|---|---|---|
| `idea.depuracion.atajos` | Object action → key | Shortcuts of the debugging window. Defaults: `F5` step into, `F6` step over, `F7` return, `F8` continue, `F9` breakpoint, `Shift+F9` other breakpoints, `Shift+F4` watchpoint, `F2` add variable, `F12` jump to statement, `F10` layout. They can also be changed from the panel's *Shortcuts* button. |

**Extended operations and SAP GUI**

| Option | Values | What it does |
|---|---|---|
| `idea.endpointAmpliacionADT` | Service path (empty by default), e.g. `/sap/serviciosazure/` | Enables the extended features (data queries, REPT text elements, dictionary, GUI Status/Title, Dynpros). If left empty, those actions open the object in SAP GUI. |
| `idea.sapGui.sapshcutPath` | Path to `sapshcut.exe` (empty by default) | Only if SAP GUI is not in a standard location or on the PATH. |
| `idea.navigation.gui` | `sapGui` (default), `webGui` | When navigating to the definition of an object the extension doesn't edit, chooses between classic SAP GUI (`sapshcut.exe`, needs the *SAP system ID*) or the Web GUI in the browser. |

</details>

<details>
<summary><strong>🔌 Active connection and MCP servers</strong></summary>

IDEA distinguishes two concepts:

- **Active connection**: the SAP system *this window* of VS Code works against (search, editing, activation). It is shown and changed from the status bar. When VS Code opens, the one set in `mcpInicial` is activated. The same connection cannot be active in two windows at once. When switching connections, IDEA first closes everything open from the previous one (asking for confirmation if there are unsaved changes).
- **MCP servers**: one per connection, each on its own port. Several can run at once, so the AI can work in DEV and query QAS in parallel.

**Connecting your MCP client:**
- **Clients built into VS Code**: IDEA automatically publishes the active connection's server (`IDEA – <connection>`); nothing to configure.
- **External clients** (Claude Code, Cursor…): add an `http` server pointing to `http://127.0.0.1:<port>/mcp`, with the connection's *MCP port*. One per connection you want to use.

**MCP tools available to the AI**

| Tool | What it does | Query only |
|---|---|:---:|
| `abap_connection_info` | Tells which SAP system the server is connected to. | ✅ |
| `abap_search_object` | Searches objects by name. | ✅ |
| `abap_read_object_source` | Reads an object's source code. | ✅ |
| `abap_open_object` | Opens an object in VS Code under the extension's control. | ✅ |
| `abap_execute_query` | Runs a read-only `SELECT` query on the database *(extended feature)*. | ✅ |
| `abap_list_dumps_24h` | Lists runtime dumps from the last 24 hours (standard ADT feed). | ✅ |
| `abap_list_dumps` | Lists runtime dumps from any date (equivalent to ST22), in compact form *(extended feature)*. | ✅ |
| `abap_get_dump_detalle` | Returns the detail of a dump: ST22 summary and call stack; variables or the full dump only on request *(extended feature)*. | ✅ |
| `abap_write_object_source` | Writes an object's source (with diff and confirmation). | — |
| `abap_activate_object` | Activates an object (with confirmation). | — |
| `abap_llamar_herramienta_desarrollo` | Operations of the extended component: locks, transport requests, text elements… (with confirmation) *(extended feature)*. | — |

The *Query only* column shows the tools available on connections with **Allows development** unchecked.

</details>

<details>
<summary><strong>🖥️ The «IDEA» side panel in detail</strong></summary>

The IDEA icon in the activity bar opens four sections.

**1. Code search**: finds and replaces text in the ABAP file open in the editor. *Search type*: partial or whole word. *Scope*: current block or whole file. Results show the line number (click to jump) and can be filtered. *Replace* offers a preview before confirming. Keeps a recent history.

**2. SAP object search**: searches objects in the SAP system of the active connection and opens them in VS Code (requires the MCP server running and `idea.mcpServer.tempFilesPath` configured). The name accepts `*` as a wildcard.
- **Program / Report**, **Class** and **Function module**: opened as an editable temporary file, in Display mode; deleted when the tab is closed.
- **Classes**: buttons to open their local includes: `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` and `<TEST>` (ABAP Unit test classes).
- **Function groups**: shows their tree (function modules, includes and other parts) to open each piece separately.
- **Data element**, **Structure / Table**, **Domain**, **Table type**: opened in the dictionary editor *(extended feature)*.
- **REPT, CUA and DYNP buttons** (depending on the object type): open the text element, GUI Status/Title and Dynpro editors *(extended features)*.
- **Message class**: opens in the message class editor (through standard ADT, without the extended component).
- **New button**: creates a program, a class, a message class or a dictionary object (data element, domain, structure/table, table type) given a name and package. Without the extended component only message classes can be created.
- If the search returns a single result, it opens directly. Keeps **recent** and **history** searches.
- Objects the extension can't edit are opened in classic SAP GUI (or Web GUI, depending on `idea.navigation.gui`).

**3. Session change history**: keeps copies of the object every time a real change is saved or activated, and also when it detects that the object was changed directly in SAP. It only covers the current session: it is cleared when the tab is closed and not kept across restarts.
- *Load versions*: table with the most recent at the top, the time of the change, whether it was activated, its origin (*Local* or *Changed in SAP*) and the number of changes compared with the last activation and the previous version.
- Check **two** versions and *Show changes*: opens VS Code's diff viewer.
- *Show total changes*: compares the initial version with the current one.
- Check **one** and *Restore version*: puts its content in the editor (does not save it automatically).

**4. Settings**: quick access, without leaving the panel, to:
- SAP connections: table with *Name*, *Silent start* (its MCP server starts when VS Code opens), *AutoConnect* (the one that is active when VS Code opens) and *Development* (whether it allows development); the other details (URL, client, user, MCP port) appear when hovering over the row. *Manage connections…* button.
- Pretty Printer: engine, scope, indentation, double spaces, upper/lower case and `METHOD` indentation.
- MCP server: initial connection, write confirmation and temporary files folder.
- Navigation and SAP GUI: where to open non-editable objects, path to `sapshcut.exe` and the ADT extension service.

</details>

<details>
<summary><strong>🧩 Extended features in detail</strong></summary>

**Data queries.** Lets the AI investigate the data in your SAP system with read-only `SELECT` queries (no `INSERT`/`UPDATE`/`DELETE` or DDL). Without it, the AI sees the code but not the data, and loses much of its analytical ability.

**Text element editor (REPT).** From the *REPT* button in «SAP object search», on a program, class or interface:
- Opens in Display mode (blue background).
- *Edit* locks the object in SAP (amber background); changing any cell shows 🔴 on the tab.
- *Save and activate* uploads the texts to SAP (asking for a transport request if needed) and keeps the lock so you can keep editing.
- Returning to Display mode or closing the tab releases the lock.
- *Copy* puts the whole text table on the clipboard.

**Dictionary editor.** Data elements, structures / tables, domains and table types: header, technical options and list of fields or values. Opens in Display mode; *Edit* locks the object and lets you change and activate it with the same transport request handling as the rest. The field table header stays fixed when scrolling; columns can be sorted and filtered. From the cells you can navigate to other data elements and domains.

**GUI Status / Title (CUA).** Create, delete and edit titles, functions, statuses and the standard toolbar.

**Dynpros (SE51).** Visual editor for fields and containers (frames, subscreens, tabstrips, table controls): add an element by placing it with a click, overlap detection and validation on save.

All of them follow the same lock, transport request and activation discipline as the rest of the objects.

</details>

---

## License

The extension is free to use under the MIT license.

If you are interested in the extended features, which require the ABAP component “ADT Ampliado” (Extended ADT), contact Marcos Almeida Santolaria for terms and pricing at [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

[Español](README.md) · **English** · [Deutsch](README.de.md) · [Français](README.fr.md)
