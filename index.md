# Práctica GitFlow

## Que es Git y GitFlow?
Git es un software de control de versiones diseñado por Linus Torvalds, pensando en la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones cuando éstas tienen un gran número de archivos de código fuente y Git-flow es un conjunto de extensiones para Git, basado en el modelo de ramificaciones de Vincent Driessen, que nos facilita el trabajo con nuestros repositorios.

![Logo Git](https://upload.wikimedia.org/wikipedia/commons/thumb/3/3f/Git_icon.svg/1024px-Git_icon.svg.png)

## Documentación de la práctica

### Usuario 1
Primeramente clonaremos el repositorio que hemos creado en github utilizando el comando git clone "url" y una vez clonado realizaremos un git flow init para trabajar con esta extensión.

En segundo lugar crearemos una feature mediante el comando git flow start "nombre", para trabajar, con lo que crearemos la rama y nos posicionaremos en esta. A continuación debemos actualizar los datos en local mediante un git add . y un git commit -m "nombre" y realizamos un git flow feature publish "nombre" para subirlo a remoto y finalmente debemos cerrar esta rama con el comando git flow feature finish "nombre". 

### Usuario 2
ara trabajar con el usuario dos clonaremos el repositorio y iniciaremos el comando git flow init para utilizar git flow y creamos dos nuevas features con el comando git flow feature start "nombre" e implementar estas funcionalidades.
Cuando terminemos de utilizar estas ramas, como ningún usuario las va a utilizar las podremos eliminar con el comando git floe feature finish "nombre" y este contenido se añadirá a la rama develop.

### Usuario 3
En este usuario realizaremos el mismo proceso de clonación del proyecto y realizaremos las nuevas funcionalidades, cuando terminemos eliminaremos la rama con el mismo comando utilizado anteriormente.
Cuando tengamos todas estas funcionalidades y arreglados los conflictos, tan solo nos quedará crear una nueva feature (git flow release start "nombre") por si tenemos un cambio leve antes del lanzamiento y podremos eliminar la release con el comando git flow release fisnish "nombre".

### Usuario 1
Por último el usuario 1 creara una rama hotfix para arreglar un bug con el comando git flow hotfix start "nombre" y una vez arreglado el fallo realizara el comando git flow hotfix finish "nombre" para cerrarlo
