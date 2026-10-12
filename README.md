# <img src="https://raw.githubusercontent.com/abapinfo/idea-abap/main/resources/icon.png" alt="IDEA" height="40" align="absmiddle"> IDEA — Entorno de Desarrollo Integrado de ABAP

**Español** · [English](README.en.md) · [Deutsch](README.de.md) · [Français](README.fr.md)

> 💡 Para leer este README en otro idioma dentro de VS Code, ejecuta **IDEA: Mostrar README** (`Ctrl+Shift+P`): se abre automáticamente en el idioma de tu editor.

---

## ¿Qué es **IDEA**?

**IDEA** convierte Visual Studio Code (VS Code) en un entorno de trabajo con asistente de IA conectado a tus sistemas SAP. Con el componente *ADT Ampliado*, la IA puede investigar, analizar y proponer acciones y soluciones sobre tus propios datos y tu propio código.

Además, **IDEA** es un entorno de desarrollo ABAP completo en el que la IA:
- Propone cambios en el código fuente de tu sistema SAP, que tú revisas y aceptas o rechazas.
- Comprueba contra el sistema real que sus soluciones son válidas: que la clase, el módulo de función o los parámetros existen de verdad.
- Compara información entre varios sistemas (desarrollo, integración, producción…).
- Investiga y te ofrece la mejor solución.

**IDEA** controla que los cambios en el código sean seguros y que la IA nunca modifique datos de tu sistema SAP: solo puede consultarlos.

El coste de la IA también está controlado. El asistente que usa las herramientas de **IDEA** (Claude Code, GitHub Copilot…) se paga por suscripción, no por consumo. Solo las sugerencias de código en línea del editor, que son opcionales, pueden usar una API de pago por uso (por tokens), y se configuran aparte. Es decir, con **IDEA** trabajan dos modelos de IA: uno para las sugerencias mientras escribes y otro, el de tu asistente, que usa las herramientas de **IDEA**.

## Aplica la IA a tu negocio de forma segura, controlada y económica

**IDEA** conecta una IA a cualquiera de tus sistemas SAP para que trabaje sobre ellos: investiga, analiza y propone acciones y soluciones.

Imagina que tu negocio es una cadena de tiendas de electrónica y usas **IDEA** y la IA para responder a cualquiera de estas preguntas:

**1. Conoce la empresa**
- ¿Qué vende esta empresa? Descríbeme el catálogo en dos líneas.
- ¿Cuántos productos, clientes y pedidos tenemos?
- ¿Cuál es el producto más caro y cuál el más barato?
- ¿Qué categorías de producto hay y cuántos artículos tiene cada una?

**2. Ventas**
- ¿Cuánto hemos facturado cada año? ¿Qué año fue el mejor?
- ¿Cuáles son los 10 productos que más dinero han generado?
- ¿Hay estacionalidad? ¿En qué meses se vende más?
- ¿Cuál es el importe medio de un pedido? ¿Y el pedido más grande de la historia?
- ¿Cuántos pedidos están cobrados, pendientes de facturar o cancelados?

**3. Clientes y mapa**
- ¿Quiénes son nuestros 5 mejores clientes y de qué país es cada uno?
- ¿En qué países vendemos? Ordénalos por facturación.
- ¿Qué clientes llevan más tiempo sin comprarnos? (Detecta clientes perdidos.)
- ¿Qué cliente nos compra siempre el mismo producto?

**4. Productos y opiniones de clientes**
- ¿Cuáles son los productos mejor y peor valorados en las opiniones de los clientes?
- Resúmeme lo que dicen los clientes del peor valorado.
- ¿Hay algún producto que se vende mucho pero tiene malas opiniones?
- ¿Qué proveedor nos sirve los productos mejor valorados?

**5. Almacén**
- ¿Qué productos están por debajo del stock mínimo? ¿Cuánto habría que reponer?
- ¿Hay productos con mucho stock que apenas se venden? (Stock inmovilizado.)
- Para cada producto bajo mínimo, ¿quién es su proveedor y qué email tiene?

**6. Razonar y cruzar datos**
- Si mañana dejáramos de trabajar con nuestro mayor proveedor, ¿qué parte de las ventas perderíamos?
- ¿Qué productos se compran juntos con frecuencia? (Cesta de la compra.)
- Hazme un informe ejecutivo de 5 puntos sobre la salud del negocio.
- ¿Qué tres acciones me recomiendas para vender más el año que viene, basándote en los datos?
- Hay una caída de ventas en algún país: encuéntrala y explica por qué ha podido pasar.

## Desarrollo ABAP moderno, sin salir de VS Code

**IDEA** convierte VS Code en un entorno de desarrollo ABAP completo: conectado en tiempo real a tu sistema SAP y preparado para trabajar codo con codo con el asistente de IA que ya uses (Claude Code, GitHub Copilot, Cursor…).

Se acabó copiar y pegar código entre SAP GUI y un chat de IA. Se acabó perder de vista qué objeto está bloqueado, quién lo tocó o si sigue pendiente de activar. Con IDEA todo ocurre dentro del propio editor, con la misma disciplina de bloqueos, órdenes de transporte y activación que ya conoces de SAP, pero con la velocidad de VS Code y la potencia de la IA.

**En una frase:** busca un objeto → ábrelo → pide a tu IA que proponga el cambio (o hazlo tú) → grábalo y actívalo. Todo sin salir de VS Code, todo bajo control.

**En otra frase 😉:** ¿Ha fallado un IDoc? → pide a tu IA que lo analice y te indique la solución → aplícala. Todo sin salir de VS Code, todo bajo control.

---

## ¿Por qué le va a encantar a tu equipo?

| | |
|---|---|
| ⚡ **Rapidez real** | Búsqueda instantánea de programas, clases, interfaces y objetos de diccionario, con historial de búsquedas. Sin transacciones ni menús anidados. |
| 🤖 **IA con acceso directo a SAP** | Servidor MCP integrado: tu asistente de IA busca y lee el código y los datos de SAP y te propone los cambios en el editor, con las diferencias a la vista. Tú decides si los aceptas; nada se graba en SAP sin ti. |
| 🌐 **Multi-sistema** | Varios servidores MCP en marcha a la vez, uno por sistema: tu IA puede proponer cambios en desarrollo mientras consulta datos de producción con una conexión de solo consulta. |
| 🔒 **Cero sorpresas** | Modo Visualización por defecto, bloqueo explícito para modificar, y órdenes de transporte y activación gestionadas exactamente igual que en SAP estándar. |
| 🕘 **Historial al vuelo** | Cada grabación y cada activación quedan registradas en la pestaña del editor: compara versiones o recupera una anterior sin salir del editor. |
| 🎨 **Formateo que respeta tus diffs** | Formateador propio que puede limitarse a los métodos modificados, para no reformatear clases enteras por accidente. |
| 🖥️ **Editor de fuente como en SAP GUI** | Editor embebido en la propia pestaña: modos Visualizar y Modificar, clases por bloques o completas, descriptores editables, acceso directo a elementos de texto, GUI Status/Title, dynpros e includes locales, y control total de las esperas contra SAP. |
| 🐞 **Depurador ABAP integrado** | Breakpoints desde el editor y una ventana de depuración por cada ejecución en SAP, en paralelo: breakpoints de sentencia, método, función, FORM, excepción o mensaje, watchpoints, cambio de valores y tablas internas editables. |
| 🔎 **Dónde se usa** | Referencias de utilización de la palabra del cursor (`Ctrl+Shift+F3`) o de cada mensaje de una clase de mensajes, con la sentencia de cada uso y salto directo a la línea. |
| ✉️ **Clases de mensajes** | Alta y edición de clases de mensajes (SE91) en una tabla, con su texto explicativo y su lista de usos. |
| 🧯 **Dumps de cualquier fecha, sin gastar tokens** *(función ampliada)* | Tu IA busca dumps de cualquier fecha (no solo los de las últimas 24 h del ADT estándar): primero una lista compacta con la clave, el error y la posición de cada dump; después, solo del que interesa, el resumen de ST22 y la pila de llamadas. Las variables o el dump completo, solo si hacen falta. Menos texto para la IA, menos tokens y respuestas más rápidas. |
| 🧩 **Más allá del ADT estándar** *(función ampliada)* | Edición de elementos de texto (REPT), diccionario de datos, GUI Status/Title y dynpros: todo lo que el ADT de SAP no te deja tocar fuera de SAP GUI. |

---

## Qué cubre IDEA frente a otras herramientas

Comparativa sobre SAP ECC con NetWeaver 7.50 entre el ADT de SAP para Eclipse, otras extensiones ABAP de VS Code, el componente ABAP *ADT Ampliado* y la propia IDEA.

🟢 Cubierto · 🟡 Parcial · 🔴 No disponible · ➖ Lo resuelve el ADT estándar · **AMP** Requiere ADT Ampliado

| Funcionalidad | SAP ADT | Otras extensiones | ADT Ampliado | IDEA |
|---|---|---|---|---|
| **Objetos con código fuente** | | | | |
| Programas, includes y reports | 🟢 | 🟢 | ➖ | 🟢 |
| Clases e interfaces | 🟢 | 🟢 | ➖ | 🟢 Por bloques (método a método) o completas, como en SE24 |
| Includes locales de clase <br><sub>`CCDEF · CCIMP · CCMAC · CCAU`</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Grupos y módulos de función | 🟢 | 🟢 | ➖ | 🟢 Árbol del grupo; sin alta |
| Descriptores de clase <br><sub>Textos breves de métodos, atributos y parámetros</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Tabla editable en el editor |
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
| GUI Status / Title <br><sub>`CUAD` · SE41</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Alta, baja y edición de funciones, status y barra de herramientas |
| Dynpros <br><sub>`DYNP` · SE51</sub> | 🔴 | 🔴 | 🟢 | 🟢 **AMP** Editor visual de campos y contenedores |
| **RAP y OData** | | | | |
| Objetos de negocio RAP <br><sub>`BDEF · SRVD` · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🟡 Según extensión, como código fuente | 🔴 | 🔴 |
| Generador RAP <br><sub>Tabla, CDS, comportamiento y servicio en un paso · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| Servicios OData RAP <br><sub>`SRVB` · service binding y vista previa Fiori · solo NetWeaver 7.54 o S/4HANA</sub> | 🟢 | 🔴 | 🔴 | 🔴 |
| **Ciclo de vida del objeto** | | | | |
| Buscar objetos | 🟢 | 🟢 | ➖ | 🟢 Con recientes e histórico |
| Crear objetos de código <br><sub>Programas, clases y funciones</sub> | 🟢 | 🟢 | 🟢 Programas y clases | 🟡 **AMP** Programas, clases y clases de mensajes; sin funciones |
| Crear objetos de diccionario <br><sub>`DTEL · DOMA · TABL · TTYP`</sub> | 🟡 Solo estructuras | 🟡 Solo estructuras | 🟢 | 🟢 **AMP** |
| Modo Visualización / Edición <br><sub>Bloqueo explícito del objeto, como en SE38</sub> | 🟡 Bloquea al empezar a escribir | 🟡 Bloquea al empezar a escribir | 🟢 Cualquier objeto, también dynpros | 🟢 `Ctrl+F1`, estado siempre visible |
| Orden de transporte al grabar | 🟢 | 🟢 | 🟢 Órdenes abiertas y alta de orden | 🟢 |
| Activación y objetos inactivos | 🟢 | 🟢 Activación en masa | ➖ | 🟢 Aviso de partes modificadas |
| Gestión de órdenes <br><sub>Liberar, cambiar propietario, ATC sobre la orden</sub> | 🟢 | 🟢 | ➖ | 🔴 |
| Versiones y comparación | 🟢 | 🟢 Más autoría por línea (blame) | ➖ | 🟡 Historial de la sesión con diff |
| abapGit | 🟢 Plugin | 🟢 | ➖ | 🔴 |
| **Escribir código** | | | | |
| Autocompletado e ir a definición | 🟢 | 🟢 | ➖ | 🟢 `F2` como en SAP GUI |
| Comprobación de sintaxis | 🟢 | 🟢 | ➖ | 🟢 |
| Formateo | 🟢 | 🟢 | ➖ | 🟢 Estándar de SAP o propio de la extensión (puede limitarse a los métodos modificados) |
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
| Servidor MCP para cualquier asistente de IA <br><sub>Claude Code, Copilot, Cursor…</sub> | 🔴 | 🟢 Depende de la extensión | ➖ | 🟢 La IA propone los cambios en el editor; el usuario los acepta o rechaza |
| Varios sistemas a la vez <br><sub>Por ejemplo, desarrollo y producción</sub> | 🟢 | 🟢 | ➖ | 🟢 |
| Conexión de solo consulta <br><sub>Para sistemas productivos</sub> | 🔴 | 🟡 Aviso en producción | 🟢 | 🟢 La IA no puede proponer cambios ni modificar nada |
| Abrir en SAP GUI lo no soportado | - | 🟢 SAP GUI o Web GUI | ➖ | 🟢 SAP GUI o Web GUI, directo al objeto |

*ADT Ampliado* no es un editor: es el servicio ABAP que da a IDEA lo que el ADT estándar no expone. Sin él, IDEA abre en SAP GUI los objetos marcados **AMP**. En S/4HANA (NetWeaver 7.52 o superior) el ADT estándar trae editores propios para más objetos de diccionario y para elementos de texto. Las capacidades de IA de SAP (Joule) no están disponibles en ECC. RAP y los servicios OData RAP tampoco: en ECC los servicios OData se crean con SEGW en SAP GUI.

---

## Cómo funciona

1. **Configura tus conexiones a SAP** con `IDEA: Gestionar conexiones SAP`. Da de alta todos los sistemas SAP con los que quieras trabajar: así, desde el chat de la IA, podrás indicar contra qué sistema debe trabajar. Marca las conexiones cuyo servidor MCP quieras arrancar con VS Code (esto no hace nada en los sistemas SAP: solo deja el servidor MCP escuchando en tu equipo) y elige la que queda activa al abrir VS Code.
2. **Busca el objeto** que necesitas desde el panel lateral «IDEA».
3. **Pide a tu IA** que proponga el cambio, o hazlo tú mismo con autocompletado, formateo y navegación a definiciones.
4. **Graba y activa con un atajo** (`Ctrl+S` y `Ctrl+F3`). IDEA gestiona por ti el bloqueo, la orden de transporte y la activación.

No hace falta abrir el objeto antes de pedirle algo a tu IA: con la conexión MCP activa, ella misma puede buscarlo, leerlo, abrirlo en el editor y proponerte el cambio.

> Para que tu IA aproveche todo el potencial de IDEA, pídele explícitamente que use las herramientas MCP de IDEA para leer de SAP y proponer los cambios en el editor.

---

## Editor de fuente: como en SAP GUI, pero en VS Code

Editor de código fuente embebido en la propia pestaña (WebView), con el mismo motor que usa VS Code (Monaco), pensado para trabajar contra SAP igual que en SE24/SE38 y con toda la operativa a mano.

**Edita las clases como en SAP GUI**
- **Todo el fuente o por bloques** (`Ctrl+Alt+B`): alterna entre ver la clase completa o solo el método que te interesa, con su *definición* arriba y su *implementación* abajo, ambas editables y con el mismo scroll, igual que en SE24.
- **Descriptores**: edita en una tabla propia los textos breves de atributos, tipos, métodos, eventos y parámetros de la clase o interfaz, sin salir del editor; se graban junto con el resto del fuente.
- **Botón Abrir componente**: abre los elementos de texto (REPT), el GUI Status/Title (CUA) y las pantallas (dynpros) del objeto, y los includes locales de la clase: definiciones (`CCDEF`), implementaciones (`CCIMP`), macros (`CCMAC`) y clases de test ABAP Unit (`CCAU`), cada uno en su propia pestaña.

**Cambios propuestos por la IA**
- Cuando la IA propone un cambio, se abre la ventana *Cambio propuesto por la IA* con las diferencias entre el fuente actual y el propuesto, viendo el fuente completo o solo los cambios.
- *Aceptar* aplica el cambio en el editor como una edición que se puede deshacer (`Ctrl+Z`), **sin grabar en SAP**: lo revisas, lo grabas y lo activas tú. *Rechazar* lo descarta.
- Una cuenta atrás indica el tiempo que queda para revisarlo; al llegar a cero se pregunta si mantienes la revisión o cancelas el cambio.

**Dónde se usa (referencias de utilización)**
- **Botón Referencias** (`Ctrl+Shift+F3`): lista dónde se usa el identificador bajo el cursor: clase, interfaz, método, atributo, variable, programa, función, tipo, elemento de datos, tabla, estructura o dominio.
- Cada uso muestra el tipo de objeto, su nombre, la línea y la sentencia completa; con un clic en la fila se abre el objeto en esa línea.
- Desde un `MESSAGE e001(zclase)` o un `MESSAGE ID 'ZCLASE' ... NUMBER '001'`, `F2` navega a la clase de mensajes con el foco en ese mensaje.

**Depuración desde el editor**
- **Botón Breakpoint** (`F9`): pone o quita un breakpoint en la línea del cursor; se marca en rojo en el margen.
- **Botón Ejecutar** (`Ctrl+F8`): abre el objeto en Web GUI para lanzarlo y que pare en los breakpoints.

**Control absoluto de las esperas contra SAP**
- Mientras se bloquea, graba, verifica, activa o formatea contra SAP, el editor se bloquea entero (una capa indica qué se está haciendo), para que no se pueda seguir escribiendo ni lanzar otra acción mientras SAP responde.
- Si SAP tarda demasiado, el editor se desbloquea solo y avisa, en vez de dejarte esperando sin saber qué pasa.
- El estado del objeto (*Sin modificar*, *Modificado no grabado* o *Modificado no activado*) se ve siempre en la propia barra del editor.

**Toda la operativa a un clic, en su propia barra de herramientas**
- Botones para Modificar/Visualizar, Grabar, Verificar, Activar, Buscar y reemplazar, Historial de versiones (con comparador de diferencias), Modificaciones de la sesión, Descriptores, Abrir componente, Referencias, Mensajes, Maximizar y Cerrar, sin pasar por la paleta de comandos.
- **Verificar** (`Ctrl+F2`) comprueba la sintaxis en SAP del fuente actual sin grabarlo.
- **Maximizar** (`Ctrl+K Z`) pasa la pestaña a pantalla completa (modo Zen de VS Code) y la restaura.
- **Atajos de teclado configurables** por acción (botón *Atajos*), con validación de conflictos y comunes a todas las ventanas de VS Code.
- Snippets, autocompletado contra SAP y sugerencias de código de IA (Claude, Gemini o los modelos de VS Code, como Copilot) en el propio editor.

Los editores de elementos de texto, diccionario, GUI Status/Title, dynpros y clases de mensajes tienen también su botón *Cerrar* en la barra.

---

## Depurador ABAP

Depura en VS Code los programas que se ejecutan en SAP, con una ventana propia por cada ejecución.

1. **IDEA: Iniciar depuración ABAP** deja la conexión activa escuchando las ejecuciones en SAP.
2. Pon breakpoints en el editor con `F9` (o con el botón *Breakpoint*).
3. Ejecuta el programa en SAP (por ejemplo, con el botón *Ejecutar* del editor, que lo abre en Web GUI).
4. Cuando la ejecución llega a un breakpoint, se abre una ventana de depuración. Si llegan varias ejecuciones, se abre una ventana por cada una, en paralelo (hasta 4; por encima de ese número se liberan sin abrir ventana).
5. **IDEA: Detener depuración ABAP** quita de SAP los breakpoints puestos y cierra las sesiones.

**La ventana de depuración**
- **Barra de herramientas**: Paso a paso (`F5`), Ejecutar (`F6`), Retorno (`F7`), Continuar (`F8`), breakpoint en la línea (`F9`), otros breakpoints (`Shift+F9`), watchpoint (`Shift+F4`), lista de breakpoints y watchpoints, disposición (`F10`) y atajos.
- **Cabecera fija**: programa, include, tipo y nombre del bloque, línea, `SY-SUBRC` y `SY-TABIX`.
- **Código**: siempre en visualización; los métodos se ven por bloques, como en el editor. Doble clic en el número de línea pone o quita un breakpoint; doble clic o `F2` sobre una variable la añade a *Variables*; `F12` salta a la instrucción del cursor.
- **Variables, Locales y Globales**: nombre, valor, tipo técnico, tipo absoluto y valor hexadecimal. Los valores se cambian con el lápiz; las estructuras se despliegan; las tablas internas se ven por páginas, con alta y baja de filas. Todo se puede copiar al portapapeles para pegarlo en una hoja de cálculo.
- **Navegación**: la pila de llamadas (nivel, tipo y evento, programa, include y línea); doble clic para ver otro nivel.
- **Otros breakpoints**: de sentencia ABAP, método (de clase global o local), función, FORM, excepción de clase, mensaje o código fuente, con condición opcional. Se recuerdan y se vuelven a poner en la siguiente ejecución del programa.
- **Watchpoints**: paran cuando cambia una variable, con condición opcional.
- **Disposición de la pantalla configurable**: tú decides cuántas filas y columnas hay y qué frame va en cada celda (Código, Navegación, Variables, Locales, Globales). Las disposiciones se guardan con nombre y valen para todas las ventanas; el tamaño de cada frame se cambia arrastrando las barras que los separan.
- **Atajos de teclado configurables** para todas las acciones, desde el propio panel (botón *Atajos*) o con el ajuste `idea.depuracion.atajos`.

---

## Clases de mensajes (SE91)

Desde «Búsqueda objeto SAP» (tipo *Clase de mensajes*), o navegando con `F2` desde un `MESSAGE`, la clase se abre en una tabla editable. Funciona íntegramente con el ADT estándar, sin necesidad del componente ampliado.

- Se abre en Modo Visualización; *Editar* bloquea la clase y *Guardar* la graba, pidiendo la orden de transporte si hace falta.
- Tabla con número, texto, longitud y marca de autoexplicativo; se filtra por columna y se puede copiar entera al portapapeles.
- Alta y baja de mensajes, con validación al guardar (números de 3 cifras sin repetir, textos obligatorios y longitud máxima).
- Por cada mensaje: ver su **texto explicativo**, ver **dónde se usa** (con salto directo a cada uso) o abrirlo en SE91.
- Con el botón *Nuevo* de «Búsqueda objeto SAP» se crea una clase de mensajes vacía, que se abre en Modo Edición.

---

## Inicio rápido

1. Instala la extensión y recarga VS Code.
2. `Ctrl+Shift+P` → **IDEA: Gestionar conexiones SAP** → da de alta tus sistemas SAP.
3. Elige la conexión activa en la barra de estado (o márcala como *AutoConexión* para que se active sola al abrir VS Code).
4. Conecta tu asistente de IA al servidor MCP de la conexión (ver *Conexión activa y servidores MCP* en la referencia técnica).

Listo: la extensión ya busca, edita, graba y activa contra SAP, y tu asistente de IA ya puede analizar, investigar y proponerte cambios.

> 💡 Cómo obtener la dirección de mi entorno SAP. 
- Abrir la transacción SICF y ejecutarla
- Desplegar el árbol y localizar /default_host/sap/bc/adt
- Usar el menú contextual para ejecutar el comando "Test servicio"
- Se abre el navegador web y la dirección o URL del sistema SAP es el `http(s)://servidor:puerto` que aparece

![Transacción SICF](image.png)

![Dirección o URL del sistema](image-1.png)

---

## Servidor MCP: tu IA, trabajando directamente en SAP

El servidor MCP permite que un asistente de IA consulte el sistema SAP conectado y proponga cambios en el código ABAP. No trabaja sobre copias locales: lee directamente de SAP, y los cambios que propone pasan por el editor de IDEA, con las mismas garantías de bloqueo, orden de transporte y activación que el resto de la extensión.

**Lo que puede hacer la IA:**
- Consultar a qué sistema SAP está conectada.
- Buscar objetos por nombre y leer su código fuente.
- Abrir un objeto en el editor de IDEA.
- Leer el fuente tal como está en el editor (con los cambios aún sin grabar) y la selección.
- Proponer un cambio en el editor, que tú aceptas o rechazas.
- Consultar datos de las tablas de SAP y analizar dumps *(funciones ampliadas)*.

La IA no graba ni activa directamente en SAP: eso lo haces tú desde el editor, cuando das el cambio por bueno.

**Conexión desde tu cliente MCP:** los clientes integrados en VS Code lo detectan solos; en los externos (Claude Code, Cursor…) añade un servidor de tipo `http` apuntando a `http://127.0.0.1:<puerto>/mcp` (puerto configurable en cada conexión, por ejemplo `4856`).

---

## 🔐 Seguridad y control

- IDEA no guarda código fuente en la nube ni en ficheros de tu equipo: todo se lee y se graba directamente contra tu sistema SAP, y el fuente abierto vive solo en la pestaña del editor, que lo descarta al cerrarla.
- Las contraseñas y las claves de API se guardan cifradas en el almacén seguro de VS Code, nunca en texto plano ni en la configuración.
- Los cambios que propone la IA se muestran siempre como diferencias y solo se aplican si los aceptas; aun así, no se graban en SAP hasta que tú grabas.
- El servidor MCP escucha solo en `127.0.0.1` (tu propio equipo).
- Las consultas de datos son solo consultas (`SELECT`): nunca modifican datos de las tablas.
- Si desmarcas «Permite desarrollo» en una conexión, te garantizas que la IA nunca modificará nada en ese sistema: ni objetos ni datos.
- Una misma conexión no puede estar activa en dos ventanas de VS Code a la vez. Y, para no confundir una versión con otra, un mismo objeto no se puede editar a la vez con dos conexiones distintas en la misma ventana (por ejemplo, desarrollo y producción), ni con la misma conexión en dos ventanas. Visualizarlo sí se puede siempre.

---

## Funciones ampliadas (con licencia)

Con un pequeño componente instalado en tu sistema SAP (configurado en `idea.endpointAmpliacionADT`), IDEA desbloquea dentro de VS Code lo que ni el ADT estándar de SAP ofrece:

- **Consultas de datos**: la IA puede consultar las tablas de SAP (solo lectura). Es lo que permite a la IA dar todo su potencial.
- **Dumps de cualquier fecha (ST22)**, no solo los de las últimas 24 horas del ADT estándar, y optimizados para la IA: lista compacta, detalle solo del dump que interesa y datos completos solo si hacen falta, con lo que la IA gasta muchos menos tokens.
- **Crear programas y clases** con su estructura vacía.
- **Descriptores de clases e interfaces**: textos breves de atributos, métodos y parámetros, editables en el propio editor.
- **Elementos de texto (REPT)** de programas, clases e interfaces: edición directa, sin SE38/SE24.
- **Diccionario de datos**: elementos de datos, estructuras, tablas, dominios y tipos tabla, con navegación cruzada entre ellos.
- **GUI Status / Title** de programas: alta, baja y edición visual de funciones, status y barra de herramientas.
- **Dynpros (SE51)**: editor visual de campos y contenedores, con validación al guardar.

Sin este componente configurado, estas acciones siguen disponibles: simplemente abren el objeto en SAP GUI clásico en lugar de en VS Code.

📩 **¿Quieres la licencia completa para tu equipo o consultoría?** Escribe a [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info).

---

## Referencia técnica

<details>
<summary><strong>📋 Comandos y atajos de teclado</strong></summary>

**Atajos del editor de fuente**

Son los atajos por defecto. Todos se pueden cambiar desde el botón *Atajos* del editor (o con el ajuste `idea.editor.atajosWebview`) y, dentro del editor, tienen prioridad sobre los de VS Code. Las acciones sin atajo por defecto (Historial, Modificaciones, Abrir componente, Descriptores, Mensajes) están siempre en la barra de herramientas.

| Acción | Atajo | Descripción |
|---|---|---|
| Modificar / Visualizar | `Ctrl+F1` | Cambia entre Modo Edición (bloquea el objeto en SAP) y Modo Visualización (lo libera). |
| Grabar | `Ctrl+S` | Formatea y graba en SAP. Si el objeto es transportable, pide la orden de transporte **antes** de grabar nada. |
| Verificar | `Ctrl+F2` | Comprueba la sintaxis en SAP del fuente actual, sin grabarlo. |
| Activar | `Ctrl+F3` | Graba si hay cambios y activa el objeto en SAP. |
| Cancelar edición | `Ctrl+Shift+U` | Descarta los cambios sin grabar y vuelve a Modo Visualización. |
| Formatear | `Shift+F1` | Formatea el fuente con el motor configurado. |
| Cerrar el editor | `Ctrl+W` | Cierra la pestaña; si hay cambios sin grabar o sin activar, pide confirmación. |
| Comentar / descomentar | `Ctrl+<` | Comenta o descomenta las líneas seleccionadas con `*` en la columna 1, al estilo SAP. |
| Unir líneas | `Ctrl+Shift+J` | Une varias líneas en una sola sentencia, en las menos líneas posibles. |
| Dividir sentencia | `Ctrl+Shift+K` | Divide una sentencia larga (`SELECT`, `CALL METHOD`, etc.) en varias líneas. |
| Dividir DATA / TYPES | `Ctrl+Shift+D` | Separa las declaraciones encadenadas `DATA:` / `TYPES:` en sentencias individuales. |
| Lista de bloques | `Ctrl+Alt+M` | Lista con filtro para saltar a un METHOD, FORM, MODULE o evento del fuente. |
| Ir al inicio / al fin del bloque | `Ctrl+Shift+↑` / `Ctrl+Shift+↓` | Salta al inicio o al fin del bloque en el que está el cursor. |
| Vista por bloques / fuente completo | `Ctrl+Alt+B` | (Clases) Alterna entre la clase completa y el método actual. |
| Ir a la definición | `F2` | Navega a la definición del objeto bajo el cursor, como en SAP GUI. |
| Volver / ir a la posición siguiente | `Alt+←` / `Alt+→` | Recorre las posiciones visitadas al navegar. |
| Buscar / reemplazar en el editor | `Ctrl+F` / `Ctrl+H` | Búsqueda y reemplazo rápidos del propio editor. |
| Buscar y reemplazar (ventana) | `Ctrl+Shift+F` | Ventana de búsqueda por palabra completa o parcial, en el bloque actual o en todo el fuente, con lista de resultados filtrable y previsualización del reemplazo. |
| Referencias de utilización | `Ctrl+Shift+F3` | Dónde se usa el identificador bajo el cursor. |
| Cerrar mensajes de error | `Ctrl+Q` | Cierra todos los avisos de error que hay a la vista en el editor. |
| Breakpoint en la línea | `F9` | Pone o quita un breakpoint en la línea del cursor. |
| Ejecutar en Web GUI | `Ctrl+F8` | Abre el objeto en Web GUI para ejecutarlo. |
| Maximizar / restaurar | `Ctrl+K Z` | Pasa la pestaña a pantalla completa (modo Zen de VS Code) y la restaura. No configurable. |

Además: autocompletado contra SAP (`Ctrl+Space`) y plegado de código.

**Comandos de VS Code** (`Ctrl+Shift+P`)

| Comando | Descripción |
|---|---|
| `IDEA: Gestionar conexiones SAP` | Añade, edita o elimina los sistemas SAP disponibles. |
| `IDEA: Cambiar Conexión Activa` | Elige contra qué sistema SAP trabaja esta ventana. También con un clic en la conexión de la barra de estado. |
| `IDEA: Cerrar Todas las Conexiones` | Cierra la conexión activa y detiene los servidores MCP de esta ventana. |
| `IDEA: Iniciar Servidor MCP` | Arranca el servidor MCP de una conexión. |
| `IDEA: Detener Servidor MCP` | Detiene un servidor MCP en marcha. |
| `IDEA: Iniciar depuración ABAP` | Deja la conexión activa escuchando las ejecuciones en SAP; cada una que pare en un breakpoint abre su ventana de depuración. |
| `IDEA: Breakpoint en la línea actual` | Pone o quita un breakpoint en la línea del cursor (`F9` en el editor). |
| `IDEA: Detener depuración ABAP` | Quita de SAP los breakpoints puestos, deja de escuchar y cierra las ventanas de depuración. |
| `IDEA: Abrir SAP GUI` | Abre una ventana de SAP GUI clásico contra la conexión que elijas. |
| `IDEA: Guardar la clave de la API de Anthropic` | Guarda, cifrada, la clave para las sugerencias de IA con Claude. |
| `IDEA: Guardar la clave de la API de Gemini` | Guarda, cifrada, la clave para las sugerencias de IA con Gemini. |
| `IDEA: Mostrar README (idioma de VS Code)` | Abre este README en el idioma del editor. |

</details>

<details>
<summary><strong>⚙️ Configuración completa</strong></summary>

Ajustes bajo `idea.*` (Archivo → Preferencias → Configuración, o desde la sección «Configuración» del panel IDEA).

**Formateo (Pretty Printer)**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.prettyprinter.formateadorAUsar` | `extension` (por defecto), `sapConfig` | Motor que formatea al usar *Formatear* y al grabar. `extension`: el formateador propio. `sapConfig`: el Pretty Printer configurado en SAP. |
| `idea.prettyprinter.indentation` | `true` (por defecto), `false` | Activa o no el sangrado automático. |
| `idea.prettyprinter.removeDoubleSpaces` | `true` (por defecto), `false` | Elimina o no los espacios dobles. |
| `idea.prettyprinter.caseSetting` | `upperKeywords` (por defecto), `lowerKeywords`, `upperAll`, `lowerAll` | Mayúsculas/minúsculas: solo palabras clave, o todo el código. |
| `idea.prettyprinter.methodBaseIndent` | `auto` (por defecto), `modoSe24`, `estandar` | Sangría de `METHOD` / `ENDMETHOD` (solo clases). `auto`: respeta los espacios existentes. `modoSe24`: columna 0. `estandar`: un nivel (2 espacios). |
| `idea.prettyprinter.formatScope` | `fullFile` (por defecto), `currentMethodOnly` | Alcance del formateo en clases e interfaces: todo el fuente, o solo el método del cursor (al grabar, solo los métodos modificados). |

**Editor de fuente**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.codeCompletion.insertParameterComments` | `true` (por defecto), `false` | Al insertar la llamada a un método o función con `Ctrl+Space`, incluye el comentario de cada parámetro. Con `false` inserta solo los parámetros. |
| `idea.editor.sugerenciasIa.proveedor` | `desactivado` (por defecto), `vscode`, `anthropic`, `gemini` | Sugerencias de código de IA en línea (texto fantasma; `Tab` las acepta), solo en Modo Edición y tras 500 ms sin escribir. `vscode`: los modelos ya disponibles en VS Code (por ejemplo, Copilot), sin clave propia. `anthropic` y `gemini`: la API correspondiente con tu clave. |
| `idea.editor.sugerenciasIa.modelo` | Nombre del modelo (vacío por defecto) | Modelo de las sugerencias. Con `vscode`, la familia del modelo; con `anthropic` o `gemini`, el identificador del modelo. Vacío: el de por defecto del proveedor. |
| `idea.editor.atajosWebview` | Objeto acción → combinación | Atajos del editor de fuente que difieren de los de por defecto (cadena vacía = sin atajo). Se cambian desde el botón *Atajos* del editor. |

**Conexiones y servidor MCP**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.mcpServer.connections` | Lista de sistemas SAP | Sistemas disponibles. Se edita con «IDEA: Gestionar conexiones SAP». La contraseña **no** se guarda aquí: se pide y se almacena cifrada en el almacén seguro de VS Code. Campos de cada conexión en la tabla siguiente. |
| `idea.mcpServer.config` → `mcpInicial` | Nombre de una conexión (vacío por defecto) | Conexión que queda **activa** al abrir VS Code. Vacío = ninguna. |
| `idea.mcpServer.confirmWrites` | `true` (por defecto), `false` | Pide confirmación (mostrando un diff) antes de que la IA grabe o active directamente en SAP. Hoy esas herramientas no se publican a la IA: sus cambios llegan siempre como propuesta en el editor. |

**Campos de cada conexión**

| Campo | Obligatorio | Qué hace |
|---|---|---|
| Nombre | Sí | Identificador del sistema (p. ej. `DEV`, `QAS`). Es el nombre con el que la IA y la barra de estado se refieren a él. |
| URL | Sí | URL base del sistema SAP (p. ej. `https://miserver.midominio.com:44300`). |
| Mandante | Sí | Mandante SAP (p. ej. `100`). |
| Usuario | Sí | Usuario SAP. |
| Puerto MCP | Sí | Puerto local (`127.0.0.1`) del servidor MCP de esta conexión. Debe ser distinto en cada conexión. |
| Idioma | No | Idioma de logon en SAP. No cambia el idioma de la extensión, que es siempre el de VS Code. |
| Permitir certificados no confiables | No (`false`) | Acepta certificados TLS autofirmados para este sistema. |
| ID del sistema SAP (SID) | No | SID tal como figura en tu SAP Logon. Necesario para abrir SAP GUI clásico. |
| Permite desarrollo | No (`true`) | Si se desmarca, la conexión es de **solo consulta**: la IA solo puede buscar, leer, abrir en Visualización, consultar datos y analizar dumps; no puede proponer cambios ni grabar ni activar. Pensado para sistemas productivos. |
| Arranque silencioso | No (`false`) | Arranca el servidor MCP de esta conexión al abrir VS Code, sin preguntar. Se pueden marcar varias conexiones para tener varios servidores en marcha a la vez. |

**Depurador**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.depuracion.atajos` | Objeto acción → combinación | Atajos de la ventana de depuración que difieren de los de por defecto: `F5` paso a paso, `F6` ejecutar, `F7` retorno, `F8` continuar, `F9` breakpoint, `Shift+F9` otros breakpoints, `Shift+F4` watchpoint, `F2` añadir variable, `F12` saltar a la instrucción, `F10` disposición. También se cambian desde el botón *Atajos* del panel. |

**Funciones ampliadas y SAP GUI**

| Opción | Valores | Qué hace |
|---|---|---|
| `idea.endpointAmpliacionADT` | Ruta del servicio (vacío por defecto), p. ej. `/sap/serviciosazure/` | Habilita las funciones ampliadas (consultas de datos, dumps de cualquier fecha, descriptores, elementos de texto, diccionario, GUI Status/Title, dynpros). Si se deja vacío, esas acciones abren el objeto en SAP GUI. |
| `idea.sapGui.sapshcutPath` | Ruta a `sapshcut.exe` (vacío por defecto) | Solo si SAP GUI no está en una ubicación estándar ni en el PATH. |
| `idea.navigation.gui` | `sapGui` (por defecto), `webGui` | Al navegar a un objeto que la extensión no edita, elige entre SAP GUI clásico (`sapshcut.exe`; necesita el *ID del sistema SAP*) o Web GUI en el navegador. |

</details>

<details>
<summary><strong>🔌 Conexión activa y servidores MCP</strong></summary>

IDEA distingue dos conceptos:

- **Conexión activa**: el sistema SAP contra el que trabaja *esta ventana* de VS Code (búsqueda, edición, activación). Se ve y se cambia desde la barra de estado. Al abrir VS Code se activa la indicada en `mcpInicial`. Una misma conexión no puede estar activa en dos ventanas a la vez. Al cambiar de conexión, IDEA cierra antes todo lo abierto de la anterior (pidiendo confirmación si hay cambios sin grabar).
- **Servidores MCP**: uno por conexión, cada uno en su propio puerto. Pueden estar varios en marcha a la vez, de modo que la IA puede trabajar en DEV y consultar QAS en paralelo.

**Conectar tu cliente MCP:**
- **Clientes integrados en VS Code**: IDEA publica automáticamente el servidor de la conexión activa (`IDEA – <conexión>`); no hay que configurar nada.
- **Clientes externos** (Claude Code, Cursor…): añade un servidor de tipo `http` apuntando a `http://127.0.0.1:<puerto>/mcp`, con el *Puerto MCP* de la conexión. Uno por cada conexión que quieras usar.

**Herramientas MCP disponibles para la IA**

| Herramienta | Qué hace | Solo consulta |
|---|---|:---:|
| `abap_connection_info` | Indica a qué sistema SAP está conectado el servidor. | ✅ |
| `abap_search_object` | Busca objetos por nombre (admite `*` como comodín). | ✅ |
| `abap_read_object_source` | Lee de SAP el código fuente de un objeto. | ✅ |
| `abap_open_object` | Abre un objeto en el editor de fuente de IDEA. | ✅ |
| `abap_editor_get_fuente` | Lee el fuente tal como está en el editor, con los cambios aún sin grabar, y su estado: modo, bloque actual, cursor y selección. | ✅ |
| `abap_editor_get_seleccion` | Lee el texto seleccionado en el editor y su posición. | ✅ |
| `abap_editor_proponer_cambio` | Propone un cambio en el fuente abierto en el editor: el usuario ve las diferencias y lo acepta o lo rechaza. Si lo acepta, se aplica en el editor (se puede deshacer), sin grabar en SAP. | — |
| `abap_editor_esperar_propuesta` | Sigue esperando la decisión del usuario sobre un cambio propuesto cuando la revisión dura más de lo que el cliente MCP permite esperar en una sola llamada. | — |
| `abap_get_datos` | Ejecuta una consulta `SELECT` de solo lectura sobre la base de datos *(función ampliada)*. | ✅ |
| `abap_list_dumps_24h` | Lista los dumps de ejecución de las últimas 24 horas (feed estándar de ADT). | ✅ |
| `abap_list_dumps` | Lista los dumps de ejecución de cualquier fecha (equivalente a ST22), en formato compacto *(función ampliada)*. | ✅ |
| `abap_get_dump_detalle` | Devuelve el detalle de un dump: resumen de ST22 y pila de llamadas; las variables o el dump completo, solo si se piden *(función ampliada)*. | ✅ |

La columna *Solo consulta* indica las herramientas disponibles en conexiones con **Permite desarrollo** desmarcado.

Por seguridad, las herramientas que grababan o activaban directamente en SAP (`abap_write_object_source`, `abap_activate_object` y `abap_llamar_herramienta_desarrollo`) no se publican a la IA: la IA propone, y tú revisas, grabas y activas desde el editor.

</details>

<details>
<summary><strong>🖥️ Panel lateral «IDEA» en detalle</strong></summary>

El icono de IDEA en la barra de actividad abre dos secciones. La búsqueda en el código y el historial de versiones están dentro del propio editor de fuente (botones *Buscar* e *Historial*).

**1. Búsqueda objeto SAP**: busca objetos en el sistema SAP de la conexión activa y los abre en VS Code (requiere el servidor MCP de la conexión en marcha). El nombre admite `*` como comodín.
- **Programa / Report**, **Clase** y **Módulo de función**: se abren en el editor de fuente, en Modo Visualización.
- **Clases**: botones para abrir sus includes locales: `<DEF LOCAL>`, `<IMPL LOCAL>`, `<MACROS>` y `<TEST>` (clases de test ABAP Unit).
- **Grupos de funciones**: muestra su árbol (módulos de función, includes y otras partes) para abrir cada pieza por separado.
- **Elemento de datos**, **Estructura / Tabla**, **Dominio** y **Tipo tabla**: se abren en el editor de diccionario *(función ampliada)*.
- **Botones REPT, CUA y DYNP** (según el tipo de objeto): abren los editores de elementos de texto, GUI Status/Title y dynpros *(funciones ampliadas)*.
- **Clase de mensajes**: se abre en el editor de clases de mensajes (por ADT estándar, sin componente ampliado).
- **Botón Nuevo**: crea un programa, una clase, una clase de mensajes o un objeto de diccionario (elemento de datos, dominio, estructura/tabla, tipo tabla) indicando nombre y paquete. Sin el componente ampliado solo se pueden crear clases de mensajes.
- Si la búsqueda devuelve un único resultado, se abre directamente. Guarda **recientes** e **histórico** de búsquedas.
- Los objetos que la extensión no sabe editar se abren en SAP GUI clásico (o en Web GUI, según `idea.navigation.gui`).

**2. Configuración**: acceso rápido, sin salir del panel, a:
- Conexiones SAP: tabla con *Nombre*, *Arranque silen.* (su servidor MCP arranca al abrir VS Code), *AutoConexión* (la que queda activa al abrir VS Code) y *Desarrollo* (si permite desarrollo); el resto de datos (URL, mandante, usuario, puerto MCP) aparece al pasar el ratón por la fila. Botón *Gestionar conexiones…*.
- Pretty Printer: motor, alcance, indentación, espacios dobles, mayúsculas/minúsculas y sangría de `METHOD`.
- Servidor MCP: conexión inicial y confirmación de escrituras.
- Navegación y SAP GUI: dónde abrir los objetos no editables, ruta de `sapshcut.exe` y servicio de ampliación de ADT.
- Autocompletado y sugerencias de IA: comentarios de parámetros, proveedor, modelo y clave de la API.

**Historial de versiones** (botón *Historial* del editor): guarda una versión del objeto cada vez que se graba o se activa un cambio real, y también cuando detecta que el objeto se ha cambiado directamente en SAP. Es solo de la pestaña: se pierde al cerrarla.
- Tabla con la versión más reciente arriba, la hora del cambio, si se activó, su origen (*Local* o *Cambiado en SAP*) y el nº de cambios respecto a la última activación y a la versión anterior.
- *Ver cambios* entre dos versiones (en línea o lado a lado) y *Ver cambios totales* entre la versión inicial y la actual.
- *Recuperar versión*: vuelca su contenido en el editor, sin grabarlo (se puede deshacer).

</details>

<details>
<summary><strong>🧩 Funciones ampliadas en detalle</strong></summary>

**Consultas de datos.** Permiten a la IA investigar los datos de tu sistema SAP con consultas `SELECT` de solo lectura (sin `INSERT`/`UPDATE`/`DELETE` ni DDL). Sin ellas, la IA ve el código pero no los datos, y pierde buena parte de su capacidad de análisis.

**Editor de elementos de texto (REPT).** Desde el botón *REPT* de «Búsqueda objeto SAP» (o *Abrir componente* en el editor), sobre un programa, clase o interfaz:
- Se abre en Modo Visualización (fondo azul).
- *Editar* bloquea el objeto en SAP (fondo ámbar); al modificar cualquier celda aparece 🔴 en la pestaña.
- *Guardar y activar* sube los textos a SAP (pidiendo orden de transporte si hace falta) y mantiene el bloqueo para seguir editando.
- Al volver a Visualización o cerrar la pestaña se libera el bloqueo.
- *Copiar* lleva toda la tabla de textos al portapapeles.

**Editor de diccionario.** Elementos de datos, estructuras / tablas, dominios y tipos tabla: cabecera, opciones técnicas y lista de campos o valores. Se abre en Visualización; *Editar* bloquea el objeto y permite modificarlo y activarlo con la misma gestión de órdenes de transporte que el resto. La cabecera de la tabla de campos queda fija al hacer scroll; las columnas se pueden ordenar y filtrar. Desde las celdas se navega a otros elementos de datos y dominios.

**GUI Status / Title (CUA).** Alta, baja y edición de títulos, funciones, status y barra de herramientas estándar.

**Dynpros (SE51).** Editor visual de campos y contenedores (marcos, subscreens, tabstrips, table controls): alta situando el elemento con un clic, detección de solapes y validación al guardar.

Todos ellos siguen la misma disciplina de bloqueo, orden de transporte y activación que el resto de objetos.

</details>

---

## Licencia

La extensión es de uso libre bajo licencia MIT.

Si te interesan las funciones ampliadas, que requieren el componente ABAP *ADT Ampliado*, contacta con Marcos Almeida Santolaria en [marcosalmeida@abap.info](mailto:marcosalmeida@abap.info) para conocer condiciones y precios.

---

**Español** · [English](README.en.md) · [Deutsch](README.de.md) · [Français](README.fr.md)
