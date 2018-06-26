# Contenido
### 1. Para empezar

Los archivos que necesitas descargar, como abrirlos, etc. 

### 2. Explicación sobre HTML y CSS

Un poco de información sobre los lenguajes con los que trabajaremos hoy.

### 3. Tus tareas

Personalizar la plantilla web proporcionada con tus propias imágenes, texto y estilos.

---

# Para empezar

Código es sólo texto en una página, así que podrías utilizar cualquier editor de texto como el 'Bloc de notas' de Windos o el editor de texto de Mac, pero es más fácil leer y encontrar errores si se utilizan mejores editores de texto que colorean el código de acuerdo al lenguaje de programación utilizado.

## 1.
Descarga un editor de texto si no tienes uno. [Visual Studio code](https://code.visualstudio.com/) es uno muy bueno tanto para Windows como para Mac.

## 2.
Descarga los archivos de arriba haciendo click en el botón verde y seleccionando 'Descargar zip' (o 'Download Zip')

![screenshot](./images/screenshots/screenshot-download-files.png)

## 3.
Hay unos cuantos navegadores diferentes, pero Google Chrome tiene herramientas de desarrollo incluidas y es fácil de utilizar. Puedes descargarlo [aquí](https://www.google.co.uk/chrome/) si aún no lo tienes.

## 4.
Abre el archivo `index.html` en tu navegador para ver la página web.

![screenshot](./images/screenshots/screenshot-open-in-browser.png)

## 5.
En Google Chrome puedes usar las herramientas de desarrollo (developer tools) para inspeccionar la página.

Haz click derecho en la página y selecciona `Inspeccionar`.

![screenshot](./images/screenshots/screenshot-get-web-inspector.png)

Ahora puedes ver y explorar el HTML y CSS de la página (o de cualquier página).

![screenshot](./images/screenshots/screenshot-inspecting-webpage.png)

## 6.
Ahora puedes probar a inspeccionar cualquier página y cambiar el texto, los colores, etc. Esto no tendrá ningun efecto permanente en el sitio, en cuanto refresques la página tus cambios desaparecerán.

## 7.
Los únicos dos archivos que necesitas para trabajar en la vista del código son `index.html` y `style.css`.

Abre estos dos archivos en el editor de texto (Visual Studio code).

![screenshot](./images/screenshots/screenshot-open-code-view.png)

**Nota:** El archivo `index.html` es el contenido te tu página web. Cuando se abre en un navegador se ve como una página web, mientras que si lo abres en un editor de texto verás el código que genera esa página web.

**Recuerda!** Cada vez que hagas un cambio en tu archivo en el editor de texto, necesitarás guardarlo (Archivo > Guardar, en Visual Studio Code) y entonces refrescar la pantalla en el navegador para que los cambios hagan efecto.

---

# Explicación sobre HTML y CSS

## El HTML

El archivo `index.html` es el contenido de tu página web

![screenshot](./images/screenshots/screenshot-html.png)

Algunas lecturas ligeras (en inglés):

[Basic HTML structure explained](https://www.w3schools.com/html/html_basic.asp)

[HTML elements explained](https://www.w3schools.com/html/html_elements.asp)

[HTML attributes explained](https://www.w3schools.com/html/html_attributes.asp)

Los elementos de HTML están representados por etiquetas (tags) HTML. Por ejemplo, una etiqueta 'body' envolverá la página entera, empezando así `<body>` y acabando con `</body>`.

Los atributos (attributes) son información adicional que se le da a los elementos HTML. Empiezan con el nombre del atributo, por ejemplo para el origen de una imagen utilizaremos `src`, un signo igual `=` y entre comillas `""` el link a la imagen.

Los elementos HTML que usamos en esta plantilla son:

* `<body>`...`</body>` - Un elemento body que envuelve el contenido de la página (sólo puede aparecer una vez en la página). 
* `<div>`...`</div>` - Etiquetas div que se usan todo el tiempo para envolver cualquier bloque
* `<h2>`...`</h2>` - Etiqueta h2 (cabecera tamaño 2) para la cabecera
* `<p>`...`</p>` - Etiqueta p (párrafo) para cualquier tipo de texto
* `<a href="/path/to/link">`...`</a>` - Etiqueta 'a' (para vínculos/links) envuelve texto o una imagen y contiene la dirección del en el atributo `href`.
* `<img src="/path/to/image.png" />` - Etiqueta img (imagen) son etiquetas únicas (se auto-cierran) y la dirección de la imagen se encontrará en el atributo `src`.

## The CSS

El archivo `styles.css` contiene los estilos de tu página.

![screenshot](./images/screenshots/screenshot-styles.png)

Cada set de normas corresponde a un elemento HTML, al que podemos referirnos por tipo: por ejemplo `<p>` sería `p` seguido de una llave de apertura `{` ... Aquí irían las normas de estilo ... y cerramos con una llave de cierre `}`.

Si necesitas ser más específico/a, puedes añadir el atributo 'class' (clase) al elemento HTML, por ejemplo aquí `<p class="copyright">` la clase 'copyright' se ha añadido al elemento 'p'. En los estilos usarías un punto para referirte a la clase `.copyright`.

![screenshot](./images/screenshots/screenshot-css-rules.png)

En el ejemplo de arriba, todo texto envuelto en un elemento `<p>` será de color verde oscuro y tamaño de 30px. Pero el texto en un elemento `<p>` que contenga la clase 'copyright' será de color blanco. Esto es porque estás haciendo referencia directamente a la clase, que tiene preferencia respecto al tipo de elemento.

---

# Tus tareas

## 1. Añade tu propio logo

* Put your cut out logo in the images folder.

The image files will need to be `.png` or `.jpg`.

![screenshot](./images/screenshots/screenshot-add-logo-image.png)

* In the HTML file, find where the current logo is `<img class="logo" src="./images/logo.jpg" alt="Spiral" />` and replace the file name `logo.jpg` with your own, and also the `alt` attribute text with the name and slogan (this will be hidden but is needed for accessibility and SEO etc).

![screenshot](./images/screenshots/screenshot-logo-html.png)

* In the CSS file, find where it says `.logo` - these are the style rules that define what the logo looks like on the page. You can change the width here to suit your logo.

![screenshot](./images/screenshots/screenshot-logo-styles.png)

## 2. Añade tu propia imagen para la aplicación

* Same steps as above for the app image. Can you work it out?

## 3. Añade tu contenido en texto

* Find the text in the HTML which will be wrapped in `<p>` and `<h2>` tags, and replace with your own content. So this should be the heading, text and copyright text.
* You should also change the title of the page (which appears on the tab of the browser window). This is wrapped in a `<title>` tag near the top of the index.html.

## 4. Añade tu propia fuente

* Find a font you like from [Google web fonts](https://fonts.google.com/)

For example the 'Lobster' font.

![screenshot](./images/screenshots/screenshot-font-family.png)

* Click on the red plus icon, the font will appear in a black box at the bottom. Click the box to view the font you have selected (making sure it is just one font).

![screenshot](./images/screenshots/screenshot-font-family-selected.png)

* It gives code snippets for both the HTML and the CSS. Find the similar code snippets in this template and replace with your own.

In your `index.html` you will currently have...

![screenshot](./images/screenshots/screenshot-html-link-to-font.png)

In your `styles.css` you will currently have...

![screenshot](./images/screenshots/screenshot-font-in-css.png)

## 5. Juega con los estilos de la página...

The text elements currently on the page that you would probably want to change are:

* `p`
* `h2`
* `.copyright`

The main styles you may want to change for the text are:

* `color` : #000000; (applies to text)
* `font-size` : 14px;

Note: Colours can also be the name of the colour eg. `'blue'` (has to be in single quotes if it is a colour name). You have more control if it is a hex code colour eg. `#000000`.

The containing elements currently on the page that you would probably want to change are:

* `body`
* `.header`
* `.footer`
* `.col-image`
* `.col-text`

The main styles you may want to use/change for containing elements are:

* `background-color` : #FFFFFF; (applies to the background colour)
* `width` : 100px; (can be px or %)
* `height` : 200px; (if the width is set, the height doesn't usually need to be)
* `border-bottom` : 1px dotted #CCCCCC (3 values should be given - thickness, type of border, colour) [more about borders](https://www.w3schools.com/css/css_border.asp)

For spacing on text and containing elements, `padding` and `margin` are used. You probably wouldn't want to change them but if you do, have a read about how they work here: [the box model](https://www.w3schools.com/css/css_boxmodel.asp), [margin](https://www.w3schools.com/css/css_margin.asp), [padding](https://www.w3schools.com/css/css_padding.asp)

You can also find extensive lists of CSS rules [here](https://www.w3schools.com/css/default.asp) (the links on the left)

## 6. Tarea extra - añade links falsos a los botones de Apple Store y Google Play

Estos links están creados con una imagen envuelta por un elemento `<a>` (link), y el la dirección del link se tiene que añadir en el atributo `href`.

* Puedes añadir links a estos elementos y comprobar que funcionan?

## Otras lecturas (en inglés)

[A list of learning resources](https://github.com/Nezteb/Teaching_WebDev)
