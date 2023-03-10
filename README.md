# Enunciado ejercicios básicos de Git, GitHub (Parte 1)
# Repositorio masterpidgey-examen
### Crear un repositorio en vuestro GitHub llamado masterpidgey-examen.
- Creamos el repositorio de examen desde el github
![Alt text](capturas/Crearrepositorio.png)
### Clonar vuestro repositio en local.
- git clone https://github.com/DavidTous/masterpidgey-examen.git
![Alt text](../Clonamoselrepositorio.png)
### README
Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md.
- git touch README.md
![Alt text](../creamos_readme.png)
Y añadimos el README.md
- git add README.md
![Alt text](../A%C3%B1adimos_el_readme.png)

### Commit inicial
Añadir al README.md los comandos utilizados hasta ahora y hacer un coomit inicial con el mensaje commit inicial.
- git commit -m "commit inicial"
![Alt text](../Commit_inicial.png)

### Push inicial
Subir los cambios al repositorio remoto.
- git push -u origin main
![Alt text](../Push_inicial.png)

### Ignorar archivos
Crear en el repositorio local un fichero llamado privado.txt.
- touch privado.txt
![Alt text](../creamos_archivo_privado.png)
Crear en el repositorio local una carpeta llamada privada.
- mkdir privada
![Alt text](../creamos_carpeta_privada.png)
Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.
- nano .gitignore
![Alt text](../creamos_gitignore.png)
![Alt text](../editando_gitignore.png)

### Añadir fichero 1.txt
Añadir fichero 1.txt al repositorio local.
- touch 1.txt
![Alt text](../creamos_1txt.png)
- git add 1.txt
![Alt text](../a%C3%B1adimos_1txt.png)
# Visualizar los commits realizados hasta el momento
- git log
![Alt text](../visualizar_commits.png)
### Crear el tag v0.1
- git tag -a v0.1
![Alt text](../creamos_tag.png)
### Subir el tag v0.1
Subir los cambios al repositorio remoto.
- git push --tags
![Alt text](../subir_tags.png)
# Visualizar de nuevo los commits realizados hasta el momento
- git log
![Alt text](../visualizar_commits2.png)
### Crear una tabla
Crear una tabla de este estilo en el fichero README.md con la información del docente del módulo:
| Nombre | Github |
| ------ | ------ |
| Maximo | [enlace github](https://github.com/maximofernandezriera) |
### Colaboradores
Poner a github.com/maximofernandezriera como colaborador del repositorio masterpidgey-examen
![Alt text](../a%C3%B1adir_colaborador.png)
# Contribución guiada a un proyecto (Simulación examen parte 2)
### Contribución al proyecto first-contributions

1. Realizamos un fork del repositorio
Realiza un fork del repositorio haciendo un clic en el botón fork de la parte superior de la página. Esto creará una instancia del repositorio completo en tu cuenta.
![Alt text](../hacemos_el_fork.png)
2. Clona el repositorio
Una vez que el repositorio esté en tu cuenta, clónalo a tu ordenador para trabajarlo localmente.

- git clone https://github.com/DavidTous/first-contributions.git
![Alt text](../clonamos_fork.png)
clone2
Ahora hemos configurado una copia de la rama maestra desde el repositorio principal del proyecto en línea.

Debemos ir al repositorio clonado ejecutando el siguiente comando:

- cd first-contributions/
![Alt text](../entramos_en_carpeta.png)

3. Crea una rama
Es una buena práctica crear una rama (branch) nueva cuando trabajas con repositorios, ya sea que se trate de un proyecto pequeño o estés contribuyendo en un equipo de trabajo.

El nombre de la rama debe ser breve y debe reflejar el trabajo que estamos haciendo.

- git checkout -b rama
![Alt text](../creamos_rama.png)

4. Realiza cambios y confírmalos
Has cambios esenciales al proyecto y guárdalos.
Creamos un fichero
- nano fichero.txt
![Alt text](../creamos_fichero.png)

- git status
![Alt text](../status.png)
Agrega esos cambios a la rama recién creada usando el comando git add:

- git add .
![Alt text](../add_rama.png)

Ahora confirma esos cambios utilizando el comando git commit:

- git commit -m "commit rama"
![Alt text](../commit_rama.png)

5. Envía los cambios a GitHub
Para enviar los cambios a GitHub, debemos identificar el nombre del repositorio remoto.

- git remote
![Alt text](../remote.png)

Para este repositorio el nombre es "origin".

Luego de identificar el nombre podemos enviar en forma segura los cambios a GitHub.

- git push origin rama
![Alt text](../push_rama.png)

6. Crea un pull request
Ve a tu repositorio en GitHub y verás un botón llamado "Pull request", has clic en él.


Por favor, provee todos los detalles necesarios de lo que has hecho. Ahora, envía el pull request.

![Alt text](../pull_request.png)

7. Sincroniza tu rama maestra con la del repositorio original
Antes de enviar cualquier pull request al repositorio original debes sincronizar tu repositorio con aquel.


Primero, revisamos en que rama estás ubicado.
- git branch
![Alt text](../en_que_rama.png)
Esto enumerará todas las ramas y indicará en verde la rama actual o activa.

2. Cambia a la rama maestra.

- git checkout main
![Alt text](../rama_main.png)

3. Agrega el repositorio original como un repositorio upstream.

Para poder extraer los cambios desde el repositorio original a tu versión local, necesitas agregar el repositorio Git original como un repositorio upstream.

- git remote add upstream https://github.com/maximofernandezriera/first-contributions.git
![Alt text](../upstream.png)

4. Busca (fetch) el repositorio.

Busca todos los cambios  del repositorio original. Las confirmaciones (commits) del repositorio original serán almacenadas en una rama local llamada upstream/master.

- git fetch upstream
![Alt text](../fetch.png)
5. Fusionala.

Fusiona los cambios de la rama upstream/master a tu rama maestra local. Esto hará que tu rama maestra se sincronice con el repositorio upstream sin perder tus cambios locales.

- git merge upstream/main
![Alt text](../merge.png)
6. Envía (push) los cambios a GitHub

En este punto tu rama local está sincronizada con la rama maestra del repositorio original. Si deseas actualizar el repositorio de GitHub, necesitas enviar tus cambios.

- git push origin main
![Alt text](../push_main.png)


Y con esta practica enseñamos todos los conocimientos que tenemos de git.