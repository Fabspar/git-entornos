# Secuecia introductoria 3

- El objetivo de este ejercicio es crear una rama nueva llamada *bugFix* , crear dos commits tanto en la rama *main* y en la rama *bugFix* y hacer *git merge bugFix* para que tengamos el trabajo unificado.

<p align="center"><img src="imagenes-md\image6.png" alt="drawing" width="700" style="center"/></p>
<p align="center"><img src="imagenes-md\image26.png" alt="drawing" width="300" style="center"/></p>

## Comencemos:

1. *git branch bugFix*

<p align="center"><img src="imagenes-md\image21.png" alt="drawing" width="300" style="center"/></p>

- Con el comando *git branch bugFix* estoy creando una nueva rama llamada *bugFix*.

<p align="center"><img src="imagenes-md\image8.png" alt="drawing" width="200" style="center"/></p>

2. *git checkout bugFix*

<p align="center"><img src="imagenes-md\image22.png" alt="drawing" width="300" style="center"/></p>


- Hago *git checkout bugFix* para trabajar sobre esa rama. El asterisco se cambia de *main* a *bugFix*.

<p align="center"><img src="imagenes-md\image17.png" alt="drawing" width="200" style="center"/></p>

3. *git commit*

<p align="center"><img src="imagenes-md\image18.png" alt="drawing" width="300" style="center"/></p>

- Creo un nuevo commit en la rama *bugFix*, por lo tanto cambia de color ya que estoy trabajando en una rama diferente a *main*. Un commit es un nuevo conjunto de cambios en el proyecto en el que estamos trabajando.

<p align="center"><img src="imagenes-md\image15.png" alt="drawing" width="180" style="center"/></p>

4. *git checkout main*

<p align="center"><img src="imagenes-md\image2.png" alt="drawing" width="300" style="center"/></p>


- Ahora como tengo que crear un nuevo commit en la rama *main*,tengo que posicionarme en *main*, así que escribo el comando *git checkout main*.El asterisco cambia de *bugFix* a *main*, indicando que ahora estoy trabajando en esa rama.

<p align="center"><img src="imagenes-md\image12.png" alt="drawing" width="200" style="center"/></p>

5. *git commit*

<p align="center"><img src="imagenes-md\image3.png" alt="drawing" width="300" style="center"/></p>

- Creo un commit en *main* y la representación gráfica se vuelve como en dos ramas separadas.

<p align="center"><img src="imagenes-md\image27.png" alt="drawing" width="800" style="center"/></p>

6. *git merge bugFix*

<p align="center"><img src="imagenes-md\image19.png" alt="drawing" width="300" style="center"/></p>

- Por último y siguiendo en la rama *main* , con el comando *git merge bugFix* , estoy diciendo que quiero volver a unir el historial que se ha bifurcado anteriormente. A su vez se crea un nuevo commit que será el nuevo punto en el que seguiremos trabajando como continuación de la rama *main*.

<p align="center"><img src="imagenes-md\image20.png" alt="drawing" width="1500" style="center"/></p>




