# Learning Git

##### GIT INIT

Se usa cuando creas el repo desde tu local

##### git checkout HEAD~main

Mueve el HEAD a donde indiques

##### git reset HEAD~2

Mueve la rama al commit que elijas.
Mueve desde el HEAD, x commits atras o puedes poner el nombre del commit al que quieres que vuelva.
EJ: git reset 9565cfbdbd917504a631fcbb5e2c906cfe774ca3

We can also find the "futures" commits showing the reflogs (to know the name of the commit) and then, in the terminal with: git reset (name of the commit)

Anything made with JS uses a gitignore of NODE

The first commit is always call "Initial commit"
To clone a repository we press CODE and copy the link under the label HTTPS and paste it on the main folder: git clone (link copied).
After, we go to the new folder that we create with: cd (name of folder).

git add .
git commit -m "(message)"
git push

## Commits

Un commit consta de 4 partes:
Mensaje, Padre, Nombre y Fecha
Los commits son inmutables

## Branches

Una rama es una etiqueta.
Se puede mover y eliminar.
Podemos tener ramas infinitas. Pero solo UN HEAD
git reset (nombre del commit) para ponerlo en la rama que queramos

## Have conflicts locally

Primero actualizamos el MAIN
Vamos a la rama y hacemos un MERGE al MAIN
Resolvemos el conflicto (en local)
Lo enviamos a GitHub, donde hacemos el pull request

## Delete a branch

Solo se esta borrando una etiqueta
Vamos al MAIN y usamos el comando:
git branch -d (nombre de la rama)

## Label HEAD

Solo podemos moverlo con el comando
git checkout

## Merge

Debemos ir al MAIN, luego hacer un
command git merge
Git hace un nuevo commit para unir la rama (la cual irá cambiando) y el MAIN

## Rebase

Tambien hace un MERGE.
Cuando termina, se ve como si se hubiera hecho un fast-forward. Ya que elimina los commits que han quedado en el medio y los re-escribe (Tendremos nuevos commits, ya que los que hicimos no se pueden modificar)
Tiene una estructura limpia, pero no puedes ver los cambios hechos

## Resolver conflictos

Los conflictos pasan cuando dos personas realizan cambios en la misma rama. Para solucionarlo se debe hablar con la otra persona y desidir cual deberíamos aplicar.

## Pull Request

Se usa para mergiar una rama al main.
NO SE TRABAJA EN MAIN. (Solo los archivos iniciales si)
Se pregunta para hacer una pull request y despues que alguien la aprueba, la rama se fusiona con el main.
Podemos llevar las ramas al repo remoto, para incorporar la rama al main de GitHub
git push origin (nombre de rama)

## Work flows

Reglas que la compania / empresa decide utilizar
git flow =
En el bootcamp usamos 🔽
gitHub flow = Cuando haces un pull request de una rama, revisamos el pull request primero. Si este es aprovado, lo mergeamos y eliminamos la rama.
Main siempre debe estar protegido y actualizado.

# HTML

Siempre tenemos un HEAD y un BODY en un archivo HTML<br>
DOCTYPE: dice que programa de HTML estas usando<br>
< tag attribute="" >

## DRY

Don't repeat yourself
No realizar codigo repetido o copiado y pegado en diferentes links de la misma pagina
La pagina se monta dinamicamente con componenetes (como React, View, Angular)

### HEADER

Puede tener elementos de navegacion y de informacion principal de la pagina. Pero no es obligatorio.
Lleva el logo y menu.
Para poner el log, EJ en index.html de esta carpeta

### Viewport

Se utiliza para moviles

### Meta desc

Agrega una descripcion de la pagina para que luego se muestre en el buscador de google

### Favicon

Es importante siempre tener un favicon. Para hacer la pagina accesible.
Usamos un file .ico o .png

### HGROUP

Se usa para que tus elementos H (h1, h2, h3...) sepan que estas usando la sigueinte como un subtitulo

### Group elements

SECTION: Suelen tener título. Solo respetando la semantica. Agrupa una seccion de informacion. Si no le puedes poner nombre, suele significar que no es necesario usarla.

DIV: Se pueden usar tantos como quieras. Dividen elementos de la pagina

### Menus

Los menus se realizan con listas < ul > / < ol >

## Etiquetas con valor semantico ()

### Article

Es una seccion que otorga un bloque de articulo a algo
Agrupa toda la informacion que necesitas para comprender el texto
Informacion distribuible u objetos reales
Que con ese trozo de informacion te puedas enterar de todo (EJ: Una noticia, un elemento de una tienda)

### Aside

Info complementaria a la principal de la pag web

### Address

Datos de autoria de la pagina. Suele estar en el footer

## Grouping

### Main

Agrupador de elementos principales
Agrupa lo que no es compartido con el resto de las pag del sitio.
Solo se usa UNA VEZ por página
No aporta nada a la estructura del sitio

## Imagenes

Usan un atributo width y height.
Se pone la altura y anchura real de mi foto o la que voy a decidir por CSS para que ocupe
Reserva el espacio mencionado para la foto y no da saltos al cargar la pagina, mejora la optimizacion

## Formularios

Se envuelven en una etiqueta < form > y dentro de ella usamos los controles de formulario

Nunca puede haber un campo de formalario que no indique que se debe escribir en el

Si es obligatorio, se le agrega el atributo < required >

### Deben tener botones.

Se define como < button type="submit" >.
Estos disparan los mecanismos de funcion y ayudan a la usabilidad, ya que tocando ENTER se activa el boton

### Label

Etiqueta de un campo del formulario. Enlaza las palabras con el formulario. En el for se pone el ID de la parte del formulario que quieres.
Por ej, sirve para que no haya que tocar el cuadradito del checkbox y que con tocar el texto de al lado, te tome la respuesta

### Pattern

Se usa para requerir sierto formato en el formulario. Por ej, numero de cuenta.

### Minlength

Longitud minima del texto que debe escribir el usuario

### RadioButtons

Se agrupan por grupos, a traves del NAME. Usan el mismo.

### Select

Agrupa dos etiquetas distintas y genera una ventana desplegable con opciones

### Details

Interaccion por parte del usuario fuera del FORM
Permite indicar un elemento SUMMARY y Parrafos.
Genera un desplegable con la info de los parrafos, la cual solo se ve al clicar

#### HR

No se usa para hacer la linea. Se hace desde CSS, dandole un borde al elemento superior o al elemento inferior

#### BR

No se usa. Para dar un salto de linea se hace desde CSS con margin y paddin

# CSS

Nunca usamos el atributo STYLE para modificar el CSS dentro del HTML. A no ser, que estes usando un framework que necesites que lo hagas
EJ: < h1 style="font-size: 1rem" >

La etiqueta < style >, se puede usar si estas haciendo una prueba o poniendo estilos muy cortos.

Teniendo en un fichero aparte, mejora la legibilidad y puede hacer que varios HTML usen el mismo diseño de CSS

Selector de ID NO SE USA ya que tiene demasiadas especificaciones

Selectores multiples: Le agrega a varias cosas el mismo estilo

### CSSS RESET

Primero se realiza el CSS, para asegurarte de que los navegadores no modifiquen el CSS
Normalmente se aplica en un ficehro aparte
Primero reseteo los estilos y luego agrego los mios
En un proyecto real es práctico. Pero no vamos a estar usandolo mucho para aprender cosas

### Medida REM:

Si quiero modificar fuentes siempre uso REM por accesibilidad. Ayuda al usuario a que pueda aumentar la tipografia. Cosa que los PX no permiten.
Valen igual en toda mi pagina web, es una unidad estable.

### Medida EM:

Es relativo y varia segun se va cambiando el tamaño de la letra.

### Medida en viewport height / width

min-height: 100vh; Setea la minima altura al viewport (la pantalla en donde se esta mirando tu web)
Lo usamos sobre todo para headers y footer que le queramos dar un tamaño
min-width: 100wh;

### Medida caracteres

Que no ponga en la pantalla lineas de más de X caracteres

### COLOR

Inherit coge el valor que heredaria de tu padre. Para que si hay cambios no haya que cambiarlos
Initial hace que vuelva al valor que tenía al principio de todo
La paleta de colores se aplica mediante variables por JS

### Propiedades logicas

No se usa mas top, bottom, left, right
margin-block-start: ; al principio del bloque (top)
margin-block-end: ; al final del bloque (bottom)
margin-inline-start: ; al principio de la linea (right)
margin-inline-end: ; al final de la linea (left)

## Cajas

En CSS todo es cajas. Tienen contenido, padding, borde y margen
Modelo de cajas : Box-Sizing: border-box = Indica su borde, su padding y su contenido. Para acomodar las cajas en la pantalla.
El border-box, no se hereda. Por eso siempre lo ponemos al principio y con (UN SOLO ASTERISCO) **{}. Para aplicarselo a todo el html.
Se escapan dos elementos, el after y el before. Por lo cual, ponemos ** , **::after, **::before {}

### Margen

El margen se entiende como una cosa externa

## Maquetar

Reacomodar la disposicion de los elementos (Layout)
Para ayudarnos a crear layouts usamos flex-box y grid (cuando sea necesario)
Ambos son modos de display
Para comenzar tener siempre la cantidad de bloques necesarios.

### Display FLEX

Automaticamente todos los elementos a los que les das display flex, los elementos dejan de ser bloque para ser linea.
Se aplica en el contenedor padre

#### Flex direction

ROW - COLUMN - ROW REVERSE - COLUMN REVERSE
ROW: de der a izq
COLUMN de abajo arriba

#### Flex-wrap

No-Wrap = Se aplastan para caber todos dentro, no revasaria
wrap = Se dividen las pantallas al 50% (si cabe en dos columnas) y lo coloca al principio a la izq

#### Flex-flow

Une flex direction y wrap

#### Justify content

Se utiliza para centrar elementos en la pantalla
Permite colocar los elementos de izq a derecha
Horisontal

#### Align Items

Se utiliza para centrar elementos en la pantalla
Permite colocar los elementos de arriba a abajo
Vertical

#### Gap

Sirve para dejar un espacio entre los distintos elementos
Es mejor utilizar esto que margin, para separar a los hijos
Lo realiza respecto a los hijos del contenedor al que se lo aplicas

#### Propiedades para aplicar a los hijos

Con order le damos un orden a sus hijos EJ: order: 2; (lo pone segundo)
Para posicionar un elemento sin tener en cuenta los demas elementos EJ align-self: center;

#### Flex

flex: 0 1 auto;
Flex es el resumen de las demas propiedades juntas:

flex-grow: ; Cuanto quiero que puedan crecer. Le digo que puede crecer X más que su hermano
flex-shrink: ; Cuanto quiero que puedan encoger
flex-basis: ; Que quiero que tomen como punto de partida

Si los dos tienen el valor de creciemito igual (grow) crecen al 50%
Utiliza un ratio entre valores. Hay veces que no es tan preciso.

## Metalenguaje

Un lenguaje que el navegador no entiende. El navegador solo entiende JS, CSS y HTML
Podemos usar uno, como TY o SASS, pero hay que traducirlos.
Codigo fuente y codigo compilado:
El codigo fuente (EJ: SASS), no tiene ningun valor y hay que compilarlo para subirlo (EJ: netlify)

### Sass

Es un pre-procesador de CSS
.
