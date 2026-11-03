# Entrega del Trabajo Práctico Integrador

## Datos del participante

- Nombre y apellido: Pedro Antonio Guaytima
- Curso: Introducción a Git y GitHub para la Gestión de Proyectos Digitales
- Fecha de entrega:3 nov 2026

## Enlaces

- Repositorio de GitHub:
- Issue:
- Pull request:

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
- git merge
- git pull

## Descripción del proceso


- Parado en directorio local 'tp-integrador' con los archivos ENTREGA.md y README.md, se genera la carpeta 'proyectoEleccionesCAI' con el comando mkdir. Seguidamente se agregan los archivos index.html y style.css. En estas condiciones se inicia repositorio local git con git init.
- Se hace seguimiento a la carpeta 'proyectoEleccionesCAI'
- commit inicial solo con 'proyectoEleccionesCAI'
- Actualización de ENTREGA.md Y README.md. Seguidamente se hace seguimiento

## Dificultades encontradas

<!-- Completar: errores, dificultades o conflictos y cómo se resolvieron. -->
Tras ejecutar git add proyectoEleccionesCAI/ se presenta la siguiente advertencia "warning: in the working copy of 'proyectoEleccionesCAI/index.html', LF will be replaced by CRLF the next time Git touches it". Cabe aclarar que previo al inicio de este trabajo se configuró git para autoconversión de CRLF con valor true con el comando "git config --global core.autocrlf true", debido a que la pc corre con Windows 11 Pro for Workstations - version 25H2.


## Reflexión final

<!-- Completar: qué se aprendió al utilizar Git y GitHub. -->
El curso ha servidor para aclarar algunos conceptos básicos, poder debatir algunas cuestiones avanzadas como ser correr con docker, actualización de algunos comandos como switch reemplazando a checkout y fundamentalmente obtener buenas prácticas de desarrollo colaborativo.
