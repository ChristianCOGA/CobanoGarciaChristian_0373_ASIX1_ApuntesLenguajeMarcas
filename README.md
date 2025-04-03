# LENGUAJE DE MARCAS - ASIX 0373
## INDICE
- [GITHUB](#github)
- [MARKDOWN](#markdown)
- [HTML](#html)
- [CSS](#css)
## GITHUB
### - ¿Que és **GITHUB**?
- Portal creado para alojar el código de las aplicaciones de cualquier desarrollador que usaremos especifícamente para crear nuestros Repositorios. Estos los tendremos en la nube o *GitHub* los cuales podremos ir copiando y bajando copias a nuestros dispositivos locales así como a la inversa subir las modificaciones hechas en local hacia la nube gracias al *CMD* o a las herramientas de *GitHub*.
- Cada modificación de dicho Repositorio lo llamaremos **Commit**.
- Tenemos la posibilidad de alternar en que sean públicos o privados nuestros Repositorios.
  - Como puntualización, decir que aunque estén en público nuestros Repositorios, siendo estos tomados por su **URL** podrán como mucho copiarlos y modificarlos por su cuenta pero nunca modificar nuestro Repositorio.

##

### - Crear cuenta en GITHUB
-En la página de *GitHub* nos registraremos para permitirnos crear repositorios o colaborar en proyectos ajenos.

##

### - Repositorios
#### ¿Qué es un Repositorio?
Es un lugar o archivo donde puedes almacenar el código, los archivos y el historial de revisiones de cada archivo. Los repositorios pueden contar con múltiples colaboradores y pueden ser públicos como privados.

 Antes de empezar a trabajar en nuestro dispositivo local, deberemos tener en cuenta una serie de comandos de trabajo en **CMD** cada uno con una función específica: 
  - ``git init`` para inicializar el repositorio en nuestro dispositivo local.
  - ``git branch -m "rama"`` para cambiar entre ramas del repositorio. Podemos visualizar las ramas de nuestro repositorio con el comando ``gir branch`` .
  - ``git add + "nombre del archivo"`` para añadir el archivo seleccionado al área intermedia antes de ser subido en nuestro **commit**. Tenemos otro comando ``git add .`` para directamente subir todos los archivos.
  - ``git commit -m + "mensaje/nombre del commit" `` para guardar los cambios que subiremos a posteriori, resepresentara en *GitHub* una actualización del archivo.
  - ``git push origin main`` para enviar el **commit** desde la rama *origen* desde la que trabajamos a la *main* en *GitHub*.
  -  ``git remote add origin + URL`` para clonar un repositorio ajeno o remoto a nuestro dispositivo local.

Ahora si crearemos nuestro repositorio en *GitHub* y nos aseguraremos de copiar la **URL** para poder clonarlo en nuestro sistema.
- En la pestaña **New** crearemos el repositorio.

![Foto03](./Imagenes/Apuntes004.jpg)
- Nombraremos el repositorio y lo pondremos en público o privado según preferencia.

![Foto01](./Imagenes/Apuntes001.jpg)
- Copiaremos el link del repositorio para añadirlo a nuestro dispositivo local.

![Foto02](./Imagenes/Apuntes002.jpg)

- Ahora tendremos que clonarlo en nuestro dispositivo local con el comando:  

![Foto03](./Imagenes/Apuntes003.jpg)

Con esto ya podriamos trabajar en local e ir subiendo **commits** según avancemos en nuetsro proyecto para no perder el avance.

<!--Hasta aquí GUTHUB-->

## [MARKDOWN](#indice)
Es un lenguaje de marcado ligero creado por **John Gruber** y **Aaron Swartz** que trata de conseguir la máxima legibilidad y facilidad con la aplicación de formato a un texto empleando una serrie de caracteres de una forma especial.

Para poder mostrar nuestro texto de manera organizada como hemos estado viendo en el primer apartado explicaremos los diferentes caracteres y sus aplicaciones:

### - Encabezado
Estos se se diferenciarán según la cantidad de ``##`` que pongamos, es decir, los podremos dividir en subniveles o títulos y subtítulos:
# Título 1
## Título 2
### Título 3
Empleando la siguiente nomenclatura:
```
    # Título 1
    ## Título 2
    ### Título 3 
``` 
##

### - **Negrita** y *Cursiva*
Como se ve en el encabezado, la nomenclatura a seguir será la siguiente:
```
    Negrita : **negrita**
    Cursiva : _cursiva_
```
Comentar que será indiferente que usemos ``*`` o ``
_`` para indicar que sea en negrita o cursiva, se tienen en cuenta la cantidad de caracteres que se escriben para indicar como queremos que se vea la palabra si en **negrita** o **cursiva**.

Añadir que si queremos que sea ambas a la vez, deberemos usar 3 caracteres a cada lado. Palabra en ***cursiva y negrita***
```
    Negrita y cursiva : ***Palabra*** // ___Palabra___
```
##

### - Listas
Comprende el formato en que se harían las listas en cualquier procesador de texto, ya sea con guión o con numerales:
1. Primero
2. Segundo
3. Tercero
- Título 1
- Título 2
- Título 3

##

### - Mostar código
La nomenclatura que usaremos pra mostrar el código es mediante el uso de ``` `` ``` y dentro del espacio generado, insertaremos el código que querramos, por ejemplo:
```
    ```
        <!DOCTYPE html>
        <html>
            <body>

            <h1>My first PHP page</h1>

            <?php
            echo "Hello World!";
            ?>

            </body>
        </html>
    ```
```

##

### - Enlaces
Enlazar una página web en nuestro repositorio se hace de la siguiente manera, copiamos la dirección web y insertaremos la siguiente línea:

```
    [Nombre X](link a la página web // URL)
```

Como ejemplo el link de abajo a la página padre de todos los hobbys.

[Warhammer](https://www.warhammer.com/es-ES/home)

##

### - Imagenes
Para seleccionar y enseñar una imagen es tan sencillo como descargarla y ubicarla en la carpeta del repositorio donde trabajamos de manera local y inscribir una nomenclatura similar a la de enlace con la siguiente línea:

```
    ![Nombre X](nombre de la imagen o ubicación + "Título opcional de la imagen)
```

![Emperador](./Imagenes/Emperador.jpg "Warhammer mola")

##

### - Tablas
 Para la creación de tablas debemos seguir una nomeclatura y orden específico.
 - Crearemos los títulos:
  ```
    |Título 1|Título 2|Título 3|
  ```
- Definiremos los caracteres que podremos escribir en cada columna con el límite de ``-`` que le indiquemos.
- Así mismo también podemos indicar hacía que parte de la tabla queremos que se orienten los campos a rellenar con ``:``.
 ``` 
    |Título 1|Título 2|Título 3|
    |----------|------|----------|
    |:---------|:----:|---------:|
 ``` 
- Quedando como resultado una tabla como la siguiente que por dedecto nos devuelve la tabla con efecto visual **Zebra Stripes**.
    |Capítulo |Unidades|Origen|
    |:---------|:----:|---------:|
    |Templarios Negros|500|Terra|
    |Ultramarines|1500|Ultramar|

<!--Hasta aquí MARKDOWN-->

## [HTML](#indice)
### - ¿Qué es HTML?
**HTML** o **HyerText Markup Lenguage** es el lenguaje de marcas mas importante de internet, siendo este la base de poder visualizar contenido en un navegador web.

Creado por **Tim Berners-Lee**, **HTML** define la estructura y el contenido de los diferentes archivos multimedia mediante **etiquetas**.
Destacando también por la facilidad que ofrece este lenguaje para ser usado y aprendido, de ahí que se haya estandarizado su uso en un procentaje muy elevado de páginas web.

##

### - Estructura del código de HTML
Los documentos **HTML** tienen una estructura inicial común, es decir, todo el contenido va dentro de dicha arquitectura de código.
```
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <tittle>Document</tittle>
    </head>
    <body>

    </body>
    </html>    
```
Desgranando que significa cada nomenclatura sería de la siguiente manera:
- ``<!DOCTYPE html>`` : Define el formato de documento en este caso **HTML5**
- ``<html></html>`` : Contiene el contenido principal del documento **HTML**.
- ``<head></head>`` : Provee información general **(metadatos)** acerca del documento, incluyendo su título, enlaces a scripts y hojas de estilos.
  - ``<meta></meta>`` :  **Metainformación**, sirve para aportar información sobre el documento..
  - ``<tittle></tittle>`` : Define el título que tendra la página web en la pestaña de navegación.
- ``<body></body>`` : Contiene el cuerpo de nuestro documento con todos los archivos que incluyamos en el, visible en la página web.

##

### - Etiquetas de HTML 
Los "tags" HTML, o "etiquetas" HTML, son códigos utilizados para "marcar" el texto de una página web, con el fin de dar instrucciones al navegador sobre cómo mostrarlo.

Tenemos varias posibilidades destacando los más usados:
- ``<h1> ... <h6>`` : Según el número de encabezado que le demos, tendrá mas prioridad o mayor tamaño que los demás.
- ``<p> </p>`` : Con estas etiquetas HTML puedes indicar dónde empieza y termina cada párrafo de texto.
- ``<strong> </strong>`` : Para poner en negrita las palabras dentro de la etiqueta. ``<strong> Palabara X </strong>`` : <strong>Palabra X </strong>.
- ``<em></em>`` : Para escribir en cursiva las palabras dentro de la etiqueta. ``<em> Palabra Y</em>`` : <em>Palabra Y</em>.
- ``<u></u>`` : Para escribir en cursiva las palabras dentro de la etiqueta. ``<u> Palabra Z</u>`` : <u>Palabra Z</u>.
- ``<br>`` : Para ejecutar cambios de línea.
- ``<hr>`` : Para subrayar o delinear entre parrafos con una línea divisoria.
- ``<ul></ul>`` : Si necesitas agregar una lista que solo tendrá viñetas, es decir, que no tiene que enumerarse.
- ``<ol></ol>`` : En cambio, si quieres que los elementos de la lista aparezcan enumerados en orden ascendente.
- ``<li></li>`` : En contexto con el ejemplo anterior, cada uno de los elementos de una lista debe escribirse con una etiqueta especial, no importa si serán numerados o no.
- ``<a></a>`` : Para agregar hipervínculos que llevan a otros documentos o páginas web que indiquemos.
- ``<img></img>`` : Para incluir imágenes en tu documento.
  
Estas etiquetas pueden dividirse en **Elementos de bloque** : Necesidad de una líena para poder ejecutarse. O por el contrario en **Elementos de línea** que son etiquetas que se pueden ejecutar en una misma línea detras de otro bloque.

##

### - Rutas
Para poder movernos y saber donde buscar el nuestros archivos multimedia o enlaces tendremos dos opciones : 
- **Ruta Absoluta** : Para certicificar la ruta a seguir al pie de la letra del archivo a buscar. Útil para trabajo entre servidores o diferentes ubicaciones con menos propenciones a errores de ruta.
- **Ruta Relativa** : Conexión o ruta que se hace en relación con el archivo actual. Práctico para trabajo local en un mismo dispositivo o proyectos pequeños.

##

### - Imagenes
Para insertar imagenes deberemos usar uno de los comandos antes mostrados ``<img> + src`` el cual específica que cargaremos una imagen y con ``src`` de donde procede.
- ``<img src="./Imagenes/Emperador.jpg" width="250" height="350">``

<img src="./Imagenes/Emperador.jpg" width="250" height="350">

Como podemos observar además de indicar la fuente de la imagen, podemos modificar párametros de tamaño con las etiquetas ``width`` y ``height``.

##

### - Enlaces
De igual manera que hemos visto con la imagen, haremos uso de otros comandos para poder enlazar nuestro documento, bien con otra sección del mismo o con una página web externa, tal y como veremos en el siguiente ejemplo:

- ``<a href="https://www.warhammer.com/es-ES/home"> Visita la página del Emperador </a>``
  
<a href="https://www.warhammer.com/es-ES/home"> Visita la página del Emperador </a>

##

### - Validador de HTML 

Página web que nos verifica y indica los errores que hemos podidio cometer a la hora de escriir la sintaxis o las nomenlcaturas de nuestro documento **HTML**.

Siguiendo los estándares establecidos por el **World Web Consortium**.

Enlace : <a href="https://validator.w3.org/">Validador HTML</a>

##

### - Elementos semánticos HTML5

Es crucial saber usar contenedores de información que indiquen que tipo de elemento estructural contienen, como por ejemplo:
- ``<footer>`` : Pie de página.
- ``<header>`` : Encabezado.
- ``<article>`` : Donde va el contenido del artículo.
- ``<section>`` : Sección de información de la página.
- ``<nav>`` : Proporcionar enlaces de navegación.
- ``<figure>`` : Representa contenido independiente, a menudo con un título.

##

### - Formularios y sus etiquetas
Los formularios nos sirven para interactuar con el usuario y que esta pueda transmitirnos información.

- ``<form></fomr>`` : Se uutiliza para la creación de formularios de interacción con el usuario, todo aquello dentro de esta sección será parte del mismo.
- ``<input></input>`` : Utilizado para crear diversos tipos de campos interactivos con el formulario. Siendo estos campos de diferentes tipos de atributos:
  - ``type`` : Define el tipo de entrada que se debe mostrar.
  - ``id`` : Identificador único para el campo, puede asociarse con un elemento que veremos más adelante; ``<label>``.
  - ``name`` : Nombre del campo de entrada.
  - ``value`` : Valor predeterminado del campo de entrada.
  - ``placeholder`` : Texto que aparece el campo cuando está vacío, ofrce pista de que dato debe introducir el usuario.
  - ``disabled`` : Para desactivar un campo evitando interacción del usuario.
- ``<label>`` : Se usa para proporcionar una etiqueta o descripción para un elemento de formulario.
- - ``<fieldset></fieldset>`` : Nos permie agrupar las ocpiones del formulario de manera ordenada en un recuadro con un nombre de encabezado para el.

Un ejemplo de como emplear las etiquetas mostradas: 
```
    <form action = "recepcion.png" method = "GET"> 
        <label for = "nombre">Nombre :</label>
        <input type = "text" id ="nombre" name ="nombre" placeholder ="Introduce tu nombre"><br><br>
        <label for = "password" >Contraseña :</label>
        <input type = "password" id ="password" name ="password" placeholder ="Introduce tu contraseña"><br><br>
    </form>
```
Dando como resultado el formulario pidiendo **Nombre** y **Contraseña** al usuario.

![Foto05](./Imagenes/Apuntes005.jpg)

De la siguiente manera podriamos pedir que nos aporte el usuario la información de la manera en que categorizemos el atributo ``type`` como en el siguiente ejemplo, donde pediremos una selección de opciones y no rellenar datos:
```
    <form
        <fieldset>
            <legend>Idioma</legend>
            <input type = "radio" id="idioma" name = "idioma" value = "castellano">
            <label for = "castellano">Castellano</label>

            <input type = "radio" id="idioma" name = "idioma" value = "catalan">
            <label for = "catalan">Catalán</label>

            <input type = "radio" id="idioma" name = "idioma" value = "chino">
            <label for = "chino">Chino</label> 
        </fieldset>
    </form>    
```
![Foto06](./Imagenes/Apuntes006.jpg)

Ahora mostraremos ``<select></select>`` cuya función consiste en desplegar una pestaña de opciones a elegir para el usuario en el formulario que le proporcionamos, de la siguiente manera:
```
<form>
    <label for="ciudad">Ciudad</label>
        <select id="ciudad" name="ciudad">
            <option value=""disabled>Seleccione una ciudad</option>
            <option value="Barcelona">Barcelona</option>
            <option value="Madrid">Madrid</option>
            <option value="Valencia ">Valencia</option>
            <option value="Sevilla">Sevilla</option>
            <option value="Murcia">Murcia</option>
        </select>
</form>   
```

Estas línes de código nos permiten hacer uso del siguiente desplegable, dando varias opciones de elección gracias a la etiqueta ``<select>`` con sus diferentes opciones usando la etiqueta ``option`` más el atributo 

![Foto07](./Imagenes/Apuntes007.jpg)

Para terminar esta sección de formularios, hablaremos de la etiqueta ``<button>`` que se usa para crear botones interactivos para el usuario en el formulario o una página web. Por ejemplo:
```
    <button type="submit"> Enviar datos</button>
```
Dando la línea de código mostrada el siguiente resultado de interacción.
![Foto08](./Imagenes/Apuntes008.jpg)

## Tablas

Todo dentro de un formato ``<table></table>`` , este tendrá dos atributos a rellenar o definir : ``border`` y ``width``. Ojo de poner ``width = 100%``.

Filas serán llamadas  = **row**
Las columnas serán llamadas  = **col**

Una tabala puede dos partes, una primera parte llamada encabezado **Heater** : ``<thead></thead>`` y una segunda parte llamada pie o **Footer** acabando con un cierre o pie de página **Footer**.

``<tr> </tr>`` : Define una fila en la parte de la tabla. El atributo ``align`` junto al ``<tr>`` permite alinearlo donde le indiquemos.
``<td> </td>`` : Definimos las celdas de una fila.
``<th> </th>`` : Define a nivel semántico que estas celdas pertenecen a un encabezado, diferenciandolas de otras celdas. // Esto sirve también para el encabeado de pie o **Footer**.

``bgcolor`` : Para cambiar el color de fondo del elemento seleccionado. Definidos por su código hexadecimal RGB *(Red/Green/Blue)* valores que oscilan entre 0 - 255, **HTML** de por si ya detecta los colores básicos,

``colspan`` : Permtie cambiar los párametros de la celda de manerea horizontal, para permitirle ocupar dos celdas o las que dictemos en vez de una.

``rowspan`` : Permite cambiar los párametros de la celda de manera vertical, para permitirle ocupar dos celdas o las que dictemos en vez de una.

Para ambos atributos debemos eliminar la celda que vamos a ocupar de más.

## [CCS](#css)

## Evolución y función

**CSS (Cascading Style Sheets)** surge para separar el contenido de una web (HTML) de su presentación visual.

Antes, **HTML** asumía tanto la estructura como el diseño de las páginas web.
**CSS** se introduce para evitar esto, permitiendo aplicar estilos sin modificar el contenido.

## Ventajas e inconvenientes

**Ventajas:**

-   Facilita el mantenimiento del código.
-   Más potente y flexible que las etiquetas de estilo HTML.
-   Sencillo de aprender.
-   Permite definir estilos distintos para impresión y pantalla.
-   Se puede reutilizar desde distintos documentos.

**Inconvenientes:**

-   No todos los navegadores interpretan CSS igual.
-   Requiere crear hojas de estilo diferentes para algunos navegadores.

## Ubicación del CSS

**Inline (en la misma etiqueta HTML):**

``<p style="text-align:center; color:red">Texto centrado y rojo</p>``

**Interno (en la cabecera del documento):**
```
<head>
    <style>
        p 
        {
            text-align: center;
            color: red;
        }
    </style>
</head>
```
**Externo ``styles.css``:**

Primeramente crearemos dos archivos diferentes , siendo uno el **HTML** como **index.html** y otro archivo **CSS** como **style.css**.

**HTML ``index.html``:**
```
<head>
    <link rel="stylesheet" href="estils.css" type="text/css">
</head>
```

**CSS ``styles.css``:**
```
p 
{
    text-align: center;
    color: red;
}
```
## Prioridad del CSS

Si hay varios estilos aplicados al mismo elemento la prioridad se organiza de tal manera que el estilo aplicado más cercano al elemento al que hace efecto es el que tiene prioridad por encima de los demas excepto por una excepción:

-   Inline (más prioridad).
-   Interno.
-   Externo.
-   El orden dentro del mismo CSS también importa (lo último sobrescribe lo anterior).
-   Por Herencia que seria el de menos prioridad.
-   Excepcion de ``!important`` que sobrescribe todo.


### Sintaxis básica

**Una regla CSS está compuesta por:**

-   **Selector:** A qué elemento se aplica, ``p``.

-   **Declaraciones:** Propiedad + valor, ``font-size_ 10px;``.

    Por ejemplo:
```
p 
{
    font-size: 10px;
    background-color: gray;
}
```
-   **Comentarios**: Se usan para añadir notas que el navegador ignora.

``/* Esto es un comentario */``

-   **Agrupar selectores:** En lugar de escribir reglas duplicadas, las agrupamos en única declaración:
```
h1, p 
{
    color: red;
}
```
**Tipos de selectores**

-   **Básicos:**

    - Selector de elementos ``p``, ``h1``.
    - Selector de ID ``#id``.
    - Selector de clase ``.clase``.

-   **Avanzados:**

    - Selector universal ``*``.
    - Selectores de atributos ``[type="text"]``.
    - Selectores de hijos ``>``.
    - Selectores de descendientes ``espacio``.
    - Hermanos adyacentes ``+``.
    - Pseudoclases ``:hover``.
    - Pseudoelementos ``::before``.

**Selector de elementos (selector de tipo):**

Este selector aplica un estilo a todos los elementos del tipo indicado. Como por ejemplo:

``Afecta a todos los enlaces <a>``
```
a 
{
    color: red;
}
```

**Selector de ID**

Este selector afecta al elemento que tenga un id específico. Solo puede haber un elemento por ID para cada elemento, dado que es un elemento identificador único. Como por ejemplo:

``<p id="example">Texto con ID</p>``
```
#example 
{
    property: value;
    property2: value2;
}
```

**Selector de clase**

Este selector se aplica a todos los elementos con la misma clase. Como por ejemplo:

``<p class="example">Texto</p>``

``<li class="example">Elemento</li>``

``<div class="example">Contenedor</div>``

```
.example 
{
    property: value;
    property2: value2;
}
```

### Selectores Avanzados de CSS