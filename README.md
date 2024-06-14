
<div align="center">

# HTML_CSS_Definitive


<a href="https://postimg.cc/14KdYq2y">
  <img src="https://i.postimg.cc/C5QKL7dr/imagen-2024-06-02-162204992-transformed.png" alt="imagen-2024-03-07-211141241" width="500"/>
</a>

<p><strong>Esta es una recopilación de los temas vistos en el Curso Definitivo de HTML y CSS</strong></p>

</div>

# Tabla de contenido
- [HTML\_CSS\_Definitive](#html_css_definitive)
- [Tabla de contenido](#tabla-de-contenido)
- [HTML](#html)
  - [1. `Index y su estructura básica: Head`](#1-index-y-su-estructura-básica-head)
    - [1.1. *`Anatomía de una Página Web`*](#11-anatomía-de-una-página-web)
  - [| |  |](#---)
    - [1.2. *`Componentes de una Página Web`*](#12-componentes-de-una-página-web)
  - [2. `Etiquetas mas utilizadas en HTML`](#2-etiquetas-mas-utilizadas-en-html)
    - [Consulta del glosario de etiquetas](#consulta-del-glosario-de-etiquetas)
  - [3. `Anatomia de una etiqueta de HTML`](#3-anatomia-de-una-etiqueta-de-html)
  - [4. `Tipos de imagenes`](#4-tipos-de-imagenes)
    - [4.1. **`Tipos de imágenes para web`**](#41-tipos-de-imágenes-para-web)
      - [1. *`Lossless`* `(sin pérdida)`](#1-lossless-sin-pérdida)
      - [2. *`Lossy`* `(con pérdida)`](#2-lossy-con-pérdida)
    - [4.2. *`Formatos de imagen para web`*](#42-formatos-de-imagen-para-web)
  - [5. `Optimización de imagenes`](#5-optimización-de-imagenes)
    - [5.1. *`Tamaño promedio de una imagen`*](#51-tamaño-promedio-de-una-imagen)
    - [5.2. *`Recursos para optimizar imagenes`*](#52-recursos-para-optimizar-imagenes)
  - [6.  `Etiqueta <img>, <figure> y <figcaption>`](#6--etiqueta-img-figure-y-figcaption)
  - [7. `Etiqueta de <video>`](#7-etiqueta-de-video)
  - [6. `<input types..` existentes en HTML](#6-input-types-existentes-en-html)
  - [8. Attribute `autocomplete` Valores existentes en HTML](#8-attribute-autocomplete-valores-existentes-en-html)
- [CSS](#css)
  - [7. Hoja de trucos de CSS y recursos](#7-hoja-de-trucos-de-css-y-recursos)
    - [Paginas para practicar `Flexbox` y `CSS Grid`](#paginas-para-practicar-flexbox-y-css-grid)
  - [8. Formas de dar estilos a un etiqueta html con el `elemento`, `class` o `id`](#8-formas-de-dar-estilos-a-un-etiqueta-html-con-el-elemento-class-o-id)
    - [Diferencia entre elemento, `class` y `id`](#diferencia-entre-elemento-class-y-id)
  - [9. `Pseudo-clases` y `Pseudo-elementos` y la efectividad de la metodologÍa de `BEM`](#9-pseudo-clases-y-pseudo-elementos-y-la-efectividad-de-la-metodología-de-bem)
    - [Diferencias entre Pseudo-clases y Pseudo-elementos](#diferencias-entre-pseudo-clases-y-pseudo-elementos)


# HTML 


## 1. `Index y su estructura básica: Head`

En el `head` **van todos los archivos importantes para el correcto funcionamiento de nuestra plataforma pero que no deben ser visibles por lo usuarios.** Algunos de estos archivos pueden ser: 

- **Frameworks**

- **Librerías**

- **Estilos**

- **Fuentes**

- **APIs**

```html
<!DOCTYPE html>
<!-- Esta etiqueta es para que el navegador sepa que tipo de documento es en este caso es un documento html -->
<html lang="es">

<head> <!-- El head es la cabecera del documento, es donde se colocan los metadatos, los estilos, los scripts, etc. -->
    <meta charset="UTF-8"> <!-- Esta etiqueta es para que el navegador sepa que tipo de caracteres se van a utilizar -->
    <meta name="description" content="Esta pagina es de prueba xd">
    <!-- Esta etiqueta es para que los buscadores sepan de que trata la pagina -->
    <meta name="robots" content="index,follow">
    <!-- Esta etiqueta es para que los buscadores sepan que indexen la pagina y que sigan los enlaces -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minium-scale=1.0">
    <!-- Esta etiqueta es para que la pagina se adapte a cualquier dispositivo y tenga un zoom minimo de 1 -->
    <link rel="stylesheet" href="/styles/style.css"> <!-- Esta etiqueta es para enlazar el archivo css -->
    <title>Explicación de las primeras etiquetas de HTML</title>
</head>
<body> <!-- El body es el cuerpo del documento, es donde se coloca todo el contenido de la pagina -->
</body>
</html>
```

### 1.1. *`Anatomía de una Página Web`*

**HTML** (HyperText Markup Language) es un lenguaje de marcado que estructura los sitios web.

- **`Container`**: Contenedor principal.

- **`Header`**: Cabecera de la página, usualmente contiene el logo y el menú de navegación.

- **`Main content`**: Estructura principal, como el feed de una red social.

- **`Sidebar`**: Contenido secundario, usualmente se encuentra a los lados del contenido principal.

- **`Footer`**: Pie de página, se encuentra al fondo del sitio web.


```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, minium-scale=1.0">
    <title>Index y su estructura basica "Semantica adecuada"</title>
</head>
<body>


<!-- PRIMERA PARTE DE UNA PAGINA -->
    <header> <!-- El header es la cabecera de la pagina, es donde se coloca el menu, el logo, etc. -->

        <!-- PRIMERA SUBPARTE DE UNA PAGINA (LOGO) -->
        <div class="logo"> 
            <img src="https://via.placeholder.com/150" alt="Logo"> <!-- El img es la etiqueta para colocar una imagen -->
        <div class="title">
            <h1>Titulo Grande</h1> <!-- El h1 es la etiqueta para colocar un titulo encabezado Grande -->
        </div>
        <div class="subtitle">
            <h2>Titulo Mediano</h2> <!-- El h2 es la etiqueta para colocar un subtitulo encabezado Mediano-->
        </div>
        <div class="text">
            <p>Lorem ipsum</p><!-- El p es la etiqueta para colocar un parrafo -->
        </div>

        <!-- SEGUNDA SUBPARTE DE UNA PAGINA (MENU) O NAVIGATOR -->
        <nav> <!-- El nav es la etiqueta para colocar el menu -->
            <ul> <!-- El ul es la etiqueta para colocar una lista -->
                <li><a href="#">Inicio</a></li> 
                <!-- El li es la etiqueta para colocar un elemento de la lista -->
                <!-- El a es la etiqueta para colocar un enlace -->
                <li><a href="#">Acerca de</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
    </header>
    

<!-- SEGUNDA PARTE DE UNA PAGINA -->
    <main> <!-- El main es el cuerpo de la pagina, es donde se coloca el contenido principal de la pagina -->

        <section>
            <!-- El section es una seccion de la pagina, es donde se coloca el contenido secundario de la pagina -->

            <article> <!-- El article es un articulo de la pagina, es donde se coloca el contenido de la pagina -->
                <h3>Titulo Pequeño</h3> <!-- El h3 es la etiqueta para colocar un titulo encabezado Pequeño -->
            </article>
            <article>
                <h3>Titulo Pequeño</h3>
            </article>
            <article>
                <h3>Titulo Pequeño</h3>
            </article>

            <ol><!-- El ol es la etiqueta para colocar una lista ordenada -->
                <li>Elemento 1 de lista ordenada</li>
                <li>Elemento 2 de lista ordenada</li>
                <li>Elemento 3 de lista ordenada</li>
            </ol>
        </section>


<!--TERCERA PARTE DE UNA PAGINA (OPCIONAL)  -->
        <aside> <!-- El aside es una seccion de la pagina, es donde se coloca el contenido secundario de la pagina -->
            <h3>Titulo Pequeño</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.</p>
        </aside>
    </main>


<!-- CUARTA PARTE DE UNA PAGINA -->
    <footer> <!-- El footer es el pie de pagina, es donde se coloca el contenido del pie de pagina -->
    </footer>
</body>

</html>
```
>[!NOTE]
> 
> Las etiquetas en HTML nos ayudan a diferenciar en qué parte del contenido nos encontramos.

|  |  |
|:---------:|:---------:|
|[![imagen-2024-01-18-212336956.png](https://i.postimg.cc/0rRKBM8s/imagen-2024-01-18-212336956.png)](https://postimg.cc/fSCb3bt2) | [![imagen-2024-01-18-212452685.png](https://i.postimg.cc/j2VyGkXm/imagen-2024-01-18-212452685.png)](https://postimg.cc/YG34FRTz) |
---

### 1.2. *`Componentes de una Página Web`*

La web se conforma de tres conceptos:

- **`URL` (Uniform Resource Locator)**: Identificador único del sitio en el navegador.

- **`HTTP` (Protocolo de Transferencia de Hipertexto)**: Estándar para enviar datos entre el cliente y el servidor.

- **`HTML` (Hyper Text Markup Language)**: Código para estructurar el contenido de la web. Es un lenguaje interpretado y un estándar, por lo que el código es el mismo en cualquier navegador o dispositivo.
---



## 2. `Etiquetas mas utilizadas en HTML`

<p align="center">
  <img src="https://i.postimg.cc/NfcNw7wH/imagen-2024-01-18-163130336.png" alt="Aquí va el texto del enlace">
</p>

### Consulta del glosario de etiquetas
[![Aquí va el texto del enlace](https://i.postimg.cc/Y2GHRDTk/imagen-2024-01-18-213228704.png)](https://i.emezeta.com/weblog/html5-cheatsheet/html5-cheatsheet-2019.pdf)


## 3. `Anatomia de una etiqueta de HTML`
|  |  |
|:---------:|:---------:|
| ![Imagen 1](https://i.postimg.cc/TPtM4dNp/imagen-2024-01-18-181708773.png) |[![imagen-2024-01-18-181844399.png](https://i.postimg.cc/FFdz381j/imagen-2024-01-18-181844399.png)](https://postimg.cc/kDC7djQ4) |

> [!IMPORTANT]
>
> - **No todas las etiquetas llevan una etiqueta de cierre.** Las que llevan un cierre son aquellas que albergan un contenido que nos dice a dónde nos va a llevar (nombre de la página, nombre del link).
> 
> - Lo que va dentro de la etiqueta de apertura es un atributo (nombre del atributo = `href` y el valor del atributo es la `= url`).
> 
> - **`El contenido + la etiqueta = Elemento`**



## 4. `Tipos de imagenes`
### 4.1. **`Tipos de imágenes para web`**

#### 1. *`Lossless`* `(sin pérdida)`
- Capturan todos los datos del archivo original.

- No se pierde nada del archivo original.

- Puede comprimirse, pero podrá reconstruir su imagen al estado original

#### 2. *`Lossy`* `(con pérdida)`
- Se aproximan a su imagen original.

- Podría reducir la cantidad de colores en su imagen o analizar la imagen en busca de datos innecesarios.

- Por consiguiente puede reducir su tamaño, lo que mejora el tiempo de carga de la página, pero pierde su calidad.

- Los archivos tipo lossy son mucho más livianos que los archivos tipo lossless, por lo que son ideales para usar en sitios en donde el tamaño del archivo y la velocidad de descarga son importantes.

### 4.2. *`Formatos de imagen para web`*

- **El tamaño promedio de una imagen debe ser de 70 a 100 `kilobytes`.**

<p align="center">
  <img src="https://i.postimg.cc/mgpt804G/imagen-2024-01-23-172553242.png" alt="Aquí va el texto del enlace" width="500"/>
</p>

## 5. `Optimización de imagenes`

### 5.1. *`Tamaño promedio de una imagen`* 
<p align="center">
  <img src="https://i.postimg.cc/Jzk92XV4/imagen-2024-01-23-172948494.png" alt="Aquí va el texto del enlace" width="500">
</p>

### 5.2. *`Recursos para optimizar imagenes`* 
<div align="center">

|Retira metadatos | Mejora el tamaño de la img |
|:---------:|:---------:|
|[![Aquí va el texto del enlace](https://i.postimg.cc/8CnXkPVn/imagen-2024-01-23-173346423.png)](https://www.verexif.com/) |[![Aquí va el texto del enlace](https://i.postimg.cc/N0tPCPkp/imagen-2024-01-23-173126412.png)](https://tinypng.com/)|



| Descargar imagenes sin copyrigth | Compresores de imagenes |
|:---------:|:---------:|
|[Pexels](https://www.pexels.com/es-es/) |[Optimizilla](https://imagecompressor.com/es/)|
|[Pixabay](https://pixabay.com/) |[IloveIMG](https://www.iloveimg.com/es)|
|[Freerangestock](https://www.freerangestock.com/) | |
|[Realisticshots](https://realisticshots.com/) | |
|[Picjumbo](https://picjumbo.com/) | |
|[Magdeleine](https://magdeleine.co/) | |
|[Creative Commons](https://search.creativecommons.org/) | |
|[Free jpg](https://www.freejpg.com.ar/) | |

</div>


## 6.  `Etiqueta <img>, <figure> y <figcaption>`

> [!NOTE]
>
> **Es recomendable descargar imágenes solo de tamaño grande, mediano o pequeño.**

```html
  <figure style="margin: 0;">
    <img src="./pics/small.jpg" alt="Imagen de un perrito" />
    <figcaption>Es una imagen de un perrito 🐶</figcaption>
  </figure>
```
- `src`: Es el atributo que nos permite colocar la URL de la imagen.
- `alt`: Es el atributo que nos permite colocar un texto alternativo a la imagen.
- `figure`: Es una etiqueta que nos permite colocar una imagen con un texto alternativo.
- `figcaption`: Es una etiqueta que nos permite colocar un texto alternativo a la imagen.

> [!TIP]
> 
> - **Por buenas prácticas siempre deberíamos usar la etiqueta figure para insertar un archivo multimedia**
> 
> - Tambien es recomendado **almacenar las imagenes en una carpeta llamada `/assets` o `/img` para tener un orden en nuestro proyecto.**
>

## 7. `Etiqueta de <video>`

```html
<section>
            <video controls preload="auto">
                <source src="/HTML_Multimedia/Tags_video/video_prueba.mp4#t=10,60" />
                <source src="/HTML_Multimedia/Tags_video/video_prueba.mp4#t=10,60" />
            </video> 
            <iframe width="560" height="315" src="https://www.youtube.com/embed/uI6o97A4IrI" frameborder="0"
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
                allowfullscreen></iframe> <!-- Esta etiqueta es para incrustar videos de youtube en la pagina web mostrandose como un embed de youtube lo que es importante especificarlo embed -->
        </section>
```
- `video`: Es una etiqueta que nos permite colocar un video en la página web.
- `src`: Es un atributo que nos permite colocar la URL del video.

  - `#t=10,60`: Es un atributo que nos permite colocar un tiempo de inicio y un tiempo de finalización del video.

- `controls`: Es un atributo que nos permite colocar controles al video.

- `preload`: Es un atributo que nos permite cargar el video antes de que se reproduzca.

- `source`: Es una etiqueta que nos permite colocar la URL del video.

- `iframe`: Es una etiqueta que nos permite colocar un video de youtube en la página web.

- `allow`: Es un atributo que nos permite colocar permisos al video de youtube.

- `allowfullscreen`: Es un atributo que nos permite colocar un permiso para que el video de youtube se pueda ver en pantalla completa.

## 6. `<input types..` existentes en HTML
<p align="center">
  <a href="https://developer.mozilla.org/es/docs/Web/HTML/Element/input">
    <img src="https://i.postimg.cc/MTdcbqqh/imagen-2024-01-25-181810160.png" alt="Aquí va el texto del enlace">
  </a>
</p>

## 8. Attribute `autocomplete` Valores existentes en HTML
<p align="center">
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/autocomplete">
    <img src="https://i.postimg.cc/pr31rNhF/imagen-2024-01-25-185245182.png" alt="Aquí va el texto del enlace">
  </a>
</p>


# CSS

## 7. Hoja de trucos de CSS y recursos
<p align="center">
  <a href="https://htmlcheatsheet.com/css/">
    <img src="https://i.postimg.cc/pXVG5w9X/imagen-2024-02-05-150922143.png" alt="Aquí va el texto del enlace">
  </a>
</p>


### Paginas para practicar `Flexbox` y `CSS Grid`
|Flexbox Froggy | Grid Garden |
|:---------:|:---------:|
|[![Aquí va el texto del enlace](https://i.postimg.cc/xdbJx1Zj/imagen-2024-02-05-151723690.png)](https://flexboxfroggy.com/#es) |[![Aquí va el texto del enlace](https://i.postimg.cc/zDs3PNr0/imagen-2024-02-05-151829227.png)](https://cssgridgarden.com/#es)|



## 8. Formas de dar estilos a un etiqueta html con el `elemento`, `class` o `id`

### Diferencia entre elemento, `class` y `id`
- El elemento se aplica a todos los elementos de ese tipo siendo la menos practica
- La `class` se aplica a todos los elementos que tengan esa clase
- El `id` se aplica a un solo elemento 

**Por lo tanto la mas recomendada es la `class`**



## 9. `Pseudo-clases` y `Pseudo-elementos` y la efectividad de la metodologÍa de `BEM`

### Diferencias entre Pseudo-clases y Pseudo-elementos
|Pseudo-Clases | Pseudo-Elementos |
|:---------:|:---------:|
|[![Aquí va el texto del enlace](https://i.postimg.cc/sDjm2xK0/imagen-2024-02-05-164155325.png)](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes) |[![Aquí va el texto del enlace](https://i.postimg.cc/t47zhcK3/imagen-2024-02-05-164211893.png)](https://developer.mozilla.org/es/docs/Web/CSS/Pseudoelementos)|


> [!IMPORTANT]
>
> ### ¿En que consiste la metodologia de BEM y que tan efectiva es?
> 
> La metodología **Bloque**, **Elemento**, **Modificador** (comúnmente conocida como `BEM`) es una convención de nomenclatura popular para clases en HTML y CSS. Desarrollado por el equipo de Yandex, su objetivo es ayudar a los desarrolladores a comprender mejor la relación entre HTML y CSS.
> 
> ### ¿Como nombrar correctamente las clases usando esta metodología?
> **Solo usa clases.** 
> 
> Las nombra siguiendo el siguiente patrón:
> 
> `BLOQUE__ELEMENTO—MODIFICADOR` (son **2 guiones**, se **usa 1 guión para separar palabras**).
> 
> - **Bloque**: sección que puede funcionar por sí sola.
> - **Elemento**: forma una de las partes del bloque.
> - **Modificador**: variaciones de un mismo bloque/elemento.

| Representación de `BEM` | Recurso visual de `BEM` |
|:---------:|:---------:|
|![Aquí va el texto del enlace](https://i.postimg.cc/hjKgYVb0/imagen-2024-02-05-163646109.png) |[![Aquí va el texto del enlace](https://i.postimg.cc/vByHdJMf/imagen-2024-02-05-163633531.png)](https://bem-cheat-sheet.9elements.com)|

