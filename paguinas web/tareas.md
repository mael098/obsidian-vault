### Estructura de un Documento HTML y sus Etiquetas en Markdown (Obsidian)

markdown

Copy code

``# Estructura de un Documento HTML y sus Etiquetas  ## 1. Estructura Básica de un Documento HTML  Un documento HTML típico comienza con una declaración de tipo de documento (`<!DOCTYPE html>`) y está compuesto por las siguientes partes principales:  ```html <!DOCTYPE html> <html>   <head>     <title>Título de la Página</title>   </head>   <body>     <h1>Encabezado Principal</h1>     <p>Este es un párrafo.</p>   </body> </html>``

## 2. Etiquetas Principales

1. `<!DOCTYPE html>`: Esta declaración define el tipo de documento y la versión de HTML que se está utilizando. En HTML5, se usa simplemente `<!DOCTYPE html>`.
    
2. `<html>`: La etiqueta `<html>` representa la raíz del documento HTML. Todos los demás elementos deben ser descendientes de esta etiqueta.
    
3. `<head>`: La etiqueta `<head>` contiene metadatos sobre el documento, como el título, enlaces a hojas de estilo, y metaetiquetas.
    
    - `<title>`: Define el título de la página que aparece en la pestaña del navegador.
    - `<meta>`: Proporciona metadatos como la codificación de caracteres (`<meta charset="UTF-8">`).
    - `<link>`: Vincula recursos externos como hojas de estilo (`<link rel="stylesheet" href="styles.css">`).
    - `<style>`: Contiene estilos CSS internos.
4. `<body>`: La etiqueta `<body>` contiene el contenido visible de la página web, como texto, imágenes, enlaces, etc.
    

## 3. Etiquetas de Contenido

- **Encabezados**: Utilizados para definir títulos y subtítulos.
    
    - `<h1>` a `<h6>`: Los encabezados de nivel 1 a nivel 6, siendo `<h1>` el más importante y `<h6>` el menos importante.
- **Párrafos**:
    
    - `<p>`: Define un párrafo de texto.
- **Enlaces**:
    
    - `<a href="url">`: Define un hipervínculo. El atributo `href` especifica la URL del enlace.
- **Imágenes**:
    
    - `<img src="url" alt="texto alternativo">`: Inserta una imagen. El atributo `src` define la ruta de la imagen y `alt` proporciona un texto alternativo.
- **Listas**:
    
    - `<ul>`: Define una lista no ordenada.
    - `<ol>`: Define una lista ordenada.
    - `<li>`: Define un elemento de lista.
- **Tablas**:
    
    - `<table>`: Define una tabla.
    - `<tr>`: Define una fila de tabla.
    - `<td>`: Define una celda de tabla.
    - `<th>`: Define una celda de encabezado en una tabla.

## 4. Etiquetas de Formulario

- `<form>`: Define un formulario HTML para la entrada del usuario.
- `<input>`: Define un control de entrada en un formulario.
    - Tipos de entrada comunes incluyen `text`, `password`, `submit`, `radio`, `checkbox`, etc.
- `<label>`: Etiqueta para un elemento `<input>`.
- `<textarea>`: Define un área de texto multilínea.
- `<button>`: Define un botón.

## 5. Etiquetas de Estilo y Script

- `<style>`: Contiene reglas CSS para aplicar estilos a los elementos HTML.
- `<script>`: Define un script client-side (generalmente JavaScript).

## 6. Comentarios

Los comentarios en HTML se escriben entre `<!--` y `-->`. No se muestran en el navegador.

html

Copy code

`<!-- Este es un comentario -->`

## Ejemplo Completo

html



```html

<html>   <head>     <meta charset="UTF-8">     <title>Mi Página Web</title>     <link rel="stylesheet" href="styles.css">   </head>   <body>     <header>       <h1>Bienvenidos a Mi Página Web</h1>       <nav>         <ul>           <li><a href="#home">Inicio</a></li>           <li><a href="#about">Acerca de</a></li>           <li><a href="#contact">Contacto</a></li>         </ul>       </nav>     </header>     <main>       <section id="home">         <h2>Inicio</h2>         <p>Este es el contenido de la sección de inicio.</p>       </section>       <section id="about">         <h2>Acerca de</h2>         <p>Este es el contenido de la sección acerca de.</p>       </section>       <section id="contact">         <h2>Contacto</h2>         <form action="submit_form.php" method="post">           <label for="name">Nombre:</label>           <input type="text" id="name" name="name">           <label for="email">Correo Electrónico:</label>           <input type="email" id="email" name="email">           <button type="submit">Enviar</button>         </form>       </section>     </main>     <footer>       <p>&copy; 2024 Mi Página Web. Todos los derechos reservados.</p>     </footer>   </body> </html>`
```

Este ejemplo muestra una página HTML completa con una estructura básica, encabezados, párrafos, enlaces, una imagen, una lista, una tabla y un formulario. Cada etiqueta tiene un propósito específico que ayuda a definir la estructura y el contenido del documento HTML.




