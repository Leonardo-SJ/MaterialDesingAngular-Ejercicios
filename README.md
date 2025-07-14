<<<<<<< HEAD
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
