# Bitácora personal

## Clase 06

### De figma al navegador 
- HTML / CSS
- Estructura semántica
- Estilos CSS
- Asistencia de IA
- CSS + DevTools
- Estados interactivos

### visual studio code
- editor de código -- herramienta para escribir texto plano, resalta sintaxis y ayuda a detectar errores
- github -- plataforma en la nube para guardar, compartir y editar códigos permitiendo el trabajo de forma colaborativa

### HTML5
- documento que lee el navegador, escrito en un lenguaje de etiquetas llamado HTML (hyper text markup languaje), introducir información de forma semántica, todo lo visual se gestiona en lenguaje css
  
**detrás de un sitio web**
- html -- estructura -- define que elementos existen: título, imagen, botón 
- css -- estilo -- apariencia visual: tipografía, color, espaciado
- javascript -- comportamiento -- interactividad: cambios con un clic, botones que responden

**¿Cómo componer etiqueta?**

```
etiqueta apertura <p> contenido <p> etiqueta de cierre

```
- etiqueta siempre en minúscula, el contenido si se puede con mayúsculas 
### GitHub

**2FA** 

descargar recovery codes al activarla 2FA -- guardar en lugar seguro 

- acceder a la configuración de seguridad: clic foto de perfil -- settings --password and authentication
- iniciar activación 2FA: sección two factor authentication -- clic botón enable two factor authentication
- vincular una aplicación: seleccionar github mobile

### Hacks HTML
```cpp
<h1>Título</h1>
<p>Párrafo</p>}
<strong>Bold</strong>
<a href="link">Ver el link</a>
<ul> //para reconocer el listado 
// ol es lista enumerada
-  <li>Lista</li>
-  <li>Lista</li>
-  <li>Lista</li>
<ul/>
<img src="nombre imagen. formato"alt="descrpción imagen">
<etiqueta id="descripción" -- sirve después para los links
!<--comentar-->
! + enter (código html predeterminado)
<a href=#contexto">Contexto</a></li> -- para ir como a un link directo dentro de la página web, realizarlo en la lista
```

## Clase 07

### Estructura HTML general
```
<html>
<head> -- metadatos
</head>
<body>
</body>
</html>
```
### Body
```
<body>
<header>
</header>
<main> -- parte importante de la página
</main>
<footer> -- permanentemente abajo, contacto, dirección, teléfono 
</footer>
</body>
```
### CSS
- Cascading Style Sheets
- controlar apariencia de los elementos de una página web (color, fondo, tipografía, espaciado, bordes, disposición)
---
**todo es una caja**
- Content (contenido): el texto o la imagen, su tamaño se controla con width y height.

- Padding (relleno): espacio interior entre el contenido y el borde, toma el color de fondo de la caja.

- Border (borde): la línea que rodea la caja, se define con grosor, estilo y color: border: 2px solid #2F3C7E;.

- Margin (margen): espacio exterior que separa la caja de las demás. Es transparente.

### Funcionamiento 
```
**
p{
color (propiedad):red (valor);
}

un elemento, varias propiedades
p{
color: red;
font-size: 1rem;
}

varios elementos, misma propiedad
p,
h1{
color: red;
}
```
### Hacks css
```
<link rel="stylesheet href="style.css"> -- ponerlo en el index html -- head (para aplicar css)
/* comentario */
rem -- 3rem (todos los lados) 3rem 2rem (arriba y abajo) (lados)
* al principio para aplicar en toda la página
si quiero destacar una frase dentro de un párrafo realizar clase + propiedad -- ej: strong

si quiero modificar un texto solamente

css .nombreclase {
     font-size:
     color:

html
<p class= "nombre clase";

margin: 0; -- elimina márgenes que trae por defecto
font-family: fuente principal
color: texto general fuente
background: #000000 fondo navegación
img { max-width: 100%; } -- impide que una imagen sobrepase el contenedor "padre"
div -- bloques de contenido

header { ... }
max-width: 75rem;: ancho máximo para el contenedor del encabezado 
margin: 0 auto;: centra horizontalmente la caja en la pantalla
padding: 3rem 2rem;: Agrega espacio interno (arriba/abajo: 3rem, lados: 2rem)
border-bottom: 4px solid rgb(196, 111, 7);: pinta una línea divisoria inferior


footer -- parte de abajo final
```

**REM**
- unidad medida relativa -- equivale al tamaño de fuente del elemento raís (html)
- 1 rem = 1 vez el tamaño de fuente raíz

### Código final página
```
/* Basico */
* {
    box-sizing: border-box; /*el ancho incluye padding y borde*/
}

body {
    margin: 0;
    .bree-serif-regular 
  font-family: "Bree Serif", serif;
  font-weight: 400;
  font-style: normal;
  color: #000000;
  background: #E6E6E6;
}

img {
    max-width: 100%;
}

/* Header */

header {
    max-width: 60rem;
    margin: 0 auto;
    padding: 3rem 2rem;
    border-bottom: 4px solid #996F38;
}

h1 {
    margin: 0;
    font-size: 2.5rem;
}

.autor {
    font-size: 1.2rem;
    color: #996F38;
}

/* main (contenido principal) */

main {
    max-width: 60rem;
    margin: 0 auto;
    padding: 3rem 2rem;
}

div {
    margin: 0 0 2rem;
    padding: 1rem;
    background: white;
    border: 1px solid #996F38;
}

section {
    padding: 1.5rem 2rem;
    margin-bottom: 1.5rem;
    background: white;
    border: 1px solid #996F38;
}

h2 {
    margin: 0;
    font-size: 1.5rem;
}

.destacado {
    background: #EDCA93;
    padding: 1rem;
}

.button {
    margin-top: 1;
    padding: 0.75rem 1.5rem;
    background: #996F38;
    color: white;
    font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
    text-decoration: none;
}

footer {
    max-width: 60rem;
    margin: 0 auto;
    padding: 3rem 2rem;
}
```  
## Clase 08

### Propiedad display
- cada etiqueta es una caja
- comportamiento por defecto
- nunca usar imágenes tan pequeñas -- 1200-1600px min

### Block
- ocupa todo el ancho y empieza en una línea nueva
```display: block;```

### Inline
- ocupa solo su contenido y fluye con el texto
```display: inline;```

### Inline block
- fluye pero acepta pading y tamaño
```display: inline-block;```

### None 
- desaparece
```display: none;```

---

## Flex box
```
display: flex;
```
- cambia como se ordenan sus hijos
- grilla -- contenedor
- tarjeta -- hijos
```
  .grilla {
display: flex;
}
```
### Flex direction
- **row:** por defecto
```
  .grilla {
display: flex;
flex-direction: row;
}
```
- **column**
```
  .grilla {
display: flex;
flex-direction: column;
}
```
---
- **dos ejes**
1. eje cruzado: align-items
2. eje principal: justify-content
3. repartir el ancho y pasar a otra línea -- entre hijos
```
.grilla {
display: flex;
justify-content: space-between;
align-items: center;
gap: 1.5rem;
}
```
 4. cuando sobra espacio -- se reparten en partes iguales
```
.tarjeta {
flex: 1;
min-width: 12rem; /* ninguna se achica bajo 12rem */
}
```
 5. cuando falta espacio -- pasan a la siguiente línea
```
.grilla {
display: flex;
flex-wrap: wrap;
gap: 1.5rem;
}
```
---
- **justify content:** reparte en el eje principal
  
1. flex-start -- inicio
```     
.grilla {
display: flex;
justify-content: flex-start;
}
```
  2. center -- centro
```
.grilla {
display: flex;
justify-content: center;
}
```
  3. space-between -- uno en cada extremo
```
.grilla {
display: flex;
justify-content: space-between;
}
```
---
- **align-items:** alinea en el eje cruzado
  
1.  stretch -- estiran por defecto
```
.grilla {
display: flex;
justify-content: space-between;
align-items: stretch;
}
```
  2. flex-start -- arriba
```
.grilla {
display: flex;
justify-content: space-between;
align-items: flex-start;
}
```
  3. center -- centro
```
.grilla {
display: flex;
justify-content: space-between;
align-items: center;
}
```


---
## Botones 

### <a> 
- padding vertical se monta sobre las líneas vecinas
```
.boton {
display: inline-block;
padding: 0.75rem 1.5rem;
}
```
### <button> 
- fluye en la línea, pero respeta su padding 
```
button {
padding: 0.75rem 1.5rem;
}
```

## Imágenes
- por defecto queda queda alineada
  
### block + margin auto
- baja a su propia y el margen se reparte a los lados
```
img {
display: block;
max-width: 100%;
height: auto;
}
```
### fill
- estira y deforma por defecto
### contain
cabe completa y deja espacios
### cover 
llena la caja, sin perder proporción

## Pasos
Contenedor display: flex; 

Dirección flex-direction: row | column;

Alinear justify-content x align-itemns

Separar gap: 1.5rem;

Repartir flex: 1; (en los hijos)

## Proceso
● ¿Qué hice en el sitio?
● ¿Qué dificultades tuve y cómo las resolví? (Indica qué recursos usaste: IA, MDN, material
complementario entregado en clase, compañeros, ayudante, etc. Si usaste IA, pega al menos un
prompt y cuenta qué tuviste que corregir.)
● ¿Qué aprendí?

## Uso Inteligencia Artificial tareas

### Actividad 1
Ninguna

### Actividad 2 
Utilicé IA solo para consultarle a cerca de cómo insertar una nueva tipografía, a lo cual me dió esta sugerencia
1. Buscar en <https://fonts.google.com/> la tipografía seleccionada
2. Descargarla
3. Al momento antes de descargarla, aparece la opción de obtener el código de inserción, el cual te lo da automático para insertarlo en HTML y CSS
4. Insertar código


### HTML
```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bree+Serif&display=swap" rel="stylesheet">
```
### CSS
```
.bree-serif-regular {
  font-family: "Bree Serif", serif;
  font-weight: 400;
  font-style: normal;
}
```
### Actividad 3
No realicé uso de inteligencia artificial, ya que fue una actividad que se realizó en conjunto durante la clase
