# Entrega del Trabajo Práctico Integrador

## Datos del participante

- Nombre y apellido: Pedro Antonio Guaytima
- Curso: Introducción a Git y GitHub para la Gestión de Proyectos Digitales
- Fecha de entrega:3 nov 2026

## Enlaces

- Repositorio de GitHub: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro
- Issue: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/issues/1#issue-6192177300
- Pull request: https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/pull/2#issue-6211808528

## Comandos principales utilizados

- git init: empleado al momento inicial luego de crear
- git status: empleado para verificar estado de archivos no seguidos, agregados, modificados y commiteados.
- git status -s: empleado con mayor frecuencia que el anterior para obtener información compacta.
- git add: usado para seguimiento y agregar archivos y directorio a staged area
- git commit
- git log --oneline
- git remote add origin
- git remote -v
- git push
- git branch
- git switch (o git checkout, indicar cuál se usó)
- git switch -c: para crear y situarse en nueva rama.
- git pull


## Descripción del proceso


- Parado en directorio local 'tp-integrador' con los archivos ENTREGA.md y README.md, se genera la carpeta 'proyectoEleccionesCAI' con el comando mkdir. Seguidamente se agregan los archivos index.html y style.css. En estas condiciones se inicia repositorio local git con git init.
- Se hace seguimiento a la carpeta 'proyectoEleccionesCAI'
- commit inicial solo con 'proyectoEleccionesCAI'
- Actualización de ENTREGA.md Y README.md. Seguidamente se hace seguimiento y commit.
- Se actualizan los archivos propios del proyecto tantas veces como commits figuran hasta lograr la versión deseada por el cliente (ficticio).
- Se conectó **la rama master** con el repositorio remoto https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro.git
- Se genera Issue https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/issues/1#issue-6192177300
- Aceptada la issue y parado en la rama principal (master), se obtiene la última versión del repositorio remoto con git pull. Posteriormente se crea rama agregar-escudo y sobre ella se trabajan los archivos pertinentes, además se actualiza ENTREGA.md. Finalmente se commitean y suben los cambios al repositorio remoto.
- Se genera PR con los cambios subidos( https://github.com/pedroguaytima/tp-integrador-git-Guaytima-Pedro/pull/2#issue-6211808528 ). Validados los mismos, se cierra issue.
- Se traen los cambios a la rama master en local.
- Como agregado se actualizaron los archivos de documentación en una nueva rama actualizar-documentacion, la cual sirvió para fusionar los cambios en un nuevo PR. Este último no cierra ninguna issue.


## Dificultades encontradas

Tras ejecutar git add proyectoEleccionesCAI/ se presenta la siguiente advertencia "warning: in the working copy of 'proyectoEleccionesCAI/index.html', LF will be replaced by CRLF the next time Git touches it". Cabe aclarar que previo al inicio de este trabajo se configuró git para autoconversión de CRLF con valor true con el comando "git config --global core.autocrlf true", debido a que la pc corre con Windows 11 Pro for Workstations - version 25H2.

Luego de crear la rama agregar-escudo, se modificó el archivo index.html. Cuando se verifica que el mismo no haya sido modificado en la rama master(rama principal) se observa que el archivo figuraba con modificación. Investigando se entendió que Las zonas workingg directory y staged area son únicas y compartidas: no existe una copia por rama. Las ramas solo separan los commits, con lo cual al hacer commits se resolvió el problema.



## Reflexión final

El curso ha servidor para aclarar algunos conceptos básicos, poder debatir algunas cuestiones avanzadas como ser correr con docker, actualización de algunos comandos como switch reemplazando a checkout y fundamentalmente obtener buenas prácticas de desarrollo colaborativo.

