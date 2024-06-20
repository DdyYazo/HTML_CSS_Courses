
<div align="center">

# **HTML Concepts and Fundaments**

<p align="center">
  <img src="https://i.postimg.cc/DwvrC4gQ/imagen-2024-06-14-175050051.png" alt="Aquí va el texto del enlace" width="500">
</p>

</div>

# **Tabla de contenido**
- [**HTML Concepts and Fundaments**](#html-concepts-and-fundaments)
- [**Tabla de contenido**](#tabla-de-contenido)
- [**HTML**](#html)
  - [1. **`Index y su estructura básica: Head`**](#1-index-y-su-estructura-básica-head)
    - [1.1. *`Anatomía de una Página Web`*](#11-anatomía-de-una-página-web)
      - [**\_DESCRICIÓN DE LA ESTRUCTURA HTML DE LA PAGINA**](#_descrición-de-la-estructura-html-de-la-pagina)
      - [**\_EJEMPLO DE UNA ESTRUCTURA SEMANTICA (SIN DIVS) EN HTML**](#_ejemplo-de-una-estructura-semantica-sin-divs-en-html)
    - [1.2. *`Componentes de una Página Web`*](#12-componentes-de-una-página-web)
  - [2. **`Etiquetas mas utilizadas en HTML`**](#2-etiquetas-mas-utilizadas-en-html)
    - [2.1. *`Consulta del glosario de etiquetas`*](#21-consulta-del-glosario-de-etiquetas)
  - [3. **`Anatomia de una etiqueta de HTML`**](#3-anatomia-de-una-etiqueta-de-html)
- [**Etiquetas Multimedia**](#etiquetas-multimedia)
  - [4. **`Tipos de imagenes`**](#4-tipos-de-imagenes)
    - [4.1. *`Tipos de imágenes para web`*](#41-tipos-de-imágenes-para-web)
      - [1. *`Lossless`* `(sin pérdida)`](#1-lossless-sin-pérdida)
      - [2. *`Lossy`* `(con pérdida)`](#2-lossy-con-pérdida)
    - [4.2. *`Formatos de imagen para web`*](#42-formatos-de-imagen-para-web)
  - [5. **`Optimización de imagenes`**](#5-optimización-de-imagenes)
    - [5.1. *`Tamaño promedio de una imagen`*](#51-tamaño-promedio-de-una-imagen)
    - [5.2. *`Recursos para optimizar imagenes`*](#52-recursos-para-optimizar-imagenes)
  - [6.  **`Etiqueta <img>, <figure> y <figcaption>`**](#6--etiqueta-img-figure-y-figcaption)
  - [7. **`Etiqueta de <video>`**](#7-etiqueta-de-video)
- [**Formularios**](#formularios)
  - [8. **`Etiqueta <form> e <input>`**](#8-etiqueta-form-e-input)
  - [9. **`Calendario en HTML (Forma profesional y forma compacta)`**](#9-calendario-en-html-forma-profesional-y-forma-compacta)
  - [10. **`Atributo autocomplete y required en los formularios`**](#10-atributo-autocomplete-y-required-en-los-formularios)
  - [11. **`Etiqueta <select> y <option> (Con buenas y malas practicas) para las listas desplegables en formularios`**](#11-etiqueta-select-y-option-con-buenas-y-malas-practicas-para-las-listas-desplegables-en-formularios)
  - [12. **`Atributo type="submit" y button en los formularios`**](#12-atributo-typesubmit-y-button-en-los-formularios)


# **HTML** 

## 1. **`Index y su estructura básica: Head`**

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
    <header> 
        <!-- PRIMERA SUBPARTE DE UNA PAGINA (LOGO) -->
        <div class="logo"> 
            <img src="https://via.placeholder.com/150" alt="Logo"> 
          <div class="title">
              <h1>Titulo Grande</h1> 
          </div>
        </div>

        <!-- SEGUNDA SUBPARTE DE UNA PAGINA (MENU) O NAVIGATOR -->
        <nav> 
            <ul> 
                <li><a href="#">Inicio</a></li> 
                <li><a href="#">Acerca de</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </nav>
    </header>
    

<!-- SEGUNDA PARTE DE UNA PAGINA -->
    <main>
        <section>
            <article>
                <h3>Titulo Pequeño</h3> 
            </article>
            <article>
                <h3>Titulo Pequeño</h3>
            </article>
            <article>
                <h3>Titulo Pequeño</h3>
            </article>

            <ol>
                <li>Elemento 1 de lista ordenada</li>
                <li>Elemento 2 de lista ordenada</li>
                <li>Elemento 3 de lista ordenada</li>
            </ol>
        </section>


<!--TERCERA PARTE DE UNA PAGINA (OPCIONAL)  -->
        <aside> 
            <h3>Titulo Pequeño</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quisquam, voluptatum.</p>
        </aside>
    </main>


<!-- CUARTA PARTE DE UNA PAGINA -->
    <footer> 
        <p>© 2021 Todos los derechos reservados</p>
    </footer>
</body>

</html>
```

#### **_DESCRICIÓN DE LA ESTRUCTURA HTML DE LA PAGINA**

- **PRIMERA PARTE DE UNA PAGINA (`header`)**

  - **`header`**: Es la cabecera de la pagina, es donde se coloca el menu, el logo, etc.
 
  - **PRIMERA SUBPARTE DEL HEADER (LOGO)**
 
    - **`div`**: Es una etiqueta que nos permite colocar un contenedor en la página web.
  
    - **`img`**: Es una etiqueta que nos permite colocar una imagen en la página web.
    
      - **`src`**: Es un atributo que nos permite colocar la URL de la imagen.
    
      - **`alt`**: Es un atributo que nos permite colocar un texto alternativo a la imagen.
    
      - **`title`**: Es un atributo que nos permite colocar un título a la imagen.
  - **SEGUNDA SUBPARTE DEL HEADER (MENU) O NAVIGATOR**
  
    - **`nav`**: Es una etiqueta que nos permite colocar un menú en la página web.
  
    - **`ul`**: Es una etiqueta que nos permite colocar una lista sin ordenar en la página web.
  
    - **`li`**: Es una etiqueta que nos permite colocar un elemento de la lista en la página web.
  
    - **`a`**: Es una etiqueta que nos permite colocar un enlace en la página web.
  
      - **`href`**: Es un atributo que nos permite colocar la URL a la que se va a dirigir el enlace.

- **SEGUNDA PARTE DE UNA PAGINA (`main`)**

  - **`main`**: Es el cuerpo de la pagina, es donde se coloca el contenido principal de la pagina.
  
  - **`section`**: Es una seccion de la pagina, es donde se coloca el contenido secundario de la pagina.
  
  - **`article`**: Es un articulo de la pagina, es donde se coloca el contenido de la pagina.
  
  - **`h3`**: Es la etiqueta para colocar un titulo encabezado Pequeño.
  
  - **`ol`**: Es la etiqueta para colocar una lista ordenada.
  
    - **`li`**: Es la etiqueta para colocar un elemento de la lista ordenada.
  
- **TERCERA PARTE DE UNA PAGINA OPCIONAL (`aside`)**

  - **`aside`**: Es una seccion de la pagina, es donde se coloca el contenido secundario de la pagina.
  
  - **`h3`**: Es la etiqueta para colocar un titulo encabezado Pequeño.
  
  - **`p`**: Es la etiqueta para colocar un parrafo de texto.

- **CUARTA PARTE DE UNA PAGINA (`footer`)**

  - **`footer`**: Es el pie de pagina, es donde se coloca el contenido del pie de pagina. 

>[!NOTE]
> 
> Las etiquetas en HTML nos ayudan a diferenciar en qué parte del contenido nos encontramos.


|  |  |
|:---------:|:---------:|
|[![imagen-2024-01-18-212336956.png](https://i.postimg.cc/0rRKBM8s/imagen-2024-01-18-212336956.png)](https://postimg.cc/fSCb3bt2) | [![imagen-2024-01-18-212452685.png](https://i.postimg.cc/j2VyGkXm/imagen-2024-01-18-212452685.png)](https://postimg.cc/YG34FRTz) |


#### **_EJEMPLO DE UNA ESTRUCTURA SEMANTICA (SIN DIVS) EN HTML**

```html

```

### 1.2. *`Componentes de una Página Web`*

La web se conforma de tres conceptos:

- **`URL` (Uniform Resource Locator)**: Identificador único del sitio en el navegador.

- **`HTTP` (Protocolo de Transferencia de Hipertexto)**: Estándar para enviar datos entre el cliente y el servidor.

- **`HTML` (Hyper Text Markup Language)**: Código para estructurar el contenido de la web. Es un lenguaje interpretado y un estándar, por lo que el código es el mismo en cualquier navegador o dispositivo.
---


## 2. **`Etiquetas mas utilizadas en HTML`**

<p align="center">
  <img src="https://i.postimg.cc/NfcNw7wH/imagen-2024-01-18-163130336.png" alt="Aquí va el texto del enlace" width="500"/>
</p>

### 2.1. *`Consulta del glosario de etiquetas`*

<p align="center">
  <a href="https://i.emezeta.com/weblog/html5-cheatsheet/html5-cheatsheet-2019.pdf">
    <img src="https://i.postimg.cc/Y2GHRDTk/imagen-2024-01-18-213228704.png" alt="Aquí va el texto del enlace" width="500"/>
  </a>
</p>

## 3. **`Anatomia de una etiqueta de HTML`**
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



# **Etiquetas Multimedia** 

## 4. **`Tipos de imagenes`**
### 4.1. *`Tipos de imágenes para web`*

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

## 5. **`Optimización de imagenes`**

### 5.1. *`Tamaño promedio de una imagen`* 
<p align="center">
  <img src="https://i.postimg.cc/Jzk92XV4/imagen-2024-01-23-172948494.png" alt="Aquí va el texto del enlace" width="500">
</p>
  <p align="center"><strong>El tamaño promedio de una imagen debe ser de 70 a 100 kilobytes (kb).</strong></p>

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


## 6.  **`Etiqueta <img>, <figure> y <figcaption>`**

> [!NOTE]
>
> **Es recomendable descargar imágenes solo de tamaño grande, mediano o pequeño.**

```html
  <figure style="margin: 0;">
    <img src="./pics/small.jpg" alt="Imagen de un perrito" />
    <figcaption>Es una imagen de un perrito 🐶</figcaption>
  </figure>
```
---

- **DESCRICIÓN DE LAS ETIQUETAS DE IMAGEN**

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

## 7. **`Etiqueta de <video>`**

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
---

**DESCRICIÓN DE LAS ETIQUETAS DE VIDEO**

- **`video`**: Es una etiqueta que nos permite colocar un video en la página web.
- **`src`**: Es un atributo que nos permite colocar la URL del video.

  - `#t=10,60`: Es un atributo que nos permite colocar un tiempo de inicio y un tiempo de finalización del video.

- **`controls`**: Es un atributo que nos permite colocar controles al video.

- **`preload`**: Es un atributo que nos permite cargar el video antes de que se reproduzca.

- **`source`**: Es una etiqueta que nos permite colocar la URL del video.

- **`iframe`**: Es una etiqueta que nos permite colocar un video **de** youtube en la página web.

- **`allow`**: Es un atributo que nos permite colocar permisos al video de youtube.

- **`allowfullscreen`**: Es un atributo que nos permite colocar un permiso para que el video de youtube se pueda ver en pantalla completa.

# **Formularios**

## 8. **`Etiqueta <form> e <input>`**

Los formularios son una parte fundamental de las páginas web, ya que nos permiten interactuar con los usuarios y obtener información de ellos.

> [!IMPORTANT]
>
> Se deben generar buenos formularios para que los usuarios puedan interactuar con la página web de manera sencilla y rápida.

```html

<!-- Formulario con malas practicas -->
<div>
    <input type="text" />
    <input type="text" />
    <input type="text" />
    <input type="text" />
</div>

<!--  Formulario con buenas practicas -->
<section>
    <form action="">
      <label for="nombre">
          <span>¿Cual es tu nombre?</span>
          <input type="text" name="nombre" id="nombre" placeholder="Ingrese su nombre" />
      </label>
      <label for="inicio-platzi">
          <span>¿Que dia comenzaste en platzi? </span>
          <input type="date" name="inicio-platzi" id="inicio-platzi" />
      </label>
      <label for="email">
          <span>¿Cual es tu correo electronico?</span>
          <input type="email" name="email" id="email" placeholder="Ingrese su correo electronico" />
      </label>
    </form>
</section>
```

**DESCRICIÓN DE LAS ETIQUETAS DE FORMULARIO**

- **`form`**: Es una etiqueta que nos permite colocar un formulario en la página web.

  - **`action`**: Es un atributo que nos permite colocar la URL a la que se enviará la información del formulario.

- **`label`**: Es una etiqueta que nos permite colocar un texto a un input.
  
  - **`for`**: Es un atributo que nos permite colocar el id del input al que se le asignará el texto.

- **`span`**: Es una etiqueta se usa en los formulario para colocar un texto de ayuda.

- **`input`**: Es una etiqueta que nos permite colocar un input en el formulario.
  
  - **`type`**: Es un atributo que nos permite colocar el tipo de input.
  
  - **`name`**: Es un atributo que nos permite colocar el nombre del input.

  - **`id`**: Este atributo es para especificar el **`id`** del campo de texto que se relaciona con el atributo **`for`** de la etiqueta **`label`**

  - **`placeholder`**: Es un atributo que nos permite colocar un texto de ayuda en el input.

Es importante tener en cuenta que existen varios **`types`** en la etiqueta **`<input>`** que se pueden utilizar en los formularios, en la pagina de **[MDN Web Docs](https://developer.mozilla.org/es/docs/Web/HTML/Element/input) se pueden encontrar todos los tipos de `<input types="">` que se pueden utilizar en los formularios**.

## 9. **`Calendario en HTML (Forma profesional y forma compacta)`**

```html

<!-- Forma profesional -->
<form action="">
  <label for="hora">
      <span>Hora</span>
      <input type="time" name="hora" id="hora" />
  </label>
  <label for="dia">
      <span>Dia</span>
      <input type="date" name="dia" id="dia" />
  </label>
  <label for="semana">
      <span>Semana</span>
      <input type="week" name="semana" id="semana" />
  </label>
  <label for="mes">
      <span>Mes</span>
      <input type="month" name="mes" id="mes" />
  </label>
  <input type="submit" name="mes" id="mes" />
</form>

<!-- Forma compacta -->
<form action="">
  <label for="calendario">
      <span>Calendario</span>
      <input type="datetime-local" name="calendario" id="calendario" />
  </label>
</form>
```

**DESCRICIÓN DE LAS ETIQUETAS DE CALENDARIO**

- **`time`**: Es un atributo que nos permite colocar un input de tipo hora en el formulario.

- **`date`**: Es un atributo que nos permite colocar un input de tipo fecha en el formulario.

- **`week`**: Es un atributo que nos permite colocar un input de tipo semana en el formulario.

- **`month`**: Es un atributo que nos permite colocar un input de tipo mes en el formulario.

- **`datetime-local`**: Es un atributo que nos permite colocar un input de tipo fecha y hora en el formulario.

- **`submit`**: Es un atributo que nos permite crear un botón de envío en el formulario.

## 10. **`Atributo autocomplete y required en los formularios`**

```html
<form action="">
  <label for="nombre">
      <span>¿Cual es tu nombre?</span>
      <input type="text" name="nombre" id="nombre" autocomplete="name" required />
  </label>
  <label for="email">
      <span>¿Cual es tu correo?</span>
      <input type="email" name="email" id="email" autocomplete="email" required />
  </label>
  <label for="pais">
      <span>¿De que pais eres?</span>
      <input type="text" name="pais" id="pais"  autocomplete="country" required />
  </label>
  <label for="cp">
      <span>¿Cual es tu codigo postal?</span>
      <input type="text" name="cp" id="cp" autocomplete="postal-code" required />
  </label>
  <input type="submit" name="enviar" id="enviar" />
</form>
```

**DESCRICIÓN DE LOS ATRIBUTOS DE AUTOCOMPLETE Y REQUIRED**

- **`autocomplete`**: Es un atributo que nos permite colocar un autocompletado basado en los datos que halla recopilado el navegador.

- **`required`**: Es un atributo que nos permite colocar un campo obligatorio en el input de lo contrario no se podrá enviar el formulario.

Tambien existen varias opciones de autocompletado que se pueden utilizar en los formularios, en la pagina de **[MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/autocomplete)**.

## 11. **`Etiqueta <select> y <option> (Con buenas y malas practicas) para las listas desplegables en formularios`**

```html
<!-- Select con malas practicas -->

<select>
    <option value="JavaScript">JavaScript</option>
    <option value="Python">Python</option>
    <option value="Java">Java</option>
    <option value="C++">C++</option>
</select>

<!-- Select con buenas practicas "SIN NECESIDAD DE HACER SCROLL INFINTO" -->

<input list="lenguajes" name="lenguajes" id="lenguajes" />
<datalist id="lenguajes">
    <option value="JavaScript"></option>
    <hr>
    <option value="Python"></option>
    <hr>
    <option value="Java"></option>
    <hr>
    <option value="C++"></option>
    <hr>
</datalist>
```

**DESCRICIÓN DE LAS ETIQUETAS DE SELECT Y OPTION**

- **`select`**: Es una etiqueta que nos permite para crear **listas desplegables** en el formulario.

- **`option`**: Es una etiqueta que nos permite colocar opciones en el select.
  
  - **`value`**: Son los valores que se van a enviar al backend 	 
  
  - **`hr`**: Es una etiqueta que nos permite colocar una linea horizontal como divisor de las opciones del select.

- **`value`**: Es un atributo que se usa para especificar que se va a usar una **lista desplegable**

- **`datalist`**: Es una etiqueta que nos permite rear listas desplegables en HTML para evitar el scroll infinito

## 12. **`Atributo type="submit" y button en los formularios`**

En HTML se pueden crear dos tipos de botones en los formularios, uno es el **`<input type="submit">`** y el otro es el **`<button>`**.

```html
<main>
    <input type="submit" value="Nombre" />
    <button>Enviar</button>
</main>
```

El uso correcto de los botones es:

- **`submit">`**: Se usa para enviar el formulario.

  - **`value`**: Es un atributo que nos permite colocar un texto en el botón.	 

- **`button`**: Se usa para otro tipo de acciones en la estructura de la página web.