github pages
https://leonardo-sj.github.io/MaterialDesingAngular-Ejercicios/
# ComponentePrueba

Este proyecto fue generado usando. [Angular CLI](https://github.com/angular/angular-cli) version 20.0.5.

## Servidor de desarrollo

Para iniciar un servidor de desarrollo local, ejecuta:
```bash
ng serve
```

Una vez que el servidor esté en funcionamiento, abre tu navegador y navega a http://localhost:4200/. La aplicación se recargará automáticamente cada vez que modifiques cualquiera de los archivos fuente.

## Componentes de Angular Material Desing
### Auto complete
El Autocompletar de Angular Material es un componente de entrada de texto que te ayuda a sugerir y autocompletar valores a medida que el usuario escribe. Es ideal para mejorar la experiencia de usuario en formularios, búsquedas y cualquier campo donde el usuario necesite seleccionar una opción de una lista extensa.

**¿Cómo funciona?**

Cuando el usuario comienza a escribir en el campo de entrada, el componente de autocompletar muestra un panel de opciones sugeridas que coinciden con el texto ingresado. El usuario puede entonces:

Seleccionar una opción del panel, lo que llenará el campo de entrada con el valor completo.

Continuar escribiendo si ninguna de las sugerencias es la que busca.

**Características clave:**

Filtrado de datos: Te permite filtrar dinámicamente una lista de opciones (por ejemplo, nombres de países, contactos, productos) basándose en la entrada del usuario.

Entrada de texto flexible: El campo de entrada es un <input> HTML estándar, lo que facilita su integración con formularios reactivos de Angular.

Asociación con mat-option: El panel de sugerencias se construye utilizando elementos mat-option, que son los mismos elementos de opción utilizados en los componentes mat-select (selección desplegable) y mat-autocomplete.

Configuración personalizable: Puedes controlar el comportamiento del panel, como cuándo se abre, cómo se filtran los resultados y qué se muestra en la lista de sugerencias.

Accesibilidad: Cumple con los estándares de accesibilidad para entradas de texto con sugerencias.

**¿Cuándo usarlo?**

Es una excelente opción para situaciones donde:

Necesitas una entrada de texto libre pero con la ayuda de sugerencias.

La lista de opciones puede ser muy larga, haciendo que un mat-select tradicional sea impráctico.

Quieres guiar al usuario hacia entradas válidas.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0de5b295-3fb6-4857-9868-ee805c79c94e" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/819df1a2-e2e5-4589-825c-6ffc1b94afa6" />

### Badge
---
El componente **Badge (Insignia)** de Angular Material es un pequeño indicador numérico o de texto que se adjunta a otros elementos, como iconos, botones o texto, para mostrar una notificación, un conteo o un estado. Es útil para captar la atención del usuario sin interrumpir su flujo de trabajo principal.

---
### ¿Qué es y para qué sirve?

Una insignia es como una etiqueta o "globo" informativo que se superpone a otro elemento de la interfaz de usuario. Su propósito principal es:

* **Mostrar conteos:** Por ejemplo, el número de mensajes no leídos en un icono de bandeja de entrada, el número de artículos en un carrito de compras, o la cantidad de notificaciones.
* **Indicar un estado:** Podría ser un punto rojo para señalar que hay una nueva actualización, o un "Nuevo" para un elemento recién añadido.
* **Destacar elementos:** Llamar la atención sobre un elemento específico en la interfaz.

---
### Características clave:

* **Adjunto a cualquier elemento:** Puedes aplicar una insignia a casi cualquier elemento HTML o componente de Angular Material.
* **Contenido configurable:** La insignia puede contener un número, texto o simplemente ser un punto (punto de notificación).
* **Posicionamiento flexible:** Puedes controlar la posición de la insignia relativa al elemento al que está adjunta (superior-derecha, superior-izquierda, etc.).
* **Tamaño personalizable:** Permite ajustar el tamaño de la insignia para que se adapte mejor a tus necesidades visuales.
* **Estilos y colores:** Soporta los colores de la paleta de Angular Material (primary, accent, warn) y otras opciones de estilo.
* **Interactividad (opcional):** Aunque la insignia en sí no es interactiva, a menudo se usa con elementos que sí lo son, como botones o iconos que, al hacer clic, ocultan o actualizan la insignia.

---
### ¿Cuándo usarlo?

Usa el componente Badge cuando necesites:

* **Alertar al usuario** sobre una cantidad o un cambio sin ser intrusivo.
* Mantener una **interfaz limpia** mientras proporcionas información contextual importante.
* Mejorar la **experiencia de usuario** guiando la atención a elementos relevantes que requieren acción o visualización.

El Badge de Angular Material es un pequeño pero efectivo componente para agregar información visual concisa y contextual a tu aplicación.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/5436a432-2491-4867-9114-09f3c9834d11" />

### Bottom Sheet
La **Hoja Inferior (Bottom Sheet)** de Angular Material es un componente que abre paneles estilo Material Design en la parte inferior de la pantalla. Están diseñadas principalmente para **dispositivos móviles** como una alternativa a los diálogos y menús tradicionales.

### ¿Cómo funciona?

Se utiliza el servicio `MatBottomSheet` para abrir estos paneles. Puedes abrir una hoja inferior llamando al método `open()`, al que le pasas un componente que se cargará dentro del panel y, opcionalmente, un objeto de configuración.

El método `open()` devuelve una instancia de `MatBottomSheetRef`, que te permite controlar la hoja inferior, como cerrarla o suscribirte a eventos. Es importante saber que **solo se puede abrir una hoja inferior a la vez**.

### Características clave:

* **Paso de datos:** Puedes enviar datos al componente que se carga en la hoja inferior utilizando la propiedad `data` en el objeto de configuración. Estos datos se pueden acceder dentro del componente de la hoja inferior mediante el token de inyección `MAT_BOTTOM_SHEET_DATA`.
* **Opciones por defecto:** Puedes configurar opciones predeterminadas para todas las hojas inferiores de tu aplicación de manera global usando `MAT_BOTTOM_SHEET_DEFAULT_OPTIONS`.
* **Accesibilidad:** Este componente implementa el patrón ARIA `role="dialog"`, lo que asegura su accesibilidad. Incluye interacción con el teclado (la tecla 'Escape' la cierra por defecto) y gestión del foco para una mejor experiencia de usuario.

### ¿Cuándo usarlo?

La Hoja Inferior es ideal para:

* Ofrecer una lista de acciones o de opciones de selección en un contexto que no requiere un diálogo completo.
* Presentar información adicional o controles sin cubrir toda la pantalla, especialmente en dispositivos móviles.

Es una herramienta útil para ofrecer interacciones contextuales y de fácil acceso, optimizadas para experiencias táctiles.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/dc96aed0-8ae9-4322-84a4-0cc37caaddd8" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/76a65518-0fef-436b-93d3-9c540ee264ee" />

### Button
El componente **Button (Botón)** de Angular Material es un elemento interactivo esencial que permite a los usuarios realizar acciones y enviar información en tu aplicación. Proporciona una variedad de estilos y funcionalidades predefinidas que siguen las directrices de Material Design.

---
### ¿Qué es y para qué sirve?

Los botones son la base de la interacción del usuario en una aplicación. Con el componente `mat-button` (o sus variantes), puedes crear botones con diferentes apariencias y comportamientos, como:

* **Acciones primarias:** Iniciar un proceso, enviar un formulario, guardar datos.
* **Acciones secundarias:** Cancelar una operación, borrar un campo.
* **Navegación:** Ir a otra página o sección de la aplicación.
* **Botones con iconos:** Combinar texto con iconos para una mejor comprensión visual.

---
### Tipos de botones:

Angular Material ofrece varios tipos de botones, cada uno con un propósito y estilo visual distintos:

* **`mat-button` (Botón de texto/plano):** Un botón minimalista, ideal para acciones de baja prominencia o para usar dentro de menús y diálogos. No tiene elevación.
* **`mat-raised-button` (Botón elevado):** El tipo de botón más común, con una sombra que le da una apariencia "elevada". Se usa para acciones principales que deben destacarse.
* **`mat-flat-button` (Botón plano con relleno):** Similar al botón elevado, pero con una sombra más sutil y un fondo plano. Ofrece un punto intermedio entre el botón de texto y el elevado.
* **`mat-stroked-button` (Botón con borde):** Tiene un borde alrededor del texto y un fondo transparente. Útil para acciones secundarias que necesitan ser más visibles que un botón de texto, pero menos que uno elevado.
* **`mat-icon-button` (Botón de icono):** Diseñado específicamente para contener un icono de Material Design. Es un botón circular sin texto, perfecto para acciones como "eliminar", "editar" o "mostrar/ocultar".
* **`mat-fab` (Floating Action Button):** Un botón de acción flotante circular grande, que se coloca prominentemente para la acción principal de una pantalla.
* **`mat-mini-fab` (Mini Floating Action Button):** Una versión más pequeña del `mat-fab`, ideal para acciones relacionadas o contextuales.

---
### Características clave:

* **Colores temáticos:** Puedes aplicar los colores definidos en tu tema de Angular Material (`primary`, `accent`, `warn`) a los botones para mantener la coherencia visual.
* **Deshabilitar botones:** Los botones pueden deshabilitarse fácilmente usando la propiedad `[disabled]="true"`, lo que les da una apariencia atenuada y evita interacciones.
* **Integración con iconos:** Se integran perfectamente con el componente `mat-icon` para crear botones con íconos significativos.
* **Accesibilidad:** Los botones de Angular Material están construidos pensando en la accesibilidad, asegurando que sean navegables y utilizables por personas con diversas necesidades.

En resumen, el componente Button de Angular Material te brinda la flexibilidad y las herramientas para implementar interacciones de usuario claras y estéticamente agradables en tu aplicación, siguiendo los principios de Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/11224134-0e42-4ea3-b9d1-9bc01940bd3d" />

### Button toggle

El componente **Button Toggle (Botón de Alternancia)** de Angular Material es un grupo de botones que actúan como interruptores de encendido/apagado, permitiendo al usuario seleccionar una o varias opciones de un conjunto. Es similar a los botones de radio o casillas de verificación, pero con una apariencia de botón.

---
### ¿Qué es y para qué sirve?

El botón de alternancia se usa para cambiar el estado o la configuración de algo. Puede funcionar de dos maneras principales:

1.  **Selección exclusiva (como botones de radio):** Donde solo se puede seleccionar uno de los botones del grupo a la vez. Al seleccionar un botón, cualquier otro botón previamente seleccionado se deselecciona automáticamente.
2.  **Selección múltiple (como casillas de verificación):** Donde se pueden seleccionar varios botones dentro del grupo simultáneamente.

Es ideal para interfaces donde quieres que las opciones se vean claramente como botones interactivos, en lugar de los elementos de formulario más tradicionales.

---
### Características clave:

* **Grupo de botones (`mat-button-toggle-group`):** Los botones individuales (`mat-button-toggle`) siempre se agrupan dentro de un contenedor `mat-button-toggle-group` para gestionar su comportamiento.
* **Selección exclusiva o múltiple:** Controla el comportamiento del grupo usando la propiedad `[multiple]="true"` en `mat-button-toggle-group` para permitir múltiples selecciones. Por defecto, es de selección exclusiva.
* **Enlaces a formularios de Angular:** Se integra sin problemas con los formularios reactivos y de plantilla de Angular, lo que permite manejar fácilmente el estado y los valores seleccionados.
* **Valor (`value`):** Cada `mat-button-toggle` tiene un atributo `value` que representa la opción que selecciona.
* **Iconos y texto:** Los botones pueden contener texto, iconos o ambos, lo que los hace muy versátiles visualmente.
* **Accesibilidad:** Los grupos de botones de alternancia de Angular Material están diseñados con accesibilidad en mente, asegurando una navegación y uso adecuados para todos los usuarios.

---
### ¿Cuándo usarlo?

Utiliza el componente Button Toggle cuando:

* Necesites un conjunto de opciones donde la apariencia de **botón sea más apropiada** que una casilla de verificación o un botón de radio.
* Quieras alternar entre **estados predefinidos** (por ejemplo, "Activo" / "Inactivo", "Día" / "Semana" / "Mes").
* Desees que la **interacción sea muy visual** y clara para el usuario.

El Button Toggle de Angular Material ofrece una forma flexible y visualmente atractiva de permitir a los usuarios hacer selecciones o alternar estados dentro de tu aplicación, manteniendo la estética de Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9c29c631-277e-46e8-9776-e50a890abb0c" />
### Card

La **Tarjeta (Card)** de Angular Material es un componente versátil y flexible que se usa para agrupar contenido y acciones relacionadas de una manera visualmente atractiva y fácil de digerir. Imagina que es como un "contenedor de información" que puedes usar para mostrar un producto, un usuario, una publicación de blog o cualquier pieza de contenido que necesite su propio espacio delimitado en la interfaz.

---
### ¿Qué es y para qué sirve?

El componente `mat-card` sigue las directrices de Material Design y es ideal para:

* **Mostrar información de forma modular:** Permite presentar bloques de contenido de manera independiente, facilitando que el usuario escanee y comprenda la información.
* **Agrupar elementos relacionados:** Puedes combinar imágenes, texto, enlaces y botones dentro de una tarjeta, manteniendo la cohesión visual de la información.
* **Crear diseños de tipo "revista" o "noticias":** Son perfectas para cuadrículas de contenido donde cada tarjeta representa un elemento distinto.

---
### Estructura de una tarjeta:

Una tarjeta de Angular Material se compone de varias secciones opcionales que te permiten estructurar el contenido de manera lógica:

* **`mat-card-header`**: El encabezado de la tarjeta, que a menudo incluye un avatar (`mat-card-avatar`), un título (`mat-card-title`) y un subtítulo (`mat-card-subtitle`).
* **`mat-card-title`**: El título principal de la tarjeta.
* **`mat-card-subtitle`**: Un subtítulo para complementar el título.
* **`mat-card-content`**: La sección principal para el contenido de texto, párrafos o cualquier otro elemento.
* **`mat-card-actions`**: Un contenedor para botones de acción o enlaces relacionados con el contenido de la tarjeta, generalmente ubicados en la parte inferior.
* **`mat-card-image`**: Una imagen que se coloca dentro de la tarjeta, típicamente para resaltar el contenido visualmente.

---
### Características clave:

* **Diseño adaptable:** Las tarjetas son inherentemente responsivas y se adaptan bien a diferentes tamaños de pantalla, lo que las hace adecuadas para diseños móviles y de escritorio.
* **Sombra y elevación:** Las tarjetas suelen tener una sombra que les da una sensación de elevación en la interfaz, siguiendo el principio de Material Design del "papel" digital.
* **Flexibilidad de contenido:** Puedes poner prácticamente cualquier elemento HTML o componente Angular dentro de las diferentes secciones de una tarjeta.
* **Fácil uso:** Su API es sencilla y se integra bien con el resto de los componentes de Angular Material.

El componente Card es un pilar fundamental en el diseño de interfaces con Material Design, ofreciéndote una forma estructurada y visualmente atractiva de presentar información modular y coherente a tus usuarios.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/bb8791aa-547c-4d86-94d0-181046fd785e" />

### Checkbox
La **Casilla de Verificación (Checkbox)** de Angular Material es un control de interfaz de usuario que permite al usuario **seleccionar o deseleccionar una opción individual**. Es un tipo de entrada booleana: la opción está "activada" (seleccionada) o "desactivada" (deseleccionada).

---
### ¿Qué es y para qué sirve?

El componente `mat-checkbox` se utiliza para situaciones donde el usuario puede activar o desactivar una característica, una preferencia o un elemento de una lista de forma independiente. A diferencia de los botones de radio, donde solo puedes elegir una opción de un grupo, las casillas de verificación te permiten:

* **Seleccionar múltiples opciones** de una lista (si cada opción tiene su propia casilla).
* **Activar o desactivar una única característica**.

---
### Características clave:

* **Estado booleano:** Representa un valor verdadero/falso (true/false) o sí/no.
* **Estado indeterminado:** Además de "seleccionado" y "deseleccionado", una casilla de verificación puede tener un estado "indeterminado". Esto es útil cuando una casilla "maestra" representa un grupo de sub-casillas: si algunas sub-casillas están seleccionadas y otras no, la casilla maestra puede mostrar un estado indeterminado para indicar que no todas las sub-casillas están ni completamente seleccionadas ni completamente deseleccionadas.
* **Etiqueta personalizable:** Puedes colocar texto (o incluso otros elementos HTML) al lado de la casilla para describir la opción. La casilla se puede configurar para que la etiqueta aparezca antes o después del cuadro.
* **Enlaces a formularios de Angular:** Se integra sin problemas con los formularios reactivos y de plantilla de Angular, lo que facilita la gestión de su estado y valor.
* **Colores temáticos:** Soporta los colores de la paleta de Angular Material (`primary`, `accent`, `warn`).
* **Deshabilitar casillas:** Puedes deshabilitar una casilla de verificación para evitar la interacción del usuario, lo que la hace aparecer atenuada.
* **Accesibilidad:** El componente está construido con la accesibilidad en mente, asegurando que se pueda navegar y usar correctamente con tecnologías de asistencia.

---
### ¿Cuándo usarlo?

Usa el componente Checkbox cuando necesites:

* Permitir que el usuario **seleccione múltiples ítems** de una lista.
* Ofrecer una opción para **activar o desactivar una configuración** específica.
* Implementar una casilla **"seleccionar todo"** que tenga un estado indeterminado cuando solo algunos elementos están seleccionados.

La casilla de verificación de Angular Material es un control fundamental para recolectar entradas booleanas o de selección múltiple, manteniendo la coherencia visual y funcional de Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/783f77be-2547-4564-9e4d-001b6c452086" />

### Chips
El componente **Chips (Fichas o Píldoras)** de Angular Material son elementos compactos y interactivos que representan una pieza de información compleja, un atributo, una entidad o una acción. Son como "etiquetas" que puedes usar para mostrar selecciones, filtrar contenido, ingresar entradas o activar acciones.

---
### ¿Qué son y para qué sirven?

Los Chips son altamente versátiles y se utilizan en una variedad de escenarios:

* **Chips de Entrada (Input Chips):** Permiten al usuario ingresar información en un campo, como direcciones de correo electrónico o etiquetas. A medida que el usuario escribe, las entradas se convierten en chips, que a menudo pueden ser removidos.
* **Chips de Elección (Choice Chips):** Son grupos de chips que permiten una selección única (como botones de radio, pero con apariencia de chip) de un conjunto de opciones.
* **Chips de Filtro (Filter Chips):** Permiten seleccionar múltiples opciones de un conjunto (como casillas de verificación) para filtrar contenido. Cada chip representa un filtro activo.
* **Chips de Acción (Action Chips):** Realizan una acción cuando se hace clic en ellos. Son como botones pequeños que contienen una etiqueta y opcionalmente un icono.

---
### Características clave:

* **Contenido conciso:** Muestran información de forma breve y clara, a menudo con un icono o avatar.
* **Interactividad:** Pueden ser seleccionables, deseleccionables, removibles o ejecutables (como un botón).
* **Grupos de Chips (`mat-chip-listbox`, `mat-chip-grid`):** Los chips a menudo se organizan en grupos para gestionar la selección, la navegación o el diseño.
    * `mat-chip-listbox`: Utilizado para chips de elección o filtro, gestiona la selección de uno o varios chips.
    * `mat-chip-grid`: Organiza los chips en una cuadrícula, útil para entrada de chips donde el usuario puede añadir o quitar elementos.
* **Removibles:** Muchos chips tienen un botón de "remover" (usualmente una 'x') que permite al usuario eliminarlos de la interfaz.
* **Accesibilidad:** Proporcionan un soporte de accesibilidad robusto, incluyendo navegación por teclado y etiquetas ARIA apropiadas.
* **Personalización:** Puedes personalizar su apariencia, incluyendo colores, iconos y el texto que muestran.

---
### ¿Cuándo usarlo?

Usa el componente Chips cuando necesites:

* **Visualizar etiquetas o categorías:** Por ejemplo, en un sistema de etiquetado de contenido.
* **Permitir selección múltiple o única de filtros:** Como filtros en una página de comercio electrónico.
* **Gestionar entradas de usuario:** Donde el usuario puede añadir múltiples elementos (ej. correos electrónicos, habilidades).
* **Representar entidades:** Como nombres de personas o temas en un hilo de conversación.

Los Chips de Angular Material son una solución elegante y eficiente para manejar y visualizar información discreta y acciones relacionadas de manera interactiva, siguiendo las pautas de Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3683ed4a-dccb-4042-a772-f95d66674f4e" />

### Datepicker
El componente **Datepicker (Selector de Fecha)** de Angular Material es un campo de entrada de texto que, al ser enfocado o al hacer clic en un icono, abre un calendario interactivo. Este calendario permite a los usuarios seleccionar una fecha de manera sencilla y visual.

---
### ¿Qué es y para qué sirve?

El `mat-datepicker` se utiliza para:

* **Ingresar fechas:** Proporciona una interfaz intuitiva para que los usuarios elijan una fecha específica, como una fecha de nacimiento, una fecha de reserva o una fecha de evento.
* **Validación de fechas:** Puede configurarse para restringir el rango de fechas seleccionables, por ejemplo, permitiendo solo fechas futuras o fechas dentro de un período específico.
* **Mejorar la experiencia de usuario:** Ofrece una alternativa más amigable y menos propensa a errores que escribir manualmente una fecha en un formato específico.

---
### Características clave:

* **Integración con campos de entrada:** Funciona con el componente `matInput` (o un `input` HTML estándar) para mostrar la fecha seleccionada.
* **Selector de calendario emergente:** El corazón del componente es el calendario que aparece al hacer clic o enfocar el campo de entrada.
* **Rango de fechas:** Puedes definir fechas mínimas (`min`) y máximas (`max`) para limitar las selecciones del usuario.
* **Filtrado de fechas:** Permite deshabilitar fechas específicas (por ejemplo, fines de semana o días festivos) utilizando una función de filtro.
* **Diferentes modos de vista:** El calendario puede mostrar vistas de día, mes o año, permitiendo una navegación rápida.
* **Soporte de localización (i18n):** Es personalizable para diferentes formatos de fecha, nombres de días/meses y la fecha de inicio de la semana, lo que lo hace adaptable a diversas culturas.
* **Integración con formularios:** Se integra perfectamente con los **formularios reactivos** y de **plantilla** de Angular, facilitando la recolección y validación de datos de fecha.
* **Accesibilidad:** El componente está diseñado pensando en la accesibilidad, permitiendo la navegación por teclado y el uso con lectores de pantalla.

---
### ¿Cuándo usarlo?

Usa el componente Datepicker cuando necesites:

* Recopilar **fechas de eventos, cumpleaños, plazos**, etc.
* Implementar **filtros de búsqueda basados en fechas**.
* Restringir la selección de fechas a **rangos específicos**.

El Datepicker de Angular Material es una herramienta robusta y fácil de usar para manejar la entrada de fechas en tu aplicación, ofreciendo una experiencia de usuario consistente con Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/c6a3a691-c082-4896-b173-2df46fe4f9fc" />

### Dialog
El componente **Dialog (Diálogo)** de Angular Material es una ventana flotante modal que aparece sobre el contenido principal de la aplicación, bloqueando la interacción con el fondo hasta que se realiza una acción o se cierra. Es ideal para situaciones donde necesitas que el usuario se enfoque en una tarea específica o confirme una decisión.

---
### ¿Qué es y para qué sirve?

El componente `MatDialog` se utiliza para crear ventanas modales para diversos propósitos:

* **Alertas o confirmaciones:** Preguntar al usuario si está seguro de realizar una acción (por ejemplo, "Confirmar eliminación").
* **Formularios temporales:** Mostrar un formulario pequeño para capturar información adicional sin redirigir al usuario (por ejemplo, "Editar perfil").
* **Información adicional:** Presentar detalles sobre un elemento sin salir de la vista actual (por ejemplo, "Ver detalles del producto").
* **Mensajes de error o éxito:** Notificar al usuario sobre el resultado de una operación.

---
### ¿Cómo funciona?

Los diálogos se abren utilizando el servicio `MatDialog`. Le pasas el **componente de Angular que quieres que se cargue dentro del diálogo** y, opcionalmente, un objeto de configuración.

* El método `open()` devuelve una instancia de `MatDialogRef`, que es una referencia al diálogo abierto. Esta referencia te permite controlar el diálogo, como cerrarlo y pasar datos, o suscribirte a eventos cuando el diálogo se cierra.
* **Modales:** Por defecto, los diálogos son modales, lo que significa que el usuario no puede interactuar con el contenido detrás del diálogo hasta que este se cierra.
* **Paso de datos:** Puedes pasar datos al componente del diálogo a través de la propiedad `data` en el objeto de configuración. Dentro del componente del diálogo, se accede a estos datos mediante el token de inyección `MAT_DIALOG_DATA`.
* **Resultados al cerrar:** Cuando el diálogo se cierra, puedes pasar un valor de retorno, que el componente que abrió el diálogo puede recibir para reaccionar a la acción del usuario.

---
### Características clave:

* **Flexibilidad de contenido:** Puedes poner cualquier componente de Angular dentro de un diálogo, lo que te da total control sobre su contenido y funcionalidad.
* **Configuración personalizable:** Ofrece muchas opciones para controlar el comportamiento del diálogo: tamaño (ancho, alto), posición, si se puede cerrar haciendo clic fuera, si se puede cerrar con la tecla Escape, etc.
* **Animaciones:** Los diálogos incluyen animaciones predefinidas para una transición suave al abrirse y cerrarse.
* **Accesibilidad:** El componente está construido con un enfoque en la accesibilidad, asegurando que sean navegables por teclado y compatibles con lectores de pantalla.

En resumen, el componente Dialog de Angular Material es una herramienta poderosa y flexible para crear interacciones modales en tu aplicación, permitiéndote controlar el flujo de usuario y la presentación de información importante de manera efectiva y coherente con Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/feb2cd51-4c9b-45b9-a5b5-c949821db1b6" />

### Divider
El componente **Divider (Divisor)** de Angular Material es una línea fina que se utiliza para **separar visualmente el contenido** en una lista o en una sección de la interfaz de usuario. Su propósito principal es mejorar la legibilidad y la organización del diseño, creando una clara distinción entre diferentes grupos de elementos.

---
### ¿Qué es y para qué sirve?

El componente `mat-divider` es una herramienta de diseño sencilla pero efectiva para:

* **Organizar listas:** Es común usarlo en listas (como `mat-list` o `mat-menu`) para separar elementos individuales o grupos de elementos, como opciones de menú, contactos o elementos de configuración.
* **Segmentar secciones:** Puedes usarlo en cualquier parte de tu UI para crear una separación visual entre bloques de contenido, por ejemplo, entre diferentes secciones de un formulario o entre un encabezado y el contenido principal.
* **Mejorar la legibilidad:** Al dividir el contenido en bloques manejables, ayuda al usuario a escanear la página más fácilmente y a comprender la estructura de la información.

---
### Características clave:

* **Orientación:** Por defecto, los divisores son **horizontales**. Puedes hacerlos **verticales** agregando la propiedad `[vertical]="true"`. Esto es útil para separar elementos uno al lado del otro.
* **Divisores insertados (Inset Dividers):** Los divisores horizontales pueden ser "insertados" (sangrados) usando la propiedad `[inset]="true"`. Esto significa que la línea no se extiende por todo el ancho del contenedor, dejando un pequeño margen al principio. Esto es común en listas de avatares donde la línea no debe pasar por debajo del avatar.
* **Ligero y simple:** Es un componente muy ligero que solo se encarga de la presentación visual de una línea divisoria, sin añadir complejidad de interactividad.
* **Estilo Material Design:** Sigue las pautas de diseño de Material Design para asegurar una apariencia y sensación consistentes con el resto de tu aplicación.

---
### ¿Cuándo usarlo?

Usa el componente Divider cuando necesites:

* Separar elementos en una **lista de opciones o configuraciones**.
* Delimitar **secciones lógicas** dentro de un panel o un formulario.
* Mejorar la **jerarquía visual** y la organización de tu interfaz de usuario.

El Divider de Angular Material es un componente discreto pero fundamental para construir interfaces de usuario limpias, organizadas y fáciles de navegar, adhiriéndose a los principios de Material Design.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e902cafb-4d60-4e51-a40c-25dd8dfefe1c" />

### Expansion panel
El componente **Expansion Panel (Panel de Expansión)** de Angular Material es un contenedor que puede ser **contraído o expandido** para mostrar u ocultar contenido. Es una excelente manera de organizar grandes cantidades de información, permitiendo a los usuarios ver solo lo que necesitan en un momento dado, mejorando así la usabilidad y el orden en la interfaz.

---
### ¿Qué es y para qué sirve?

El `mat-expansion-panel` se utiliza para:

* **Organizar información jerárquica:** Ideal para preguntas frecuentes (FAQ), detalles de un producto, pasos de un proceso (como un _stepper_ no lineal) o cualquier contenido que pueda agruparse en secciones colapsables.
* **Ahorrar espacio:** Mantiene la interfaz limpia y concisa al ocultar contenido menos relevante hasta que el usuario decida verlo.
* **Mejorar la navegación:** Permite a los usuarios expandir solo las secciones que les interesan, reduciendo el _scroll_ excesivo.

---
### Estructura y comportamiento:

Un panel de expansión generalmente consta de dos partes principales:

1.  **Encabezado (`mat-expansion-panel-header`):** Siempre visible, este es el área en la que el usuario hace clic para alternar el estado del panel (expandir/contraer). Puede contener:
    * **`mat-panel-title`:** El título principal del panel.
    * **`mat-panel-description`:** Una descripción o resumen más pequeño.
2.  **Contenido:** El área que se oculta o se muestra cuando el panel se expande.

Puedes agrupar múltiples paneles de expansión dentro de un **Acordeón (`mat-accordion`)**. En un acordeón, puedes configurar que:

* **Solo un panel** se pueda expandir a la vez (comportamiento predeterminado, como un acordeón musical). Al expandir uno, los demás se contraen.
* **Múltiples paneles** se puedan expandir simultáneamente.

---
### Características clave:

* **Control de expansión programático:** Puedes expandir o contraer un panel desde tu código TypeScript, además de la interacción del usuario.
* **Estado abierto/cerrado:** Los paneles tienen un estado `[expanded]` que puedes vincular a tus datos.
* **Eventos de cambio:** Emite eventos cuando el panel comienza a expandirse (`(opened)`) o a contraerse (`(closed)`), o cuando su estado de expansión cambia (`(afterExpand)`, `(afterCollapse)`).
* **Deshabilitar paneles:** Puedes deshabilitar un panel para evitar que el usuario lo expanda o contraiga.
* **Accesibilidad:** Compatible con la navegación por teclado y tecnologías de asistencia, siguiendo las directrices de ARIA.
* **Personalización:** Permite personalizar los iconos del encabezado y el estilo general para adaptarse a tu diseño.

El componente Expansion Panel de Angular Material es una forma efectiva y elegante de gestionar la presentación de información segmentada, haciendo que tus interfaces sean más organizadas y fáciles de usar, especialmente cuando manejas mucho contenido.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e42f17c6-3681-4939-9e82-4b5f5d3144f2" />

### Form field
El componente **Form Field (Campo de Formulario)** de Angular Material es un contenedor que envuelve controles de entrada comunes de Material Design como `input`, `textarea`, `select` y `datepicker`, aplicándoles estilos consistentes, etiquetas flotantes, mensajes de error y sugerencias.
-----

### ¿Qué es y para qué sirve?

El `mat-form-field` no es un control de entrada en sí mismo, sino un **contenedor visual y funcional** para ellos. Su propósito principal es:

  * **Aplicar estilos uniformes:** Asegura que todos tus campos de entrada tengan la misma apariencia de Material Design.
  * **Manejar la etiqueta (label):** Permite que la etiqueta del campo flote elegantemente cuando el usuario empieza a escribir o cuando el campo está enfocado.
  * **Mostrar mensajes de error:** Proporciona un espacio estandarizado para mostrar errores de validación.
  * **Ofrecer mensajes de sugerencia:** Permite añadir texto de ayuda o sugerencias debajo del campo.
  * **Iconos y prefijos/sufijos:** Facilita la adición de iconos (como `mat-icon`) o texto fijo antes (prefijo) o después (sufijo) del campo de entrada.

-----

### Características clave:

  * **Tipos de apariencia (Appearance):** Puedes elegir entre diferentes estilos visuales para el campo de formulario, como `fill` (relleno), `outline` (contorno), `standard` (estándar) y `legacy` (legado), para que se adapten a tu diseño.
  * **Etiquetas flotantes:** Las etiquetas (`mat-label`) se animan y "flotan" sobre el campo cuando este está enfocado o contiene texto, mejorando la usabilidad.
  * **Mensajes de error y de ayuda:** Los elementos `mat-error` y `mat-hint` proporcionan retroalimentación al usuario. Angular Material se encarga de mostrar los errores automáticamente cuando el control de formulario es inválido y ha sido "tocado" (interactuado por el usuario).
  * **Prefijos y sufijos:** Puedes añadir iconos o texto fijo al principio (`matPrefix`) o al final (`matSuffix`) del campo de entrada, útil para unidades de medida o iconos de visibilidad de contraseña.
  * **Encapsulación:** El contenedor gestiona el foco y la interacción entre sus elementos internos, simplificando la creación de formularios consistentes.
  * **Integración con formularios de Angular:** Se integra de forma nativa con los **Formularios Reactivos** y los **Formularios de Plantilla** de Angular.
  * **Accesibilidad:** Proporciona atributos ARIA y un manejo de foco robusto para garantizar que los formularios sean accesibles.

El componente Form Field es esencial en Angular Material para construir formularios con una apariencia consistente y una experiencia de usuario mejorada, agrupando los controles de entrada con sus etiquetas, errores y sugerencias de manera estándar y limpia.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fbe32700-5b42-4bfe-81b2-e99a0e183c08" />

### Icon
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e8620972-94b5-4ac6-8bce-aa8d12697c56" />

### Input
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/83bc245b-813e-405d-9dda-082c8b70791e" />

### Table
## Andamiaje de código (Code scaffolding)

Angular CLI incluye potentes herramientas de andamiaje de código. Para generar un nuevo componente, ejecuta:

```bash
ng generate component component-name
```

Para una lista completa de los esquemas disponibles (como components, directives o pipes), ejecuta:
```bash
ng generate --help
```

## Construcción (Building)

To build the project run:

```bash
ng build
```

This will compile your project and store the build artifacts in the `dist/` directory. By default, the production build optimizes your application for performance and speed.

## Running unit tests

To execute unit tests with the [Karma](https://karma-runner.github.io) test runner, use the following command:

```bash
ng test
```

## Running end-to-end tests

For end-to-end (e2e) testing, run:

```bash
ng e2e
```

Angular CLI does not come with an end-to-end testing framework by default. You can choose one that suits your needs.

## Additional Resources

For more information on using the Angular CLI, including detailed command references, visit the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.
=======
# MaterialDesigAngular-Ejercicios
Algunos Material Desing de Angular explicados
>>>>>>> 85d8fdf8c7e8ece90bfa6598abb001752a1e424d
