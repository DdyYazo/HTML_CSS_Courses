
<div align="center">

# **CSS Concepts and Fundaments**


<p align="center">
  <img src="https://i.postimg.cc/xCMNj95T/imagen-2024-06-14-175959797.png" alt="Aquí va el texto del enlace" width="500">
</p>


</div>

# **Tabla de contenido**
- [**CSS Concepts and Fundaments**](#css-concepts-and-fundaments)
- [**Tabla de contenido**](#tabla-de-contenido)
- [1. **Hoja de trucos de CSS y recursos**](#1-hoja-de-trucos-de-css-y-recursos)
  - [Paginas para practicar `Flexbox` y `CSS Grid`](#paginas-para-practicar-flexbox-y-css-grid)
- [2. **Formas de dar estilos a un etiqueta html con el `elemento`, `class` o `id`**](#2-formas-de-dar-estilos-a-un-etiqueta-html-con-el-elemento-class-o-id)
  - [2.1. Diferencia entre elemento, `class` y `id`](#21-diferencia-entre-elemento-class-y-id)
  - [3. `Pseudo-clases` y `Pseudo-elementos` y la efectividad de la metodologÍa de `BEM`](#3-pseudo-clases-y-pseudo-elementos-y-la-efectividad-de-la-metodología-de-bem)
    - [Diferencias entre Pseudo-clases y Pseudo-elementos](#diferencias-entre-pseudo-clases-y-pseudo-elementos)

# 1. **Hoja de trucos de CSS y recursos**
<p align="center">
  <a href="https://htmlcheatsheet.com/css/">
    <img src="https://i.postimg.cc/pXVG5w9X/imagen-2024-02-05-150922143.png" alt="Aquí va el texto del enlace">
  </a>
</p>


## Paginas para practicar `Flexbox` y `CSS Grid`
|Flexbox Froggy | Grid Garden |
|:---------:|:---------:|
|[![Aquí va el texto del enlace](https://i.postimg.cc/xdbJx1Zj/imagen-2024-02-05-151723690.png)](https://flexboxfroggy.com/#es) |[![Aquí va el texto del enlace](https://i.postimg.cc/zDs3PNr0/imagen-2024-02-05-151829227.png)](https://cssgridgarden.com/#es)|



# 2. **Formas de dar estilos a un etiqueta html con el `elemento`, `class` o `id`**

## 2.1. Diferencia entre elemento, `class` y `id`
- El elemento se aplica a todos los elementos de ese tipo siendo la menos practica
- La `class` se aplica a todos los elementos que tengan esa clase
- El `id` se aplica a un solo elemento 

**Por lo tanto la mas recomendada es la `class`**



## 3. `Pseudo-clases` y `Pseudo-elementos` y la efectividad de la metodologÍa de `BEM`

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

