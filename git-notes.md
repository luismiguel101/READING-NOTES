# comandos esenciales Git
Este documento contiene una recopilacion de los comandos fundamentales de git que todo desarrollador debe conocer.

1. ## Configuración inicial
# Configurar el nombre de usuario
git config --global user.name "Tu Nombre"

# Configurar el correo electrónico
git config --global user.email "tuemail@example.com"

# Verificar la configuración
git config --list

2. ## Creación y administración de repositorios

# Inicializar un nuevo repositorio
git init

# Clonar un repositorio existente
git clone URL_DEL_REPOSITORIO

3. # Estados del repositorio y seguimiento de cambios

# Ver el estado del repositorio
git status

# Agregar archivos al área de preparación (staging area)
git add nombre_archivo    # Un solo archivo
git add .                 # Todos los archivos

# Confirmar cambios con un mensaje
git commit -m "Mensaje descriptivo del cambio"

4. # Gestión de ramas

# Crear una nueva rama
git branch nombre_rama

# Cambiar a otra rama
git checkout nombre_rama

# Crear y cambiar a una nueva rama
git checkout -b nombre_rama

# Listar todas las ramas
git branch

# Fusionar una rama en la actual
git merge nombre_rama

# Eliminar una rama
git branch -d nombre_rama

5. # Trabajo con un repositorio remoto

# Agregar un repositorio remoto
git remote add origin URL_DEL_REPOSITORIO

# Ver los repositorios remotos configurados
git remote -v

# Enviar cambios al repositorio remoto
git push origin nombre_rama

# Obtener cambios del repositorio remoto
git pull origin nombre_rama

6. # Deshacer cambios 

# Descartar cambios en un archivo
git checkout -- nombre_archivo

# Restablecer el área de preparación
git reset nombre_archivo

# Deshacer un commit pero mantener los cambios en el área de trabajo
git reset --soft HEAD~1

# Deshacer un commit y eliminar los cambios definitivamente
git reset --hard HEAD~1

7. # Inspección y depuración

 Ver el historial de commits
git log

# Ver cambios en los archivos
git diff

# Ver quién hizo cambios en una línea específica
git blame nombre_archivo

8. # Git stash (guardar cambios temporalmente)

# Guardar cambios sin confirmarlos
git stash

# Ver lista de cambios almacenados
git stash list

# Aplicar el último stash guardado
git stash apply

# Eliminar el último stash
git stash drop

9. # Otros comandos útiles

# Eliminar un archivo del repositorio pero mantenerlo localmente
git rm --cached nombre_archivo

# Agregar un alias para comandos largos
git config --global alias.st status  # Ahora `git st` equivale a `git status`