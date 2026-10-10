# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Entorno de Desarrollo Integrado de ABAP

**Español** · [English](README.en.md) · [Deutsch](README.de.md) · [Français](README.fr.md)

> 💡 Para leer este README en otro idioma dentro de VS Code, ejecuta **IDEA: Mostrar README** (`Ctrl+Shift+P`): se abre automáticamente en el idioma de tu editor.

---

## Desarrollo ABAP moderno, sin salir de VS Code

**IDEA** convierte Visual Studio Code en un entorno de desarrollo ABAP completo: conectado en tiempo real a tu sistema SAP y preparado para trabajar codo con codo con el asistente de IA que ya uses (Claude Code, GitHub Copilot, Cursor…).

Se acabó copiar y pegar código entre SAP GUI y un chat de IA. Se acabó perder de vista qué objeto está bloqueado, quién lo tocó o si sigue pendiente de activar. Con IDEA todo ocurre dentro del propio editor, con la misma disciplina de bloqueos, órdenes de transporte y activación que ya conoces de SAP — pero con la velocidad de VS Code y la potencia de la IA.

**En una frase:** busca un objeto → ábrelo → pide a tu IA que lo modifique (o edítalo tú) → actívalo. Todo sin salir de VS Code, todo bajo control.

**En otra frase 😉:** ¿Te falló un iDoc? → pide a tu IA que lo analice y te indique la solución → soluciónalo. Todo sin salir de VS Code, todo bajo control.

---

## ¿Por qué le va a encantar a tu equipo?

| | |
|---|---|
| ⚡ **Rapidez real** | Búsqueda instantánea de programas, clases, interfaces y objetos de diccionario, con historial de búsquedas. Sin transacciones ni menús anidados. |
| 🤖 **IA con acceso directo a SAP** | Servidor MCP integrado: tu asistente de IA lee, escribe y activa código ABAP directamente en SAP, mostrando siempre un diff de confirmación antes de tocar nada. |
| 🌐 **Multi-sistema** | Varios servidores MCP en marcha a la vez, uno por sistema: tu IA puede escribir en DEV mientras consulta datos en PRD con una conexión de solo lectura. |
| 🔒 **Cero sorpresas** | Modo Visualización por defecto, bloqueo explícito para editar, órdenes de transporte y activación gestionadas exactamente igual que en SAP estándar. |
| 🕘 **Historial al vuelo** | Cada guardado y cada activación quedan registrados en la sesión: compara versiones o recupera una anterior sin salir del editor. |
| 🎨 **Formateo que respeta tus diffs** | Formateador propio que solo toca las líneas que el programador ha modificado — nada de reformatear archivos enteros por accidente. |
| 🖥️ **Editor de fuente como en SAP GUI** | Editor embebido en la propia pestaña: modos de visualización o edición, clases por bloques o completas, descriptores editables, navegación directa a REPT/CUA/Dynpros e includes locales, y control total de los tiempos de espera contra SAP. |
| 🐞 **Depurador ABAP integrado** | Breakpoints desde el editor y una ventana de depuración por cada ejecución en SAP, en paralelo: breakpoints de sentencia, método, función, FORM, excepción o mensaje, watchpoints, cambio de valores y tablas internas editables. |
| 🔎 **Dónde se usa** | Referencias de utilización de la palabra del cursor (`Ctrl+Shift+F3`) o de cada mensaje de una clase de mensajes, con la sentencia de cada uso y salto directo a la línea. |
| ✉️ **Clases de mensajes** | Alta y edición de clases de mensajes (SE91) en una tabla, con su texto explicativo y su lista de usos. |
| 🧯 **Dumps de cualquier fecha, sin gastar tokens** *(función ampliada)* | Tu IA busca dumps de cualquier fecha (no solo los de las últimas 24 h del ADT estándar): primero una lista compacta con la clave, el error y la posición de cada dump; después, solo del que interesa, el resumen de ST22 y la pila de llamadas. Las variables o el dump completo, solo si hacen falta. Menos texto para la IA, menos tokens y respuestas más rápidas. |
| 🧩 **Más allá del ADT estándar** *(función ampliada)* | Edición de elementos de texto (REPT), diccionario de datos, pantallas GUI Status/Title y Dynpros — todo lo que el ADT de SAP no te deja tocar desde fuera de SAP GUI. |

---

## Qué cubre IDEA frente a otras herramientas

Comparativa sobre SAP ECC con NetWeaver 7.50 entre el ADT de SAP para Eclipse, otras extensiones ABAP de VS Code, el componente ABAP «ADT Ampliado» y la propia IDEA.

🟢 Cubierto · 🟡 Parcial · 🔴 No disponible · ➖ Lo resuelve el ADT estándar · **AMP** Requiere ADT Ampliado

| Funcionalidad | SAP ADT | Otras extensiones | ADT Ampliado | IDEA |
|---|---|---|---|---|
| **Objetos con código fuente** | | | | |
| Programas, includes y reports | 🟢 | 🟢 | ➖ | 🟢 |
| Clases e interfaces | 🟢 | 🟢 | ➖ | 🟢 Por bloques (método a método) o completa, como en SE24 |
| Includes locales de clase <br><sub>`CCDEF · CCIMP · CCMAC · CCAU`</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Grupos y módulos de función | 🟢 | 🟢 | ➖ | 🟢 Árbol del grupo; sin alta |
| Descriptores de clase <br><sub>Textos cortos de métodos, atributos y parámetros</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Tabla editable en el editor |
| Vistas CDS y grupos de tipos <br><sub>`DDLS · TYPE`</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Clases de mensajes <br><sub>`MSAG`</sub> | 🟢 | 🟢 | ➖ | 🟢 Alta, edición en tabla, texto explicativo y dónde se usa cada mensaje |
| **Diccionario de datos** | | | | |
| Elementos de datos <br><sub>`DTEL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Dominios <br><sub>`DOMA`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Valores fijos incluidos |
| Estructuras <br><sub>`TABL`</sub> | 🟢 | 🟢 Como código fuente | 🟢 | 🟢 **AMP** Editor de campos con navegación |
| Tablas de base de datos <br><sub>`TABL`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| Tipos tabla <br><sub>`TTYP`</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** |
| **Textos e interfaz clásica** | | | | |
| Elementos de texto <br><sub>`REPT` · símbolos de texto y textos de selección</sub> | 🟡 Según release | 🟡 Según release | 🟢 | 🟢 **AMP** |
| GUI Status / Title <br><sub>`CUAD` · SE41</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Alta, baja y edición de funciones, status y barra |
| Dynpros <br><sub>`DYNP` · SE51</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Editor visual de campos y contenedores |
| **RAP y OData** | | | | |
| Objetos de negocio RAP <br><sub>`BDEF · SRVD` · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🟡 Según extensión, como código fuente | 🔴 | 🔴 |
| Generador RAP <br><sub>Tabla, CDS, comportamiento y servicio en un paso · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| Servicios OData RAP <br><sub>`SRVB` · service binding y vista previa Fiori · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| **Ciclo de vida del objeto** | | | | |
| Buscar objetos | 🟢 | 🟢 | ➖ | 🟢 Con recientes e histórico |
| Crear objetos de código <br><sub>Programas, clases y funciones</sub> | 🟢 | 🟢 | 🟢 Programas y clases | 🟡 **AMP** Programas, clases y clases de mensajes; sin funciones |
| Crear objetos de diccionario <br><sub>`DTEL · DOMA · TABL · TTYP`</sub> | 🟡 Solo estructuras | 🟡 Solo estructuras | 🟢 | 🟢 **AMP** |
| Modo Visualización / Edición <br><sub>Bloqueo explícito del objeto, como en SE38</sub> | 🟡 Bloquea al empezar a escribir | 🟡 Bloquea al empezar a escribir | 🟢 Cualquier objeto, también dynpros | 🟢 Ctrl+F1, estado siempre visible |
| Orden de transporte al grabar | 🟢 | 🟢 | 🟢 Órdenes abiertas y alta de orden | 🟢 |
| Activación y objetos inactivos | 🟢 | 🟢 Activación en masa | ➖ | 🟢 Aviso de partes modificadas |
| Gestión de órdenes <br><sub>Liberar, cambiar propietario, ATC sobre la orden</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Versiones y comparación | 🟢 | 🟢 Más autoría por línea (blame) | ➖ | 🟡 Historial de la sesión con diff |
| abapGit | 🟢 Plugin | 🟢 | ➖ | 🔴 |
| **Escribir código** | | | | |
| Autocompletado e ir a definición | 🟢 | 🟢 | ➖ | 🟢 F2 como en SAP GUI |
| Comprobación de sintaxis | 🟢 | 🟢 | ➖ | 🟢 |
| Formateo | 🟢 | 🟢 | ➖ | 🟢 Estándar de SAP o propio de la extensión (solo las líneas modificadas) |
| Referencias de utilización <br><sub>Where-used list</sub> | 🟢 | 🟢 | ➖ | 🟢 De la palabra del cursor y de cada mensaje; con la sentencia de cada uso |
| Refactorización <br><sub>Renombrar, extraer método</sub> | 🟢 | 🟡 Correcciones rápidas | ➖ | 🔴 |
| Utilidades al estilo SAP GUI <br><sub>Comentar con *, unir y dividir sentencias, saltar entre bloques</sub> | 🟡 | 🔴 | ➖ | 🟢 |
| Sugerencias de IA en el editor | 🔴 | 🟢 GitHub Copilot | ➖ | 🟢 Claude, Gemini o GitHub Copilot |
| **Probar y analizar** | | | | |
| Depurador | 🟢 | 🟢 | ➖ | 🟢 Varias sesiones en paralelo; breakpoints de todo tipo, watchpoints, disposición y atajos configurables |
| ABAP Unit | 🟢 | 🟢 | ➖ | 🔴 |
| ATC / Code Inspector | 🟢 | 🟢 | ➖ | 🔴 |
| Trazas de rendimiento | 🟢 | 🟢 | ➖ | 🔴 |
| Dumps de las últimas 24 horas <br><sub>ST22 · feed estándar de ADT</sub> | 🟢 | 🟢 | ➖ | 🟡 Sin pantalla: obtiene los dumps por ADT estándar para dárselos a la IA |
| Dumps de cualquier fecha <br><sub>ST22 · entre fechas, con detalle completo y pila de llamadas</sub> | 🔴 Solo las últimas 24 horas | 🔴 Solo las últimas 24 horas | 🟢 | 🟡 **AMP** Sin pantalla: lista y detalle por ADT Ampliado, optimizados para ahorrar tokens de la IA |
| Consultas de datos <br><sub>SELECT de solo lectura</sub> | 🟢 Consultas simples | 🟢 Consultas simples | 🟢 Consultas complejas | 🟢 **AMP** Consultas complejas, para la IA |
| **IA y varios sistemas** | | | | |
| Servidor MCP para cualquier asistente de IA <br><sub>Claude Code, Copilot, Cursor…</sub> | 🔴 | 🟢 Depende de la extensión | ➖ | 🟢 |
| Varios sistemas a la vez <br><sub>Por ejemplo, desarrollo y producción</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Conexión de solo consulta <br><sub>Para sistemas productivos</sub> | 🔴 | 🟡 Aviso en producción | 🟢 | 🟢 La IA no puede escribir ni activar |
| Abrir en SAP GUI lo no soportado | - | 🟢 SAP GUI o Web GUI | ➖ | 🟢 SAP GUI o Web GUI, directo al objeto |

*ADT Ampliado* no es un editor: es el servicio ABAP que da a IDEA lo que el ADT estándar no expone. Sin él, IDEA abre en SAP GUI los objetos marcados **AMP**. En S/4HANA (NetWeaver 7.52 o superior) el ADT estándar trae editores propios para más objetos de diccionario y para elementos de texto. Las capacidades de IA de SAP (Joule) no están disponibles en ECC. RAP y los servicios OData RAP tampoco: en ECC los servicios OData se crean con SEGW en SAP GUI.

---

## Cómo funciona

1. **Configura tus conexiones a SAP** con `IDEA: Gestionar Conexiones SAP` — Define todas las conexiones a los sistemas SAP con los que quieras trabajar, para que desde el chat de la IA puedas indicar contra qué entorno quieres que trabaje; al iniciar VS Code se conectarán los servidores MCP para cada sistema (esto no hace nada en los sistemas, solo deja escuchando el servidor MCP). Configura una de las conexiones para que se autoarranque con VS Code.
2. **Busca el objeto** que necesitas desde el panel lateral «IDEA».
3. **Pide a tu IA** que lo modifique, o edítalo tú mismo con autocompletado, formateo y navegación a definiciones.
4. **Actívalo con un atajo** (`Ctrl+F3`). IDEA gestiona el bloqueo, la orden de transporte y la activación por ti.

No hace falta abrir el objeto manualmente antes de pedirle algo a tu IA: con la conexión MCP activa, ella misma puede buscarlo, leerlo y modificarlo directamente en SAP.

> Para que tu IA aproveche todo el potencial de IDEA, pídele explícitamente que use las herramientas MCP de IDEA para leer y escribir en SAP, en vez de editar a mano el objeto en el editor.

---

## Editor de fuente en WebView: como en SAP GUI, pero en VS Code

Editor de código fuente embebido directamente en la pestaña con el mismo motor que usa VS Code (Monaco), pensado para trabajar contra SAP igual que en SE24/SE38 con mucha operativa a mano.

**Edita las clases como en SAP GUI**
- **Todo el fuente o por bloques**: alterna entre ver la clase completa o solo el método que te interesa, con su *definición* arriba y su *implementación* abajo, ambas editables y con el mismo scroll — igual que en SE24.
- **Descriptores**: edita en una tabla propia los textos cortos de atributos, tipos, métodos, eventos y parámetros de la clase o interfaz, sin salir del editor; se graban junto con el resto del fuente.
- **Botón Navegar**: salta directamente a los elementos de texto (REPT), al GUI Status/Title (CUA) y a las pantallas (Dynpros) del objeto, y a los includes locales de la clase — definiciones (`CCDEF`), implementaciones (`CCIMP`), macros (`CCMAC`) y clases de test ABAP Unit (`CCAU`) —, cada uno en su propia pestaña.

**Dónde se usa (referencias de utilización)**
- **Botón Referencias** (`Ctrl+Shift+F3`): lista dónde se usa el identificador bajo el cursor — clase, interfaz, método, atributo, variable, programa, función, tipo, elemento de datos, tabla, estructura o dominio.
- Cada uso muestra el tipo de objeto, su nombre, la línea y la sentencia completa; clic en la fila y se abre el objeto en esa línea.
- Desde un `MESSAGE e001(zclase)` o un `MESSAGE ID 'ZCLASE' ... NUMBER '001'`, `F2` navega a la clase de mensajes con el foco en ese mensaje.

**Depuración desde el editor**
- **Botón Breakpoint** (`F9`): pone o quita un breakpoint en la línea del cursor; se marca en rojo en el margen.
- **Botón Ejecutar** (`Ctrl+F8`): abre el objeto en Web GUI para lanzarlo y que pare en los breakpoints.

**Control absoluto de los momentos de espera en SAP**
- Mientras se bloquea, graba, activa o formatea contra SAP, el editor se bloquea entero (una capa indica qué se está haciendo) para que no se pueda seguir escribiendo ni lanzar otra acción mientras SAP responde.
- Si SAP tarda demasiado, el editor se desbloquea solo y avisa, en vez de dejarte esperando sin saber qué está pasando.
- El estado del objeto — *Sin modificar*, *Modificado no grabado* o *Modificado no activado* — se ve siempre en la propia barra del editor.

**Toda la operativa, a un clic desde su propia barra de herramientas**
- Botones para Modificar/Visualizar, Grabar, Activar, Buscar y reemplazar, Historial de versiones (con comparador de diferencias integrado), Modificaciones de la sesión, Descriptores, Navegar y Mensajes — sin pasar por la paleta de comandos.
- **Atajos de teclado configurables** por acción, con validación de conflictos y comunes a todas las ventanas de VS Code.
- Snippets, autocompletado contra SAP y sugerencias de código de IA integradas en el propio editor.

---

## Depurador ABAP

Depura en VS Code los programas que se ejecutan en SAP, con una ventana propia por cada ejecución.

1. **IDEA: Iniciar depuración ABAP** deja a la conexión activa escuchando las ejecuciones en SAP.
2. Pon breakpoints en el editor con `F9` (o el botón *Breakpoint*).
3. Ejecuta el programa en SAP (por ejemplo, con el botón *Ejecutar* del editor, que lo abre en Web GUI).
4. Cuando la ejecución llega a un breakpoint, se abre una ventana de depuración. Si llegan varias ejecuciones, se abre una ventana por cada una, en paralelo (hasta 4; por encima se liberan sin abrir ventana).
5. **IDEA: Detener depuración ABAP** quita de SAP los breakpoints puestos y cierra las sesiones.

**La ventana de depuración**
- **Barra de herramientas**: Paso a paso (`F5`), Ejecutar (`F6`), Retorno (`F7`), Continuar (`F8`), breakpoint en la línea (`F9`), otros breakpoints (`Shift+F9`), watchpoint (`Shift+F4`), lista de breakpoints y watchpoints, disposición (`F10`) y atajos.
- **Cabecera fija**: programa, include, tipo y nombre del bloque, línea, `SY-SUBRC` y `SY-TABIX`.
- **Código**: siempre en visualización; los métodos se ven por bloques como en el editor. Doble clic en el número de línea pone o quita un breakpoint; doble clic o `F2` sobre una variable la añade a *Variables*; `F12` pasa a la instrucción del cursor.
- **Variables, Locales y Globales**: nombre, valor, tipo técnico, tipo absoluto y valor hexadecimal. Los valores se cambian con el lápiz; las estructuras se despliegan; las tablas internas se ven por páginas, con alta y baja de filas. Todo se puede copiar al portapapeles para pegarlo en una hoja de cálculo.
- **Navegación**: la pila de llamadas (nivel, tipo y evento, programa, include y línea); doble clic para ver otro nivel.
- **Otros breakpoints**: de sentencia ABAP, método (de clase global o local), función, FORM, excepción de clase, mensaje o código fuente, con condición opcional. Se recuerdan y se vuelven a poner en la siguiente ejecución del programa.
- **Watchpoints**: paran cuando cambia una variable, con condición opcional.
- **Disposición de la pantalla configurable**: tú decides cuántas filas y columnas y qué frame va en cada celda (Código, Navegación, Variables, Locales, Globales). Se guardan con nombre y valen para todas las ventanas; el tamaño de cada frame se cambia arrastrando las barras que los separan.
- **Atajos de teclado configurables** para todas las acciones, desde el propio panel (botón *Atajos*) o con el ajuste `idea.depuracion.atajos`.

---

## Clases de mensajes (SE91)

Desde «Búsqueda objeto SAP» (tipo *Clase de mensajes*), o navegando con `F2` desde un `MESSAGE`, se abre la clase en una tabla editable. Va entera por el ADT estándar, sin necesidad del componente ampliado.

- Se abre en Modo Visualización; *Editar* bloquea la clase y *Guardar* la graba pidiendo la orden de transporte si hace falta.
- Tabla con número, texto, longitud y marca de autoexplicativo; se filtra por columna y se puede copiar entera al portapapeles.
- Alta y baja de mensajes, y validación al guardar (números de 3 cifras sin repetir, textos obligatorios y longitud máxima).
- Por cada mensaje: ver su **texto explicativo**, ver **dónde se usa** (con salto directo a cada uso) o abrirlo en SE91.
- Con el botón *Nuevo* de «Búsqueda objeto SAP» se crea una clase de mensajes vacía y se abre en Modo Edición.

---

## Inicio rápido

1. Instala la extensión y recarga VS Code.
2. `Ctrl+Shift+P` → **IDEA: Gestionar Conexiones SAP** → da de alta tus sistemas o entornos SAP.
3. Define en la configuración una carpeta local para los ficheros temporales (`idea.mcpServer.tempFilesPath`).
4. Recarga la ventana (**Desarrollador: Recargar ventana**).

Listo: la extensión ya busca, edita y activa contra SAP, y tu asistente de IA ya se puede usar para que analice, investigue, modifique,... Para que te ayude.

---

## Servidor MCP: tu IA, trabajando directamente en SAP

El servidor MCP permite que un asistente de IA lea y modifique código ABAP directamente en el sistema SAP conectado. No trabaja sobre copias locales: todo va contra SAP, con las mismas garantías de bloqueo y activación que el resto de la extensión.

**Acciones para desarrollar disponibles para la IA:**
- Consultar a qué sistema SAP está conectada.
- Buscar objetos por nombre.
- Leer el código de un objeto.
- Abrir un objeto en VS Code bajo control de la extensión.
- Escribir el código de un objeto (con confirmación).
- Activar un objeto.

**Conexión desde tu cliente MCP:** añade un servidor de tipo `http` apuntando a `http://127.0.0.1:<puerto>` (puerto configurable, por ejemplo, `4856`).

---

## 🔐 Seguridad y control

- IDEA no guarda código fuente en la nube: todo se lee y escribe directamente contra tu sistema SAP. El fuente que abre se guarda en ficheros temporales en tu ordenador. Se borran en cuanto cierras la ventana de edición.
- Las contraseñas se guardan cifradas en el almacén seguro de VS Code, nunca en texto plano ni en la configuración.
- Con `idea.mcpServer.confirmWrites` (activo por defecto), toda escritura o activación propuesta por la IA lleva una pregunta de confirmación previa. Además, se muestra como diff antes de aplicarse.
- El servidor MCP escucha solo en `127.0.0.1` (tu propio equipo).
- Las consultas de datos son solo consultas, SELECT. Nunca modifican datos de las tablas.
- Si marcas la conexión como "Permite desarrollo" a false, te garantizas que la IA nunca modificará nada en el sistema ni objetos ni datos.

---

## Funciones ampliadas (con licencia)

Con un pequeño componente instalado en tu sistema SAP (configurado en `idea.endpointAmpliacionADT`), IDEA desbloquea dentro de VS Code lo que ni el ADT estándar de SAP ofrece:

- **Consultas de datos** La IA puede consultar las tablas de SAP (solo lectura) Esto es lo que permite que las IAs den todo su potencial.
- **Dumps de cualquier fecha (ST22)**, no solo los de las últimas 24 horas del ADT estándar, y optimizados para la IA: lista compacta, detalle solo del dump que interesa y datos completos solo si hacen falta, con lo que la IA gasta muchos menos tokens.
- **Crear la estructura vacía de una clase, programa o interfaz**
- **Elementos de texto (REPT)** de programas, clases e interfaces — edición directa, sin SE38/SE24.
- **Diccionario de datos**: Elementos de datos, estructuras, dominios y tipos tabla, con navegación cruzada entre ellos.
- **GUI Status / Title** de programas: Alta, baja y edición visual de funciones, status y barra de herramientas.
- **Dynpros (SE51)**: Editor visual de campos y contenedores, con validación al guardar.

Sin este componente configurado, estas acciones siguen disponibles: simplemente abren el objeto en SAP GUI clásico en lugar de en VS Code.

📩 **¿Quieres la licencia completa para tu equipo o consultoría?** Escribe a [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Referencia técnica

<details>
<summary><strong>📋 Comandos y atajos de teclado</strong></summary>

**Edición, guardado y activación**

| Comando | Atajo | Descripción |
|---|---|---|
| `IDEA: Alternar Modo Edición / Visualización` | `Ctrl+F1` | Cambia entre Modo Edición (bloquea el objeto en SAP) y Modo Visualización (lo libera). |
| `IDEA: Grabar objeto ABAP` | `Ctrl+S` | Graba en local y en SAP. Si el objeto es transportable, pide la orden de transporte **antes** de grabar nada. |
| `IDEA: Activar objeto ABAP` | `Ctrl+F3` | Formatea el objeto y lo activa en SAP. |
| `IDEA: Cancelar cambios y volver a Visualización` | `Ctrl+Shift+U` | Descarta los cambios sin guardar y vuelve a Modo Visualización. |
| `IDEA: Ver bloques modificados desde la última activación` | — | (Clases e interfaces) Lista los métodos y secciones tocados desde la última activación y salta al elegido. También desde el botón «N modificaciones» de la barra de estado. |
| `IDEA: Formatear documento` | `Shift+F1` | Formatea el objeto con el motor configurado. |

**Escritura de código**

| Comando | Atajo | Descripción |
|---|---|---|
| `IDEA: Comentar/descomentar línea (* en columna 1)` | `Ctrl+<` | Comenta o descomenta las líneas seleccionadas con `*` en la columna 1, al estilo SAP. |
| `IDEA: Unir sentencias en las menos líneas posibles` | `Ctrl+Shift+J` | Une varias líneas en una sola sentencia. |
| `IDEA: Dividir Sentencia en Líneas` | `Ctrl+Shift+K` | Divide una sentencia larga (`SELECT`, `CALL METHOD`, etc.) en varias líneas. |
| `IDEA: Dividir Sentencia declarativas en Líneas` | `Ctrl+Shift+D` | Separa declaraciones encadenadas `DATA:` / `TYPES:` en sentencias individuales. |

**Navegación y búsqueda**

| Comando | Atajo | Descripción |
|---|---|---|
| `IDEA: Buscar y Navegar a bloque de código` | `Ctrl+Alt+M` / `Ctrl+Shift+Z` | Lista rápida para saltar a un METHOD / FORM / MODULE / evento del archivo. |
| `IDEA: Ir al inicio del bloque` | `Ctrl+Shift+↑` / `Ctrl+Alt+RePág` | Salta al inicio del bloque en el que está el cursor. |
| `IDEA: Ir al final del bloque` | `Ctrl+Shift+↓` / `Ctrl+Alt+AvPág` | Salta al final del bloque en el que está el cursor. |
| Ir a definición | `F2` / `F12` / `Ctrl+Click` | Navega a la definición del objeto bajo el cursor. En ficheros ABAP, `F2` sustituye a «Cambiar nombre» (como en SAP GUI). |
| `IDEA: Buscar y reemplazar` | `Ctrl+Shift+F` | Abre el panel «Búsqueda en el código» con el foco en el campo de buscar. Funciona siempre, no solo en el editor ABAP. |

**Depuración**

| Comando | Atajo | Descripción |
|---|---|---|
| `IDEA: Iniciar depuración ABAP` | — | Deja la conexión activa escuchando las ejecuciones en SAP; cada una que pare en un breakpoint abre su ventana de depuración. |
| `IDEA: Breakpoint en la línea actual` | `F9` | Pone o quita un breakpoint en la línea del cursor. |
| `IDEA: Detener depuración ABAP` | — | Quita de SAP los breakpoints puestos, para la escucha y cierra las ventanas de depuración. |
| Referencias de utilización | `Ctrl+Shift+F3` | (Editor de fuente) Dónde se usa el identificador bajo el cursor. |
| Ejecutar en Web GUI | `Ctrl+F8` | (Editor de fuente) Abre el objeto en Web GUI para ejecutarlo. |

**Conexiones, servidor MCP y SAP GUI**

| Comando | Atajo | Descripción |
|---|---|---|
| `IDEA: Gestionar Conexiones SAP` | — | Añade, edita o elimina los sistemas SAP disponibles. |
| `IDEA: Cambiar Conexión Activa` | — | Elige contra qué sistema SAP trabaja esta ventana. También con clic en la conexión de la barra de estado. |
| `IDEA: Cerrar Todas las Conexiones` | — | Cierra la conexión activa y detiene los servidores MCP de esta ventana. |
| `IDEA: Iniciar Servidor MCP` | `Ctrl+Alt+S` | Arranca el servidor MCP de una conexión. |
| `IDEA: Detener Servidor MCP` | — | Detiene un servidor MCP en marcha. |
| `IDEA: Abrir SAP GUI` | — | Abre una ventana de SAP GUI clásico contra la conexión que elijas. |
| `IDEA: Mostrar README (idioma de VS Code)` | — | Abre este README en el idioma del editor. |

Salvo `Ctrl+Shift+F`, los atajos se aplican con el editor ABAP en foco. En ficheros que no son ABAP, `Ctrl+F3` conserva su función original de VS Code («Buscar siguiente selección»). Además: **Format Document** (`Shift+Alt+F`), autocompletado (`Ctrl+Space`) y plegado de código.

</details>

<details>
<summary><strong>⚙️ Configuración completa</strong></summary>

Ajustes bajo `idea.*` (Archivo → Preferencias → Configuración, o desde el panel «Configuración» de IDEA).

**Formateo (Pretty Printer)**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (por defecto), `sapConfig` | Motor que formatea al usar «Format Document» y antes de activar. `extension`: el formateador propio. `sapConfig`: el Pretty Printer configurado en SAP (solo objetos abiertos desde «Búsqueda objeto SAP»). |
| `idea.prettyprinter.indentation` | `true` (por defecto), `false` | Activa o no el sangrado automático. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (por defecto), `false` | Elimina o no los espacios dobles. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (por defecto), `lowerKeywords`, `upperAll`, `lowerAll` | Mayúsculas/minúsculas: solo palabras clave, o todo el código. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (por defecto), `modoSe24`, `estandar` | Sangría de `METHOD` / `ENDMETHOD` (solo clases). `auto`: respeta los espacios existentes. `modoSe24`: columna 0. `estandar`: un nivel (2 espacios). |
| `idea.prettyprinter.formatScope` | `fullFile` (por defecto), `currentMethodOnly` | Al formatear con atajo (solo clases): todo el archivo o solo el método donde está el cursor. |

**Autocompletado**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (por defecto), `false` | Al insertar la llamada a un método o función con `Ctrl+Space`, incluye el comentario de cada parámetro. En `false` inserta solo los parámetros. |

**Conexiones y servidor MCP**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.mcpServer.connections` | Lista de sistemas SAP | Sistemas disponibles. Se edita con «IDEA: Gestionar Conexiones SAP». La contraseña **no** se guarda aquí: se pide y se almacena cifrada en el almacén seguro de VS Code. Campos de cada conexión en la tabla siguiente. |
| `idea.mcpServer.config` → `mcpInicial` | Nombre de una conexión (vacío por defecto) | Conexión que queda **activa** al abrir VS Code. Vacío = ninguna. |
| `idea.mcpServer.confirmWrites` | `true` (por defecto), `false` | Pide confirmación (mostrando un diff) antes de que la IA escriba o active código en SAP. |
| `idea.mcpServer.tempFilesPath` | Ruta de carpeta (vacío por defecto) | Carpeta donde se crean los ficheros `.abap` temporales de «Búsqueda objeto SAP». **Obligatoria** para poder buscar y abrir objetos. Los ficheros se borran al cerrar su pestaña o al cerrar VS Code. |

**Campos de cada conexión**

| Campo | Obligatorio | Qué hace |
|---|---|---|
| Nombre | Sí | Identificador del sistema (ej. `DEV`, `QAS`). Es el nombre con el que la IA y la barra de estado se refieren a él. |
| URL | Sí | URL base del sistema SAP (ej. `https://miserver.midominio.com:44300`). |
| Mandante | Sí | Mandante SAP (ej. `100`). |
| Usuario | Sí | Usuario SAP. |
| Puerto MCP | Sí | Puerto local (`127.0.0.1`) del servidor MCP de esta conexión. Debe ser distinto en cada conexión. |
| Idioma | No | Idioma de logon en SAP. No cambia el idioma de la extensión, que es siempre el de VS Code. |
| Permitir certificados no confiables | No (`false`) | Acepta certificados TLS autofirmados para este sistema. |
| ID del sistema SAP (SID) | No | SID tal como figura en tu SAP Logon. Necesario para abrir SAP GUI clásico. |
| Permite desarrollo | No (`true`) | Si se desmarca, la conexión es de **solo consulta**: la IA solo puede buscar, leer, abrir en Visualización, consultar datos y listar dumps; no puede escribir ni activar. Pensado para sistemas productivos. |
| Arranque silencioso | No (`false`) | Arranca el servidor MCP de esta conexión al abrir VS Code, sin preguntar. Se pueden marcar varias conexiones para tener varios servidores en marcha a la vez. |

**Depurador**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.depuracion.atajos` | Objeto acción → tecla | Atajos de la ventana de depuración. Por defecto: `F5` paso a paso, `F6` ejecutar, `F7` retorno, `F8` continuar, `F9` breakpoint, `Shift+F9` otros breakpoints, `Shift+F4` watchpoint, `F2` añadir variable, `F12` pasar a instrucción, `F10` disposición. También se cambian desde el botón *Atajos* del panel. |

**Operativa ampliada y SAP GUI**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.endpointAmpliacionADT` | Ruta del servicio (vacío por defecto), p.ej. `/sap/serviciosazure/` | Habilita las funciones ampliadas (consultas de datos, elementos de texto REPT, diccionario, GUI Status/Title, Dynpros). Si se deja vacío, esas acciones abren el objeto en SAP GUI. |
| `idea.sapGui.sapshcutPath` | Ruta a `sapshcut.exe` (vacío por defecto) | Solo si SAP GUI no está en una ubicación estándar ni en el PATH. |
| `idea.navigation.gui` | `sapGui` (por defecto), `webGui` | Al navegar a la definición de un objeto que la extensión no edita, elige entre SAP GUI clásico (`sapshcut.exe`, necesita *ID del sistema SAP*) o la Web GUI en el navegador. |

</details>

<details>
<summary><strong>🔌 Conexión activa y servidores MCP</strong></summary>

IDEA distingue dos conceptos:

- **Conexión activa**: el sistema SAP contra el que trabaja *esta ventana* de VS Code (búsqueda, edición, activación). Se ve y se cambia desde la barra de estado. Al abrir VS Code se activa la indicada en `mcpInicial`. Una misma conexión no puede estar activa en dos ventanas a la vez. Al cambiar de conexión, IDEA cierra antes todo lo abierto de la anterior (pidiendo confirmación si hay cambios sin guardar).
- **Servidores MCP**: uno por conexión, cada uno en su propio puerto. Pueden estar varios en marcha a la vez, de modo que la IA puede trabajar en DEV y consultar QAS en paralelo.

**Conectar tu cliente MCP:**
- **Clientes integrados en VS Code**: IDEA publica automáticamente el servidor de la conexión activa (`IDEA – <conexión>`); no hay que configurar nada.
- **Clientes externos** (Claude Code, Cursor…): añade un servidor de tipo `http` apuntando a `http://127.0.0.1:<puerto>/mcp`, con el *Puerto MCP* de la conexión. Uno por cada conexión que quieras usar.

**Herramientas MCP disponibles para la IA**

| Herramienta | Qué hace | Solo consulta |
|---|---|:---:|
| `abap_connection_info` | Indica a qué sistema SAP está conectado el servidor. | ✅ |
| `abap_search_object` | Busca objetos por nombre. | ✅ |
| `abap_read_object_source` | Lee el código fuente de un objeto. | ✅ |
| `abap_open_object` | Abre un objeto en VS Code bajo control de la extensión. | ✅ |
| `abap_execute_query` | Ejecuta una consulta `SELECT` de solo lectura sobre la base de datos *(función ampliada)*. | ✅ |
| `abap_list_dumps_24h` | Lista los dumps de ejecución de las últimas 24 horas (feed ADT estándar). | ✅ |
| `abap_list_dumps` | Lista los dumps de ejecución de cualquier fecha (equivalente a ST22), en formato compacto *(función ampliada)*. | ✅ |
| `abap_get_dump_detalle` | Devuelve el detalle de un dump: resumen de ST22 y pila de llamadas; variables o dump completo solo si se piden *(función ampliada)*. | ✅ |
| `abap_write_object_source` | Escribe el fuente de un objeto (con diff y confirmación). | — |
| `abap_activate_object` | Activa un objeto (con confirmación). | — |
| `abap_llamar_herramienta_desarrollo` | Operaciones del componente ampliado: bloqueos, órdenes de transporte, elementos de texto… (con confirmación) *(función ampliada)*. | — |

La columna *Solo consulta* indica las herramientas disponibles en conexiones con **Permite desarrollo** desmarcado.

</details>

<details>
<summary><strong>🖥️ Panel lateral «IDEA» en detalle</strong></summary>

El icono de IDEA en la barra de actividad abre cuatro secciones.

**1. Búsqueda en el código**: busca y reemplaza texto dentro del archivo ABAP abierto en el editor. *Tipo de búsqueda*: parcial o palabra completa. *Alcance*: bloque actual o todo el archivo. Los resultados llevan número de línea (clic para saltar) y se pueden filtrar. *Reemplazar* ofrece previsualización antes de confirmar. Guarda un historial reciente.

**2. Búsqueda objeto SAP**: busca objetos en el sistema SAP de la conexión activa y los abre en VS Code (requiere el servidor MCP en marcha y `idea.mcpServer.tempFilesPath` configurada). El nombre admite `*` como comodín.
- **Programa / Report**, **Clase** y **Módulo de función**: se abren como fichero temporal editable, en Modo Visualización; se borran al cerrar la pestaña.
- **Clases**: botones para abrir sus includes locales: `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` y `<TEST>` (clases de test ABAP Unit).
- **Grupos de funciones**: muestra su árbol (módulos de función, includes y otras partes) para abrir cada pieza por separado.
- **Elemento de datos**, **Estructura / Tabla**, **Dominio**, **Tipo tabla**: se abren en el editor de diccionario *(función ampliada)*.
- **Botones REPT, CUA y DYNP** (según el tipo de objeto): abren los editores de elementos de texto, GUI Status/Title y Dynpros *(funciones ampliadas)*.
- **Clase de mensajes**: se abre en el editor de clases de mensajes (por ADT estándar, sin componente ampliado).
- **Botón Nuevo**: crea un programa, una clase, una clase de mensajes o un objeto de diccionario (elemento de datos, dominio, estructura/tabla, tipo tabla) indicando nombre y paquete. Sin el componente ampliado solo se pueden crear clases de mensajes.
- Si la búsqueda devuelve un único resultado, se abre directamente. Guarda **recientes** e **histórico** de búsquedas.
- Los objetos que la extensión no sabe editar se abren en SAP GUI clásico (o Web GUI, según `idea.navigation.gui`).

**3. Historial cambios en la sesión**: guarda copias del objeto cada vez que se graba o se activa un cambio real, y también cuando detecta que el objeto se ha cambiado directamente en SAP. Es solo de la sesión actual: se borra al cerrar la pestaña y no se conserva entre reinicios.
- *Cargar versiones*: tabla con la más reciente arriba, la hora del cambio, si se activó, su origen (*Local* o *Cambiado en SAP*) y el nº de cambios respecto a la última activación y a la versión anterior.
- Marca **dos** versiones y *Ver cambios*: abre el comparador de diferencias de VS Code.
- *Ver cambios totales*: compara la versión inicial con la actual.
- Marca **una** y *Recuperar versión*: vuelca su contenido en el editor (no lo guarda automáticamente).

**4. Configuración**: acceso rápido, sin salir del panel, a:
- Conexiones SAP: tabla con *Nombre*, *Arranque silen.* (su servidor MCP arranca al abrir VS Code), *AutoConexión* (la que queda activa al abrir VS Code) y *Desarrollo* (si permite desarrollo); el resto de datos (URL, mandante, usuario, puerto MCP) aparece al pasar el ratón por la fila. Botón *Gestionar conexiones…*.
- Pretty Printer: motor, alcance, indentación, espacios dobles, mayúsculas/minúsculas y sangría de `METHOD`.
- Servidor MCP: conexión inicial, confirmación de escrituras y carpeta de temporales.
- Navegación y SAP GUI: dónde abrir los objetos no editables, ruta de `sapshcut.exe` y servicio de ampliación de ADT.

</details>

<details>
<summary><strong>🧩 Funciones ampliadas en detalle</strong></summary>

**Consultas de datos.** Permite a la IA investigar los datos de tu sistema SAP con consultas `SELECT` de solo lectura (sin `INSERT`/`UPDATE`/`DELETE` ni DDL). Sin ella, la IA ve el código pero no los datos, y pierde buena parte de su capacidad de análisis.

**Editor de elementos de texto (REPT).** Desde el botón *REPT* de «Búsqueda objeto SAP», sobre un programa, clase o interfaz:
- Se abre en Modo Visualización (fondo azul).
- *Editar* bloquea el objeto en SAP (fondo ámbar); al modificar cualquier celda aparece 🔴 en la pestaña.
- *Guardar y activar* sube los textos a SAP (pidiendo orden de transporte si hace falta) y mantiene el bloqueo para seguir editando.
- Al volver a Visualización o cerrar la pestaña se libera el bloqueo.
- *Copiar* lleva toda la tabla de textos al portapapeles.

**Editor de diccionario.** Elementos de datos, estructuras / tablas, dominios y tipos tabla: cabecera, opciones técnicas y lista de campos o valores. Se abre en Visualización; *Editar* bloquea el objeto y permite modificarlo y activarlo con la misma gestión de orden de transporte que el resto. La cabecera de la tabla de campos queda fija al hacer scroll; columnas ordenables y filtrables. Desde las celdas se navega a otros elementos y dominios.

**GUI Status / Title (CUA).** Alta, baja y edición de títulos, funciones, status y barra de herramientas estándar.

**Dynpros (SE51).** Editor visual de campos y contenedores (marcos, subscreens, tabstrips, table controls): alta situando el elemento con un clic, detección de solapes y validación al guardar.

Todos ellos siguen la misma disciplina de bloqueo, orden de transporte y activación que el resto de objetos.

</details>

---

## Licencia

La extensión es de uso libre bajo licencia MIT.

Si estás interesado en las funcionalidades ampliadas, que requieren el componente ABAP «ADT Ampliado», contacta para condiciones y precios con Marcos Almeida Santolaria en [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

**Español** · [English](README.en.md) · [Deutsch](README.de.md) · [Français](README.fr.md)
