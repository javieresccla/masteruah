## 1.

He creado el repositorio en github

Lo he clonado con el comando **git clone https://github.com/javieresccla/masteruah/**

Luego me he movido a la carpeta con **cd masteruah** y he creado el archivo con **type nul > README.md**

Lo he abierto con **start README.md** y estoy escribiendo la documentación



## Commit inicial 

Voy a guardar el archivo, hacer **git add README.md** y a hacer **git commit -m "commit inicial" **, ya que no es necesario hacer "un git init"

Por último, tras esta linea subiré los archivos a remoto mediante **git push https://github.com/javieresccla/masteruah**



## Añadir fichero 1.txt

Creo el archivo mediante **type nul > 1.txt**



## Crear un tag **v0.1**

Mediante **git tag v0.1** creamos el primer tag



## Subir el tag v0.1

Voy a guardar el documento, añadirlo para el commit mediante **git add .** , a hacer commit con **git commit -m "segundo commit"** a subir este cambio a remoto mediante **git push https://github.com/javieresccla/masteruah**



## Crear una rama v0.2

He creado la rama mediante **git branch v0.2** y me posicionaré en ella mediante **git checkout v0.2**



## Añadir fichero 2.txt

Creo el archivo mediante **type nul > 2.txt**



## Crear rama remota v0.2

Hago **git add .** junto a un commit con **git commit -m "tercer commit"** y lo subimos a remoto con **git push https://github.com/javieresccla/masteruah**



## Merge directo

Nos posicionamos en la rama master mediante **git checkout main** (ya que asi se llama mi rama master) y hacemos merge con **git merge v0.2 **



## Merge con conflicto

Abrimos 1.txt  y escribimos "hola" en el mismo. Nos posicionamos con **git checkout v0.2** y hacemos lo propio con 2.txt y "adios". A continuacion hacemos commit con **git commit -m "cuarto commit"** y desde la rama main haremos **git merge v0.2**



## Listado de ramas

Haremos un listado de ramas mediante **git branch** y recibimos esto:

```
* main
  v0.2
```



## Borrar rama

Creamos el tag con **git tag v0.2** y borramos la rama de igual nombre mediante **git branch -d v0.2** y podríamos hacerlo de forma remota con **git push https://github.com/javieresccla/masteruah :v0.2 **



## Listado de cambios

Para hacer el listado usaremos **git log** y se nos devuelve lo siguiente:

```
commit 2e129ff6a0133173fc5ae8cf1496256c53768bc5 (HEAD -> main, tag: v0.2)
Author: javieresccla <jescribanocla@gmail.com>
Date:   Wed Mar 9 20:58:56 2022 +0100

    cuarto commit

commit 70c245f910bd804c8fcf2023b64ea955cf66fc98
Author: javieresccla <jescribanocla@gmail.com>
Date:   Wed Mar 9 20:27:24 2022 +0100

    segundo commit

commit 5fd1f3542a715d0659df168843ec972f9f9354f6 (tag: v0.1)
Author: javieresccla <jescribanocla@gmail.com>
Date:   Wed Mar 9 20:06:16 2022 +0100

    commit inicial
```



## Cuenta de GitHub

Para cambiar la foto de perfil, en mi perfil clicaré en la foto y la sustituiré por una mia.

Por otra parte, la autenticación en dos pasos se activa en la sección "Password and authentication" . Elegiré hacerlo por SMS, introduciendo mi número.



## Uso social de GitHub

He seguido a Damian, Álvaro, Victor y a Javi García, además de darles estrellas



## Crear una tabla

| NOMBRE | GITHUB                                |
| :----: | ------------------------------------- |
| Damian | https://github.com/MrDamian1723       |
| Álvaro | https://github.com/alvarolosadaromero |
| Victor | https://github.com/victor-aljama      |
|  Javi  | https://github.com/JavierGarciaRuiz   |



## Colaboradores

Para poner a alguien de colaborador, vamos al repositorio y en ajustes encontramos el apartado "Collaborators" 



## Crear una organización

La creamos en el apartado de "Organizations" dentro de ajustes. Crearemos una nueva desde cero y le pondremos el nombre solicitado. Por último tendremos que hacer algunos ajustes en cuanto al objetivo de la organización



## Crear equipos

En el apartado "teams" podemos crear nuevos equipos. El primero se llamará administradores y, como se nos manda, tendrá mas permisos que el resto. A este equipo invitaré a i12vecaj, MrDamian1723 y a victor-aljama 

Por otra parte en el equipo colaboradores estará JavierGarciaRuiz y alvarolosadaromero



## Crear pull requests



Voy a hacer un solo pull request, ya que no he encontrado mas compañeros que hayan sido capaces de llegar hasta aquí. A partir de aquí he avanzado con Victor, ya que nos encontrabamos los dos en el mismo punto. Voy a hacer fork de su repositorio. 

Previo a esto, hemos tenido que permitir que los miembros creen repositorios públicos en los ajustes de la organización y hemos cambiado nuestros repositorios a públicos, para poder verlos. Dejo aún así los enlaces por que no tengo muy claro como pueden verse

* https://github.com/masteruah-javieresccla/Pagina-web (repositorio creado por mí)
* https://github.com/masteruah-javieresccla/prueba1 (fork del repositorio de Victor)
* https://github.com/masteruah-victor-aljama/prueba1.git (repositorio original de Victor)

### 

### Realización 

Hacemos fork del repositorio de Victor. Para ello, en el repositorio clicaremos en fork y tendremos una copia del mismo en nuestra cuenta. En este caso, he elegido hacerlo en la organización, por seguir probando con ella. A continuación lo traeremos a local con git clone para poder modificarlo

Nos situamos en el repositorio con **cd prueba1** y con **git branch "javieresccla"** creamos una rama con mi nombre, en la que modificaremos el index.html y añadiremos nuestro nombre. Añadiremos el index con **git add .** y haremos el commit con **git commit -m "commit oficial"**.(Hice un commit antes, pero no cambie la rama)

A continuación en github, en el repositorio al que he hecho fork podremos iniciar un pull request. Elegiremos las ramas que queremos comparar. En este caso serían la rama main del repositorio de Victor con la rama "javieresccla" de mi repositorio fork.  A partir de aqui es decisión del owner aceptar el mismo o no



## Gestionar Pull-requests

Con el pull request de Victor hecho, en el apartado de pull request "abiertas" podemos administrarla. Para aceptarla, le clicamos y decidimos hacer merge entre las ramas (quizás no ha sido la opción mas acertada, ya que lo óptimo creo que habría sido dejarlo en diferentes ramas, pero al estar probandolo por primera vez no lo he hecho)

