# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Environnement de Développement Intégré pour ABAP

[Español](README.md) · [English](README.en.md) · [Deutsch](README.de.md) · **Français**

> 💡 Pour lire ce README dans une autre langue dans VS Code, exécutez **IDEA : Afficher le README** (`Ctrl+Shift+P`) : il s'ouvre automatiquement dans la langue de votre éditeur.

---

## Le développement ABAP moderne, sans quitter VS Code

**IDEA** transforme Visual Studio Code en un environnement de développement ABAP complet : connecté en temps réel à votre système SAP et prêt à travailler main dans la main avec l'assistant IA que vous utilisez déjà (Claude Code, GitHub Copilot, Cursor…).

Fini le copier-coller de code entre SAP GUI et un chat IA. Fini de perdre de vue quel objet est verrouillé, qui l'a modifié ou s'il attend encore d'être activé. Avec IDEA, tout se passe dans l'éditeur lui-même, avec la même rigueur de verrous, d'ordres de transport et d'activation que vous connaissez déjà dans SAP — mais avec la rapidité de VS Code et la puissance de l'IA.

**En une phrase :** cherchez un objet → ouvrez-le → demandez à votre IA de le modifier (ou modifiez-le vous-même) → activez-le. Le tout sans quitter VS Code, le tout sous contrôle.

**En une autre phrase 😉 :** Un IDoc a échoué ? → demandez à votre IA de l'analyser et de vous indiquer la solution → corrigez-le. Le tout sans quitter VS Code, le tout sous contrôle.

---

## Pourquoi votre équipe va l'adorer

| | |
|---|---|
| ⚡ **Vraie rapidité** | Recherche instantanée de programmes, classes, interfaces et objets du dictionnaire, avec historique des recherches. Sans transactions ni menus imbriqués. |
| 🤖 **IA avec accès direct à SAP** | Serveur MCP intégré : votre assistant IA lit, écrit et active du code ABAP directement dans SAP, en montrant toujours un diff de confirmation avant de toucher à quoi que ce soit. |
| 🌐 **Multi-système** | Plusieurs serveurs MCP en même temps, un par système : votre IA peut écrire en DEV tout en consultant des données en PRD via une connexion en lecture seule. |
| 🔒 **Zéro surprise** | Mode Affichage par défaut, verrou explicite pour modifier, ordres de transport et activation gérés exactement comme dans SAP standard. |
| 🕘 **Historique à la volée** | Chaque enregistrement et chaque activation sont consignés dans la session : comparez des versions ou récupérez-en une ancienne sans quitter l'éditeur. |
| 🎨 **Un formatage qui respecte vos diffs** | Formateur propre qui ne touche que les lignes modifiées par le développeur — fini le reformatage accidentel de fichiers entiers. |
| 🖥️ **Éditeur de source comme dans SAP GUI** | Éditeur intégré directement dans l'onglet : mode affichage ou édition, classes par blocs ou complètes, descriptions modifiables, navigation directe vers REPT/CUA/Dynpros et les includes locaux, et contrôle total des temps d'attente face à SAP. |
| 🧩 **Au-delà de l'ADT standard** *(fonction étendue)* | Édition des éléments de texte (REPT), du dictionnaire de données, des écrans GUI Status/Title et des Dynpros — tout ce que l'ADT de SAP ne permet pas de modifier hors de SAP GUI. |

---

## Comment ça marche

1. **Configurez vos connexions SAP** avec `IDEA : Gérer les connexions SAP` — Définissez toutes les connexions aux systèmes SAP avec lesquels vous voulez travailler, afin de pouvoir indiquer depuis le chat de l'IA sur quel environnement elle doit travailler ; au démarrage de VS Code, les serveurs MCP de chaque système seront connectés (cela ne fait rien dans les systèmes, le serveur MCP se contente d'écouter). Configurez l'une des connexions pour qu'elle démarre automatiquement avec VS Code.
2. **Cherchez l'objet** dont vous avez besoin depuis le panneau latéral «IDEA».
3. **Demandez à votre IA** de le modifier, ou modifiez-le vous-même avec autocomplétion, formatage et navigation vers les définitions.
4. **Activez-le avec un raccourci** (`Ctrl+F3`). IDEA gère le verrou, l'ordre de transport et l'activation pour vous.

Inutile d'ouvrir l'objet manuellement avant de demander quelque chose à votre IA : avec la connexion MCP active, elle peut elle-même le chercher, le lire et le modifier directement dans SAP.

> Pour que votre IA exploite tout le potentiel d'IDEA, demandez-lui explicitement d'utiliser les outils MCP d'IDEA pour lire et écrire dans SAP, au lieu de modifier l'objet à la main dans l'éditeur.

---

## Mode Affichage / Mode Édition

Les objets ouverts depuis «Recherche d'objet SAP» démarrent en **Mode Affichage** (fond bleuté) : ils ne verrouillent pas l'objet dans SAP et empêchent de saisir par erreur.

1. `Ctrl+F1` passe en **Mode Édition** : verrouille l'objet dans SAP.
2. Vous modifiez et enregistrez avec `Ctrl+S` ; chaque enregistrement en Édition envoie aussi le code à SAP.
3. `Ctrl+F3` formate et active l'objet.
4. `Ctrl+F1` à nouveau, ou `Ctrl+Shift+U` pour abandonner les modifications, revient en Affichage et libère le verrou. Fermer l'onglet libère aussi le verrou.

Un badge 🔴 sur l'onglet signale des modifications enregistrées en attente d'activation.

---

## Éditeur de source WebView : comme dans SAP GUI, mais dans VS Code

Un éditeur de code source intégré directement dans l'onglet, avec le même moteur que VS Code lui-même (Monaco), pensé pour travailler face à SAP exactement comme dans SE24/SE38, avec beaucoup d'opérations à portée de main.

**Modifiez les classes comme dans SAP GUI**
- **Source complet ou par blocs** : basculez entre la classe entière ou seulement la méthode qui vous intéresse, avec sa *déclaration* en haut et son *implémentation* en bas, toutes deux modifiables et partageant le même défilement — exactement comme dans SE24.
- **Descriptions** : modifiez dans un tableau dédié les textes courts des attributs, types, méthodes, événements et paramètres de la classe ou de l'interface, sans quitter l'éditeur ; ils sont enregistrés avec le reste du source.
- **Bouton Naviguer** : accédez directement aux éléments de texte (REPT), au GUI Status/Title (CUA) et aux écrans (Dynpros) de l'objet, ainsi qu'aux includes locaux de la classe — définitions (`CCDEF`), implémentations (`CCIMP`), macros (`CCMAC`) et classes de test ABAP Unit (`CCAU`) —, chacun dans son propre onglet.

**Contrôle total des temps d'attente face à SAP**
- Pendant qu'il verrouille, enregistre, active ou formate face à SAP, l'éditeur se verrouille entièrement (une couche indique ce qui se passe) pour empêcher de continuer à taper ou de lancer une autre action tant que SAP n'a pas répondu.
- Si SAP met trop de temps, l'éditeur se déverrouille de lui-même et vous prévient, au lieu de vous laisser attendre sans savoir ce qui se passe.
- Le statut de l'objet — *Non modifié*, *Modifié, non enregistré* ou *Modifié, non activé* — est toujours visible directement dans la barre de l'éditeur.

**Toute l'opérative, à un clic depuis sa propre barre d'outils**
- Boutons pour Modifier/Afficher, Enregistrer, Activer, Rechercher et remplacer, Historique des versions (avec comparateur de différences intégré), Modifications de la session, Descriptions, Naviguer et Messages — sans passer par la palette de commandes.
- **Raccourcis clavier configurables** par action, avec validation des conflits et communs à toutes les fenêtres de VS Code.
- Extraits de code (snippets), autocomplétion face à SAP et suggestions de code par IA intégrées directement dans l'éditeur.

---

## Démarrage rapide

1. Installez l'extension et rechargez VS Code.
2. `Ctrl+Shift+P` → **IDEA : Gérer les connexions SAP** → ajoutez vos systèmes ou environnements SAP.
3. Définissez dans la configuration un dossier local pour les fichiers temporaires (`idea.mcpServer.tempFilesPath`).
4. Rechargez la fenêtre (**Développeur : Recharger la fenêtre**).

C'est prêt : l'extension recherche, modifie et active déjà sur SAP, et votre assistant IA peut désormais analyser, investiguer, modifier… tout ce qui peut vous aider.

---

## Serveur MCP : votre IA, qui travaille directement dans SAP

Le serveur MCP permet à un assistant IA de lire et de modifier du code ABAP directement dans le système SAP connecté. Il ne travaille pas sur des copies locales : tout passe par SAP, avec les mêmes garanties de verrouillage et d'activation que le reste de l'extension.

**Actions de développement disponibles pour l'IA :**
- Savoir à quel système SAP elle est connectée.
- Chercher des objets par nom.
- Lire le code d'un objet.
- Ouvrir un objet dans VS Code sous le contrôle de l'extension.
- Écrire le code d'un objet (avec confirmation).
- Activer un objet.

**Connexion depuis votre client MCP :** ajoutez un serveur de type `http` pointant vers `http://127.0.0.1:<port>` (port configurable, par exemple `4856`).

---

## 🔐 Sécurité et contrôle

- IDEA ne stocke aucun code source dans le cloud : tout est lu et écrit directement sur votre système SAP. Le source ouvert est conservé dans des fichiers temporaires sur votre ordinateur, supprimés dès que vous fermez la fenêtre d'édition.
- Les mots de passe sont stockés chiffrés dans le stockage sécurisé de VS Code, jamais en clair ni dans la configuration.
- Avec `idea.mcpServer.confirmWrites` (actif par défaut), toute écriture ou activation proposée par l'IA demande une confirmation préalable. Elle est en outre affichée sous forme de diff avant d'être appliquée.
- Le serveur MCP n'écoute que sur `127.0.0.1` (votre propre machine).
- Les requêtes de données sont uniquement des requêtes, SELECT. Elles ne modifient jamais les données des tables.
- Si vous réglez "Développement autorisé" de la connexion sur false, vous avez la garantie que l'IA ne modifiera jamais rien dans le système, ni objets ni données.

---

## Fonctions étendues (sous licence)

Avec un petit composant installé dans votre système SAP (configuré dans `idea.endpointAmpliacionADT`), IDEA débloque dans VS Code ce que même l'ADT standard de SAP n'offre pas :

- **Requêtes de données** L'IA peut consulter les tables SAP (lecture seule). C'est ce qui permet à l'IA de donner toute sa puissance.
- **Créer la structure vide d'une classe, d'un programme ou d'une interface**
- **Éléments de texte (REPT)** des programmes, classes et interfaces — édition directe, sans SE38/SE24.
- **Dictionnaire de données** : éléments de données, structures, domaines et types de table, avec navigation croisée entre eux.
- **GUI Status / Title** des programmes : création, suppression et édition visuelle des fonctions, status et barre d'outils.
- **Dynpros (SE51)** : éditeur visuel des champs et conteneurs, avec validation à l'enregistrement.

Sans ce composant, ces actions restent disponibles : elles ouvrent simplement l'objet dans SAP GUI classique au lieu de VS Code.

📩 **Vous voulez la licence complète pour votre équipe ou votre cabinet de conseil ?** Écrivez à [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Référence technique

<details>
<summary><strong>📋 Commandes et raccourcis clavier</strong></summary>

**Édition, enregistrement et activation**

| Commande | Raccourci | Description |
|---|---|---|
| `IDEA : Basculer Mode Édition / Affichage` | `Ctrl+F1` | Bascule entre le Mode Édition (verrouille l'objet dans SAP) et le Mode Affichage (le libère). |
| `IDEA : Enregistrer l'objet ABAP` | `Ctrl+S` | Enregistre en local et dans SAP. Si l'objet est transportable, demande l'ordre de transport **avant** d'enregistrer quoi que ce soit. |
| `IDEA : Activer l'objet ABAP` | `Ctrl+F3` | Formate l'objet et l'active dans SAP. |
| `IDEA : Annuler les modifications et revenir à l'affichage` | `Ctrl+Shift+U` | Abandonne les modifications non enregistrées et revient en Mode Affichage. |
| `IDEA : Afficher les blocs modifiés depuis la dernière activation` | — | (Classes et interfaces) Liste les méthodes et sections modifiées depuis la dernière activation et saute à celle choisie. Aussi via le bouton «N modifications» de la barre d'état. |
| `IDEA : Formater le document` | `Shift+F1` | Formate l'objet avec le moteur configuré. |

**Écriture de code**

| Commande | Raccourci | Description |
|---|---|---|
| `IDEA : Commenter/décommenter la ligne (* en colonne 1)` | `Ctrl+<` | Commente ou décommente les lignes sélectionnées avec `*` en colonne 1, à la manière de SAP. |
| `IDEA : Fusionner l'instruction en le moins de lignes possible` | `Ctrl+Shift+J` | Fusionne plusieurs lignes en une seule instruction. |
| `IDEA : Diviser l'instruction en lignes` | `Ctrl+Shift+K` | Divise une longue instruction (`SELECT`, `CALL METHOD`, etc.) en plusieurs lignes. |
| `IDEA : Diviser l'instruction déclarative en lignes` | `Ctrl+Shift+D` | Sépare les déclarations chaînées `DATA:` / `TYPES:` en instructions individuelles. |

**Navigation et recherche**

| Commande | Raccourci | Description |
|---|---|---|
| `IDEA : Rechercher et naviguer vers un bloc de code` | `Ctrl+Alt+M` / `Ctrl+Shift+Z` | Liste rapide pour sauter à un METHOD / FORM / MODULE / événement du fichier. |
| `IDEA : Aller au début du bloc` | `Ctrl+Shift+↑` / `Ctrl+Alt+PgPréc` | Saute au début du bloc où se trouve le curseur. |
| `IDEA : Aller à la fin du bloc` | `Ctrl+Shift+↓` / `Ctrl+Alt+PgSuiv` | Saute à la fin du bloc où se trouve le curseur. |
| Atteindre la définition | `F2` / `F12` / `Ctrl+Click` | Navigue vers la définition de l'objet sous le curseur. Dans les fichiers ABAP, `F2` remplace «Renommer» (comme dans SAP GUI). |
| `IDEA : Rechercher et remplacer` | `Ctrl+Shift+F` | Ouvre le panneau «Recherche dans le code» avec le focus sur le champ de recherche. Fonctionne toujours, pas seulement dans l'éditeur ABAP. |

**Connexions, serveur MCP et SAP GUI**

| Commande | Raccourci | Description |
|---|---|---|
| `IDEA : Gérer les connexions SAP` | — | Ajoute, modifie ou supprime les systèmes SAP disponibles. |
| `IDEA : Changer de connexion active` | — | Choisit le système SAP sur lequel travaille cette fenêtre. Aussi en cliquant sur la connexion dans la barre d'état. |
| `IDEA : Fermer toutes les connexions` | — | Ferme la connexion active et arrête les serveurs MCP de cette fenêtre. |
| `IDEA : Démarrer le serveur MCP` | `Ctrl+Alt+S` | Démarre le serveur MCP d'une connexion. |
| `IDEA : Arrêter le serveur MCP` | — | Arrête un serveur MCP en cours d'exécution. |
| `IDEA : Ouvrir SAP GUI` | — | Ouvre une fenêtre SAP GUI classique sur la connexion choisie. |
| `IDEA : Afficher le README (langue de VS Code)` | — | Ouvre ce README dans la langue de l'éditeur. |

Sauf `Ctrl+Shift+F`, les raccourcis s'appliquent lorsque l'éditeur ABAP a le focus. Dans les fichiers non ABAP, `Ctrl+F3` conserve sa fonction d'origine dans VS Code («Rechercher la sélection suivante»). En plus : **Formater le document** (`Shift+Alt+F`), autocomplétion (`Ctrl+Space`) et repli du code.

</details>

<details>
<summary><strong>⚙️ Configuration complète</strong></summary>

Paramètres sous `idea.*` (Fichier → Préférences → Paramètres, ou depuis le panneau «Configuration» d'IDEA).

**Formatage (Pretty Printer)**

| Option | Valeurs | Rôle |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (par défaut), `sapConfig` | Moteur utilisé par «Formater le document» et avant l'activation. `extension` : le formateur intégré. `sapConfig` : le Pretty Printer configuré dans SAP (uniquement les objets ouverts depuis «Recherche d'objet SAP»). |
| `idea.prettyprinter.indentation` | `true` (par défaut), `false` | Active ou non l'indentation automatique. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (par défaut), `false` | Supprime ou non les doubles espaces. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (par défaut), `lowerKeywords`, `upperAll`, `lowerAll` | Majuscules/minuscules : mots-clés seulement, ou tout le code. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (par défaut), `modoSe24`, `estandar` | Indentation de `METHOD` / `ENDMETHOD` (classes uniquement). `auto` : conserve les espaces existants. `modoSe24` : colonne 0. `estandar` : un niveau (2 espaces). |
| `idea.prettyprinter.formatScope` | `fullFile` (par défaut), `currentMethodOnly` | Lors du formatage par raccourci (classes uniquement) : tout le fichier ou seulement la méthode où se trouve le curseur. |

**Autocomplétion**

| Option | Valeurs | Rôle |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (par défaut), `false` | Lors de l'insertion d'un appel de méthode ou de fonction avec `Ctrl+Space`, inclut le commentaire de chaque paramètre. Avec `false`, seuls les paramètres sont insérés. |

**Connexions et serveur MCP**

| Option | Valeurs | Rôle |
|---|---|---|
| `idea.mcpServer.connections` | Liste des systèmes SAP | Systèmes disponibles. Se modifie avec «IDEA : Gérer les connexions SAP». Le mot de passe n'est **pas** stocké ici : il est demandé puis stocké chiffré dans le stockage sécurisé de VS Code. Champs de chaque connexion dans le tableau suivant. |
| `idea.mcpServer.config` → `mcpInicial` | Nom d'une connexion (vide par défaut) | Connexion **active** à l'ouverture de VS Code. Vide = aucune. |
| `idea.mcpServer.confirmWrites` | `true` (par défaut), `false` | Demande une confirmation (avec un diff) avant que l'IA n'écrive ou n'active du code dans SAP. |
| `idea.mcpServer.tempFilesPath` | Chemin de dossier (vide par défaut) | Dossier où sont créés les fichiers `.abap` temporaires de «Recherche d'objet SAP». **Obligatoire** pour chercher et ouvrir des objets. Les fichiers sont supprimés à la fermeture de leur onglet ou de VS Code. |

**Champs de chaque connexion**

| Champ | Obligatoire | Rôle |
|---|---|---|
| Nom | Oui | Identifiant du système (ex. `DEV`, `QAS`). C'est le nom sous lequel l'IA et la barre d'état y font référence. |
| URL | Oui | URL de base du système SAP (ex. `https://monserveur.mondomaine.com:44300`). |
| Client (mandant) | Oui | Mandant SAP (ex. `100`). |
| Utilisateur | Oui | Utilisateur SAP. |
| Port MCP | Oui | Port local (`127.0.0.1`) du serveur MCP de cette connexion. Doit être différent pour chaque connexion. |
| Langue | Non | Langue de connexion SAP. Ne change pas la langue de l'extension, qui suit toujours celle de VS Code. |
| Autoriser les certificats non approuvés | Non (`false`) | Accepte les certificats TLS auto-signés pour ce système. |
| ID du système SAP (SID) | Non | SID tel qu'il apparaît dans votre SAP Logon. Nécessaire pour ouvrir SAP GUI classique. |
| Développement autorisé | Non (`true`) | Si décoché, la connexion est en **consultation seule** : l'IA peut seulement chercher, lire, ouvrir en Affichage, consulter des données et lister les dumps ; elle ne peut ni écrire ni activer. Prévu pour les systèmes de production. |
| Démarrage silencieux | Non (`false`) | Démarre le serveur MCP de cette connexion à l'ouverture de VS Code, sans rien demander. Plusieurs connexions peuvent être cochées pour avoir plusieurs serveurs en même temps. |

**Fonctions étendues et SAP GUI**

| Option | Valeurs | Rôle |
|---|---|---|
| `idea.endpointAmpliacionADT` | Chemin du service (vide par défaut), p. ex. `/sap/serviciosazure/` | Active les fonctions étendues (requêtes de données, éléments de texte REPT, dictionnaire, GUI Status/Title, Dynpros). S'il reste vide, ces actions ouvrent l'objet dans SAP GUI. |
| `idea.sapGui.sapshcutPath` | Chemin vers `sapshcut.exe` (vide par défaut) | Uniquement si SAP GUI n'est pas à un emplacement standard ni dans le PATH. |
| `idea.navigation.gui` | `sapGui` (par défaut), `webGui` | Lors de la navigation vers la définition d'un objet que l'extension ne modifie pas : SAP GUI classique (`sapshcut.exe`, nécessite l'*ID du système SAP*) ou Web GUI dans le navigateur. |

</details>

<details>
<summary><strong>🔌 Connexion active et serveurs MCP</strong></summary>

IDEA distingue deux notions :

- **Connexion active** : le système SAP sur lequel travaille *cette fenêtre* de VS Code (recherche, édition, activation). Elle s'affiche et se change depuis la barre d'état. À l'ouverture de VS Code, celle indiquée dans `mcpInicial` est activée. Une même connexion ne peut pas être active dans deux fenêtres à la fois. En changeant de connexion, IDEA ferme d'abord tout ce qui est ouvert de la précédente (en demandant confirmation s'il y a des modifications non enregistrées).
- **Serveurs MCP** : un par connexion, chacun sur son propre port. Plusieurs peuvent tourner en même temps, de sorte que l'IA peut travailler en DEV et consulter QAS en parallèle.

**Connecter votre client MCP :**
- **Clients intégrés à VS Code** : IDEA publie automatiquement le serveur de la connexion active (`IDEA – <connexion>`) ; rien à configurer.
- **Clients externes** (Claude Code, Cursor…) : ajoutez un serveur de type `http` pointant vers `http://127.0.0.1:<port>/mcp`, avec le *port MCP* de la connexion. Un par connexion que vous voulez utiliser.

**Outils MCP disponibles pour l'IA**

| Outil | Rôle | Consultation seule |
|---|---|:---:|
| `abap_connection_info` | Indique à quel système SAP le serveur est connecté. | ✅ |
| `abap_search_object` | Cherche des objets par nom. | ✅ |
| `abap_read_object_source` | Lit le code source d'un objet. | ✅ |
| `abap_open_object` | Ouvre un objet dans VS Code sous le contrôle de l'extension. | ✅ |
| `abap_execute_query` | Exécute une requête `SELECT` en lecture seule sur la base de données *(fonction étendue)*. | ✅ |
| `abap_list_dumps` | Liste les dumps d'exécution (équivalent de ST22). | ✅ |
| `abap_write_object_source` | Écrit le source d'un objet (avec diff et confirmation). | — |
| `abap_activate_object` | Active un objet (avec confirmation). | — |
| `abap_llamar_herramienta_desarrollo` | Opérations du composant étendu : verrous, ordres de transport, éléments de texte… (avec confirmation) *(fonction étendue)*. | — |

La colonne *Consultation seule* indique les outils disponibles sur les connexions dont **Développement autorisé** est décoché.

</details>

<details>
<summary><strong>🖥️ Le panneau latéral «IDEA» en détail</strong></summary>

L'icône d'IDEA dans la barre d'activité ouvre quatre sections.

**1. Recherche dans le code** : recherche et remplace du texte dans le fichier ABAP ouvert dans l'éditeur. *Type de recherche* : partielle ou mot entier. *Portée* : bloc courant ou fichier entier. Les résultats indiquent le numéro de ligne (clic pour y aller) et peuvent être filtrés. *Remplacer* propose un aperçu avant de confirmer. Conserve un historique récent.

**2. Recherche d'objet SAP** : cherche des objets dans le système SAP de la connexion active et les ouvre dans VS Code (nécessite le serveur MCP démarré et `idea.mcpServer.tempFilesPath` configuré). Le nom accepte `*` comme joker.
- **Programme / Report**, **Classe** et **Module fonction** : ouverts comme fichier temporaire modifiable, en Mode Affichage ; supprimés à la fermeture de l'onglet.
- **Classes** : boutons pour ouvrir leurs includes locaux : `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` et `<TEST>` (classes de test ABAP Unit).
- **Groupes de fonctions** : affiche leur arborescence (modules fonction, includes et autres parties) pour ouvrir chaque élément séparément.
- **Élément de données**, **Structure / Table**, **Domaine**, **Type de table** : ouverts dans l'éditeur de dictionnaire *(fonction étendue)*.
- **Boutons REPT, CUA et DYNP** (selon le type d'objet) : ouvrent les éditeurs d'éléments de texte, de GUI Status/Title et de Dynpros *(fonctions étendues)*.
- **Bouton Nouveau** : crée un programme, une classe ou un objet du dictionnaire (élément de données, domaine, structure/table, type de table) en indiquant le nom et le paquet.
- Si la recherche renvoie un seul résultat, il s'ouvre directement. Conserve les recherches **récentes** et l'**historique**.
- Les objets que l'extension ne sait pas modifier s'ouvrent dans SAP GUI classique (ou Web GUI, selon `idea.navigation.gui`).

**3. Historique des modifications de la session** : conserve des copies de l'objet à chaque enregistrement ou activation d'une vraie modification, et aussi lorsqu'il détecte que l'objet a été modifié directement dans SAP. Uniquement pour la session en cours : il est effacé à la fermeture de l'onglet et n'est pas conservé entre les redémarrages.
- *Charger les versions* : tableau avec la plus récente en haut, l'heure de la modification, si elle a été activée, son origine (*Local* ou *Modifié dans SAP*) et le nombre de modifications par rapport à la dernière activation et à la version précédente.
- Cochez **deux** versions et *Voir les modifications* : ouvre le comparateur de VS Code.
- *Voir les modifications totales* : compare la version initiale à l'actuelle.
- Cochez-en **une** et *Récupérer la version* : place son contenu dans l'éditeur (sans l'enregistrer automatiquement).

**4. Configuration** : accès rapide, sans quitter le panneau, à :
- Connexions SAP : tableau avec *Nom*, *Démarrage silen.* (son serveur MCP démarre à l'ouverture de VS Code), *AutoConnexion* (celle qui est active à l'ouverture de VS Code) et *Développement* (développement autorisé ou non) ; les autres informations (URL, mandant, utilisateur, port MCP) apparaissent au survol de la ligne. Bouton *Gérer les connexions…*.
- Pretty Printer : moteur, portée, indentation, doubles espaces, majuscules/minuscules et indentation de `METHOD`.
- Serveur MCP : connexion initiale, confirmation des écritures et dossier des fichiers temporaires.
- Navigation et SAP GUI : où ouvrir les objets non modifiables, chemin de `sapshcut.exe` et service d'extension ADT.

</details>

<details>
<summary><strong>🧩 Fonctions étendues en détail</strong></summary>

**Requêtes de données.** Permet à l'IA d'explorer les données de votre système SAP avec des requêtes `SELECT` en lecture seule (sans `INSERT`/`UPDATE`/`DELETE` ni DDL). Sans elles, l'IA voit le code mais pas les données, et perd une bonne partie de sa capacité d'analyse.

**Éditeur d'éléments de texte (REPT).** Depuis le bouton *REPT* de «Recherche d'objet SAP», sur un programme, une classe ou une interface :
- S'ouvre en Mode Affichage (fond bleu).
- *Modifier* verrouille l'objet dans SAP (fond ambre) ; toute modification de cellule fait apparaître 🔴 sur l'onglet.
- *Enregistrer et activer* envoie les textes à SAP (en demandant un ordre de transport si nécessaire) et conserve le verrou pour continuer à modifier.
- Revenir en Affichage ou fermer l'onglet libère le verrou.
- *Copier* place tout le tableau des textes dans le presse-papiers.

**Éditeur de dictionnaire.** Éléments de données, structures / tables, domaines et types de table : en-tête, options techniques et liste des champs ou valeurs. S'ouvre en Affichage ; *Modifier* verrouille l'objet et permet de le modifier et de l'activer avec la même gestion des ordres de transport que le reste. L'en-tête du tableau des champs reste fixe au défilement ; colonnes triables et filtrables. Depuis les cellules, on navigue vers d'autres éléments de données et domaines.

**GUI Status / Title (CUA).** Création, suppression et édition des titres, fonctions, status et de la barre d'outils standard.

**Dynpros (SE51).** Éditeur visuel des champs et conteneurs (cadres, subscreens, tabstrips, table controls) : ajout en plaçant l'élément d'un clic, détection des chevauchements et validation à l'enregistrement.

Tous suivent la même rigueur de verrou, d'ordre de transport et d'activation que les autres objets.

</details>

---

## Licence

L'extension est d'utilisation libre sous licence MIT.

Si les fonctionnalités étendues vous intéressent, qui nécessitent le composant ABAP « ADT Ampliado » (ADT étendu), contactez Marcos Almeida Santolaria pour les conditions et les tarifs à [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

[Español](README.md) · [English](README.en.md) · [Deutsch](README.de.md) · **Français**
