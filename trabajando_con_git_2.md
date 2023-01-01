# Hasta el origen y más allá

- El objetivo a cumplir es bajarme lo que hay en el repositorio remoto y hacer *merge* en cada rama siguiendo el orden de *side1, side2, side3*. Con esto se unifica todo el trabajo que hay en las diferentes ramas con la rama principal. Finalmente hay que subir el trabajo del repositorio local  al repositorio remoto haciendo *git push*.


<p align="center"><img src="imagenes-md\image24.png" alt="drawing" width="700" style="center"/></p>

<p align="center"><img src="imagenes-md\image9.png" alt="drawing" width="300" style="center"/></p>

## Empecemos:

1. *git checkout*

<p align="center"><img src="imagenes-md\image11.png" alt="drawing" width="300" style="center"/></p>

- Hago un *checkout* sobre la rama main(rama principal),para trabajar sobre ella.

<p align="center"><img src="imagenes-md\image5.png" alt="drawing" width="900" style="center"/></p>

2. *git fetch;git merge o/main*

<p align="center"><img src="imagenes-md\image14.png" alt="drawing" width="300" style="center"/></p>

- Con *git fetch* me bajo lo que hay en el repositorio remoto,en este caso el commit *c8* no lo tengo en el repositorio local.
Con el comando *git merge o/main* le estoy diciendo que a partir de *o/main*(a partir de lo último subido al repositorio remoto), cree una nueva rama y ponga allí los commits que no tenía en mi repositorio local.
Haciendo *git pull* me hubiese ahorrado un comando, pero haciéndolo con esos dos comandos creo que queda más claro a la hora de explicarlo.

3. *git merge side1*

<p align="center"><img src="imagenes-md\image13.png" alt="drawing" width="300" style="center"/></p>

- Haciendo *git merge side1*, le estoy diciendo a la rama principal main que se una a la rama secundaria *side1*,creando un nuevo commit c9 como nuevo punto de continuación.
Con este comando, el historial del trabajo que hemos estado realizando quedaría reflejado tal cual lo estábamos haciendo,manteniendo a salvo la historia de la rama *side1*.
Si se utilizase *git rebase*, la rama *side1* se hubiera integrado con la rama principal y el historial de cada paso de lo que hemos estado haciendo no quedaría reflejado,pero al utilizar rebase todo queda más ordenado y claro.
El punto donde estamos trabajando nos lo marca *main**, que ha pasado al nuevo commit *c9*.

<p align="center"><img src="imagenes-md\image1.png" alt="drawing" width="700" style="center"/></p>

4. *git merge side2*

<p align="center"><img src="imagenes-md\image10.png" alt="drawing" width="300" style="center"/></p>

- Al hacer merge sobre *side2* se unen las ramas de *main* y *side2*, y se crea un nuevo commit ,*c10* , en la rama de *main*. 
Con esto sucede lo mismo que cuando hemos hecho *git merge side1*, se ha guardado toda la historia de la rama *side2* y se ha creado un nuevo commit que será el nuevo punto en el que seguiremos trabajando.

<p align="center"><img src="imagenes-md\image23.png" alt="drawing" width="700" style="center"/></p>

5. *git merge side3*

<p align="center"><img src="imagenes-md\image16.png" alt="drawing" width="300" style="center"/></p>

- El penúltimo paso es hacer *git merge side3* para unir la rama main con la rama *side3* y seguir guardando todo el historial de ramas que hemos estado haciendo hasta ahora. Se crea el último commit , *c11*, y *main** se vuelve a desplazar a éste ya que es siguiente commit en el que vamos a seguir trabajando. 

<p align="center"><img src="imagenes-md\image7.png" alt="drawing" width="700" style="center"/></p>

6. *git push*

<p align="center"><img src="imagenes-md\image28.png" alt="drawing" width="300" style="center"/></p>

- El último paso para finalizar el ejercicio será subir los cambios al repositorio remoto y para ello se utiliza el comando *git push*.
Vemos que *o/main(origin/main)* ha pasado al último commit, así a la hora de volver a subir nuevos cambios vamos a saber hasta dónde subimos los últimos cambios la anterior vez.

<p align="center"><img src="imagenes-md\image4.png" alt="drawing" width="3000" style="center"/></p>














