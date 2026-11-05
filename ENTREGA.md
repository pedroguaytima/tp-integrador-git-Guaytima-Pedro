# Entrega del Trabajo Práctico Integrador

## Datos del participante

- Nombre y apellido: Pedro Antonio Guaytima
- Curso: Introducción a Git y GitHub para la Gestión de Proyectos Digitales
- Fecha de entrega: 05/11/2026

## Enlaces

- Repositorio de GitHub: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro
- Issue: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/issues/1#issue-6192177300
- Pull request: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/pull/2#issue-6211808528

## Comandos principales utilizados

- `git init`: se utilizó al inicio para crear el repositorio local en la carpeta del proyecto.
- `git status`: se utilizó para ver el estado de los archivos: sin seguimiento, modificados y preparados para el commit.
- `git status -s`: versión compacta del anterior, que se utilizó con mayor frecuencia por mostrar el estado en una línea por archivo.
- `git add`: se utilizó para iniciar el seguimiento de archivos nuevos y pasar los cambios al área de preparación (staging).
- `git commit`: se utilizó para guardar los cambios preparados como una versión en el historial, con un mensaje descriptivo.
- `git log --oneline`: se utilizó para ver el historial de commits de forma compacta, un commit por línea.
- `git remote add origin`: se utilizó para vincular el repositorio local con el repositorio remoto de GitHub, usando su URL.
- `git remote -v`: se utilizó para listar las URL de los repositorios remotos configurados y comprobar a cuál está vinculado el proyecto.
- `git push`: se utilizó para subir los commits locales al repositorio remoto en GitHub.
- `git branch`: se utilizó para listar las ramas existentes y ver cuál es la rama activa.
- `git switch`: se utilizó para cambiar de rama.
- `git switch -c`: se utilizó para crear una rama nueva y cambiarse a ella.
- `git pull`: se utilizó para traer los cambios del repositorio remoto y actualizar el repositorio local.


## Descripción del proceso

- En el directorio local `tp-integrador`, que ya contenía `ENTREGA.md` y `README.md`, se creó la carpeta `proyectoEleccionesCAI` con `mkdir` y se agregaron los archivos `index.html` y `style.css`. Luego se inició el repositorio local con `git init`.
- Se agregó la carpeta `proyectoEleccionesCAI` al seguimiento con `git add` y se hizo un commit inicial solo con ese contenido.
- Se actualizaron `ENTREGA.md` y `README.md`, y se registraron en un nuevo commit. Después se fue modificando el proyecto en varios commits sucesivos, hasta llegar a la versión pedida por el cliente (ficticio).
- Se vinculó el repositorio local con el remoto (`git remote add origin`) y se subió la rama `master` con `git push`: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro.git
- Se creó la issue #1, que propone agregar el escudo del club en el encabezado: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/issues/1
- Estando en `master`, se obtuvo la última versión del remoto con `git pull`. Después se creó la rama `agregar-escudo`, donde se modificaron los archivos del proyecto y se actualizó `ENTREGA.md`. Los cambios se commitearon y se subieron al remoto.
- Se creó la Pull Request #2 con esos cambios: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/pull/2. Una vez validados y fusionados, la issue #1 se cerró. Luego se trajeron los cambios a `master` en local con `git pull`.
- Como agregado, se actualizó la documentación en una nueva rama, `actualizar-documentacion`, y se fusionó con una nueva Pull Request que no cierra ninguna issue. Las ramas fusionadas se eliminaron del repositorio local.

## Dificultades encontradas

**1. Advertencia de saltos de línea (LF y CRLF).** Al ejecutar `git add proyectoEleccionesCAI/index.html` apareció el mensaje: `warning: in the working copy of 'proyectoEleccionesCAI/index.html', LF will be replaced by CRLF the next time Git touches it`. Antes de comenzar el trabajo se había configurado Git para convertir automáticamente los saltos de línea (`git config --global core.autocrlf true`), porque la computadora usa Windows 11 Pro for Workstations, versión 25H2. La advertencia es informativa: Git avisa que convertirá los saltos de línea al formato de Windows. No impide el trabajo, por lo que se continuó sin cambios.

**2. Cambios sin commitear que "aparecían" en otra rama.** Después de crear la rama `agregar-escudo` se modificó `index.html`. Al cambiar a `master` para comprobar que el archivo no se hubiera modificado allí, el archivo seguía figurando como modificado. Investigando se entendió que el directorio de trabajo y el área de preparación (staging) son únicos y compartidos: no existe una copia por rama. Las ramas solo separan los commits, de modo que los cambios sin commitear acompañan al usuario al cambiar de rama. El problema se resolvió haciendo el commit en `agregar-escudo`. Después de eso, `master` quedó sin cambios.

## Reflexión final

El curso ha servidor para aclarar algunos conceptos básicos, poder debatir algunas cuestiones avanzadas como ser correr con docker, actualización de algunos comandos como switch reemplazando a checkout y fundamentalmente obtener buenas prácticas de desarrollo colaborativo.

