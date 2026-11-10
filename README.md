# Ejercicio React
Este es un proyecto que explica brevemente un stack de trabajo para hacer un proyecto en react:

    npm para gestionar dependencias y hacer la build
    vite para iniciar el proyecto y el servidor
    react como framework usado

## Dependencia React-Confetti

<img alt= "Web con dependencia React-confetti" src="./images/1web-confetti.png" style="display: block; margin: 0 auto;" width="70%"> 

## Dependencia Canvas-Confetti

<img alt= "Web con dependencia Canvas-confetti" src="./images/2web-canvasconfetti.png" style="display: block; margin: 0 auto;" width="70%"> 

## Dependencia React-Three-Fiber para renderizado 3D

<img alt= "Web con dependencia Renderizado 3D" src="./images/3-web-escena3d.png" style="display: block; margin: 0 auto;" width="70%"> 


**Si la carpeta node_modules/ está excluida, ¿borrar una dependencia hace alguna acción sobre el repositorio? ¿Cuál?**

Sí, afecta al repositorio siempre y cuando se elimine la dependencia utilizando el comando adecuado del gestor de paquetes (como npm uninstall o yarn remove).

Aunque la carpeta node_modules/ esté excluida en el archivo .gitignore (lo que significa que Git ignora todo su contenido y no lo sube al servidor), la acción de borrar una dependencia impacta al repositorio de las siguientes maneras:
- package.json: Se elimina la referencia a la dependencia en las secciones de dependencies o devDependencies.
- Al hacer el git commit y git push de los cambios en el package.json, cualquier otro desarrollador (o en nuestro entorno de producción) que descargue la última versión del repositorio y ejecute npm install sabrá que esa dependencia ya no debe instalarse o incluirse en el proyecto.