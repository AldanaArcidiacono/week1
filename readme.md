# Learning Git

git init is only use when you create a repo from your local

git checkout HEAD~main : Moves the HEAD where you choose

git reset HEAD~2 : Moves the BRANCH to the commit you choose ##### (Move from the head, x commits behind or you can put the name of the commit EJ: git reset 9565cfbdbd917504a631fcbb5e2c906cfe774ca3 )

We can also find the "futures" commits showing the reflogs (to know the name of the commit) and then, in the terminal with: git reset (name of the commit)

Anything made with JS uses a gitignore of NODE

The first commit is always call "Initial commit"
To clone a repository we press CODE and copy the link under the label HTTPS and paste it on the main folder: git clone (link copied).
After, we go to the new folder that we create with: cd (name of folder).

git add .
git commit -m "(message)"
git push

## Commits

It has 4 parts.
Message
Parent
Name
Date
The commits are immutable.

## Branches

A branch is a LABEL.
I can move it and deleted.
We have infinites branches but only ONE HEAD.
git reset (name of the commit) to put it in the branch we need
A branch points only to a commit

## Have conflicts locally

First actualize the Main.
I go to my branch and do a MERGE MAIN.
Resolve conflict.
Go to gitHub and do the pull request

## Delete a branch

We are just deleting a LABEL
We go to main and use the command git branch -d (name of the branch)

## Label HEAD

We can only move it, With the command git checkout

## Merge

We have to go to our MAIN and then do the command git merge
Git makes a new commit to unite the MAIN (that may change) and your new branch

## Rebase

Also does a MERGE.
At the end, it looks like we made a fast-forward. Because it deletes the commits in the middle and re-write them (we have news commits, since this ones can not change)
It has a cleaner structure, but you can not see when you made a change in other branch

## Resolving conflicts

Conflicts happens when two persons makes changes in the same branch. We have to talk with the other person and decide witch one we should apply.

## Pull Request

To merge a branch with the main.
WE DON'T WORK ON MAIN. (just the initial files)
I ask for a pull and after someone sees it and approves it, is fusion with the main
We take the branches to the remote repo
With this we incorporate from the branch on GitHub to the main of GitHub
git push origin (name of the branch)

## Work flows

Rules to follow that the company decides to use
git flow =
We will use 🔽
gitHub flow = When you made a pull request of a branch, review the pull request. When this is approves, you can merge it and delete the branch. Master always protected. Master always actualized

# Learning HTML

We always have a head and a body on a HTML file <br>
DOCTYPE: tells the program witch HTML you are using <br>
< tag attribute="" >

## DRY

Don't repeat yourself
Do not repeat code one and other time in different pages that are link
We will mont the page dynamically, with components (React, view, angular)

### Viewport

Is used for mobiles

### Meta desc

Agrega una descripcion de la pagina para que luego se muestre en el buscador de google

### Favicon

Es importante siempre tener un favicon. Para hacer la pagina accesible.
Usamos un file .ico o .png

### HGROUP

Se usa para que tus elementos H (h1, h2, h3...) sepan que estas usando la sigueinte como un subtitulo

### Group elements

SECTION ...
DIV ...

### Menus

Los menus se realizan con listas <ul> / <ol>

## Etiquetas con valor semantico ()

### Section

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

## Imagenes

Usan un atributo width y height.
Se pone la altura y anchura real de mi foto o la que voy a decidir por CSS para que ocupe
Reserva el espacio mencionado para la foto y no da saltos al cargar la pagina, mejora la optimizacion

## Formularios

Se envuelven en una etiqueta < form > y dentro de ella usamos los controles de formulario

Nunca puede haber un campo de formalario que no indique que se debe escribir en el
Deben tener botones.

Se define como < button type="submit" >. Estos disparan los mecanismos de funcion y ayudan a la usabilidad, ya que tocando ENTER se activa el boton

Si es obligatorio, se le agrega el atributo < required >

Label: Etiqueta de un campo del formulario. Enlaza las palabras con el formulario. En el for se pone el ID de la parte del formulario que quieres.
Por ej, sirve para que no haya que tocar el cuadradito del checkbox y que con tocar el texto de al lado, te tome la respuesta

Pattern: Se usa para requerir sierto formato en el formulario. Por ej, numero de cuenta.

minlength: Longitud minima del texto que debe escribir el usuario

RadioButtons: Se agrupan por grupos, a traves del NAME. Usan el mismo.

Select: Agrupa dos etiquetas distintas y genera una ventana desplegable con opciones

Interaccion por parte del usuario fuera del FORM: DETAILS
Permite indicar un elemento SUMMARY y Parrafos
Genera un desplegable con info
