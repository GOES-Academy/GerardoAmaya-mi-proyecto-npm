# Proyecto con NPM y Git

Este es un ejemplo de cómo crear un proyecto utilizando NPM y Git, incluyendo explicaciones sobre los paquetes, dependencias, diferencias entre CommonJS y ESModule, así como el funcionamiento de Git y cómo gestionar los archivos.

## Crear un Proyecto con NPM

Para crear un proyecto con NPM, sigue estos pasos:

1. **Inicializa un Nuevo Proyecto:**

   ```bash
   npm init

2. **Instalar los Paquetes Necesarios:**

   ```bash
   npm install nombre-del-paquete

## Paquetes y Módulos en NPM

En NPM, los paquetes son conjuntos de código reutilizable que puedes compartir con otros desarrolladores. Estos paquetes están organizados en módulos, que son archivos o directorios que contienen un conjunto de funcionalidades relacionadas.

## Paquetes y Gestión de Dependencias

Los paquetes pueden tener dependencias, que son otros paquetes que necesitan para funcionar. Estas dependencias se instalan automáticamente cuando instalas un paquete, y se guardan en el archivo `package.json` en la propiedad `dependencies`., además puedes gestionarlas siempre en el archivo `package.json`.

* Agregar una Dependencia:

  ```bash
  npm install nombre-del-paquete --save

* Eliminar una Dependencia:

  ```bash
    npm uninstall nombre-del-paquete --save

* Actualizar una Dependencia:

  ```bash
    npm update nombre-del-paquete --save

## CommonJS y ESModule

CommonJS y ESModule son dos estándares para la creación de módulos en JavaScript. CommonJS es el estándar utilizado por Node.js, mientras que ESModule es el estándar utilizado por JavaScript.

* CommonJS:

  ```bash
    const modulo = require('nombre-paquete');

* ESModule:

    ```bash
    import modulo from 'nombre-paquete';

## Git y Rastreo de Archivos

Git es un sistema de control de versiones que nos permite rastrear los cambios que hacemos en los archivos de nuestro proyecto. Para utilizar Git, debemos inicializar un repositorio con el comando `git init`, y luego agregar los archivos que queremos rastrear con el comando `git add nombre-archivo`. Una vez agregados los archivos, podemos guardar los cambios con el comando `git commit -m "mensaje"`. También podemos ver el estado de los archivos con el comando `git status`.

## .gitignore

El archivo `.gitignore` nos permite ignorar archivos o directorios que no queremos rastrear con Git. Para ello, debemos agregar el nombre del archivo o directorio en el archivo `.gitignore`

* Ejemplo de como ignorar archivos `.gitignore`:

    ```bash
    node_modules
    .env
    .DS_Store
