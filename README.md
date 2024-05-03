Git y Github

## Git

### Configurar git

Una vez instalado git por primera vez antes de inicializar un proyecto git deberemos realizar algunas configuraciones por unica vez.

- Poner o cambiar nombre: `git config --global user.name "tu nombre"`

- Poner o cambiar email: `git config --global user.email “tu email”`

- cambiar el nombre por defecto de la rama principal en configuraciones: `git config --global init.defaultBranch main` (esta es una configuracion global lo que implica que al iniciar los siguientes proyectos en git el nombre por defecto de la rama principal sera como la que pusimos, en este caso "main", este comando no cambiara el nombre de las ramas de los proyectos git ya existentes, si quieres cambiar el nombre de una rama ya existente puedes usar `git branch -m nuevo_nombre`)

- Ver todas las configuraciones hechas = `git config --list` (Para salir se preciona tal tecla `esc` y luego la tecla `q`)

### Primeros Pasos

- Iniciar un proyecto git: `git init`

- Ver el estatus de los archivos: `git status`

### Stage

- Añadir archivos al staged: `git add .` (es necesario hacer este add para todos los archivos nuevos recién creados en nuestro directorio) (caso de no querer añadir ciertos archivos o directorios sera necesario un .gitignore)

- Eliminar un archivo individualmente del staged `git rm --cached fileName.extension` (deja de rastrear un archivo específico en Git sin eliminarlo del sistema de archivos ni del área de preparación. Es útil cuando se desea mantener el archivo en el sistema de archivos pero ya no se quiere rastrear en
  
  Git.)

- Eliminar directorio completo del staged: `git rm -r --cached nombre_directorio` (se usa un `.` en lugar del nombre del directorio para eliminar todo el staged y dejarlo vacio)
