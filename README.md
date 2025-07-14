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
