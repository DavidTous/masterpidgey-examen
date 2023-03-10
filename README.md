# Examen

### Comandos:

- git tag -a v0.1
![capt](Capturas/6.png)
![capt](Capturas/7.png)
- Foto de perfil
![capt](Capturas/8.png)
- Autentificador
![capt](Capturas/9.png)
![capt](Capturas/10.png)
![capt](Capturas/11.png)

| Nombre | Github |
| -- | -- |
| Tomas | [Tomas](https://github.com/tomascarrascoo) |
| Miguel | [Miguel](https://github.com/MiguelOrtsB) |
| Carlos | [Carlos](https://github.com/CharlyMech) |

![capt](Capturas/12.png)
![capt](Capturas/13.png)
- git push --set-upstream origin v0.2

# Enunciado ejercicios básicos de Git, GitHub (Parte 1)
# Repositorio masterpidgey-examen
### Crear un repositorio en vuestro GitHub llamado masterpidgey-examen.
- Creamos el repositorio de examen desde el github
![capt](Crearrepositorio.png)
### Clonar vuestro repositio en local.
- git clone https://github.com/DavidTous/masterpidgey-examen.git
![capt](Clonamoselrepositorio.png)
### README
Crear (si no lo habéis creado ya) en vuestro repositorio local un documento README.md.
- git add README.md
![capt](Añadimos_el_readme.png)
Y añadimos el README.md
- git add README.md
![capt](Añadimos_el_readme.png)

### Commit inicial
Añadir al README.md los comandos utilizados hasta ahora y hacer un coomit inicial con el mensaje commit inicial.
- git commit -m "commit inicial"
![capt](Commit_inicial.png)

### Push inicial
Subir los cambios al repositorio remoto.
- git push -u origin main
![capt](Push_inicial.png)

### Ignorar archivos
Crear en el repositorio local un fichero llamado privado.txt.
- touch privado.txt
![capt](creamos_archivo_privado.png)
Crear en el repositorio local una carpeta llamada privada.
- mkdir privada
![capt](creamos_carpeta_privada.png)
Realizar los cambios oportunos para que tanto el archivo como la carpeta sean ignorados por git.
- nano .gitignore
![capt](creamos_gitignore.png)
![capt](editando_gitignore.png)

### Añadir fichero 1.txt
Añadir fichero 1.txt al repositorio local.
- touch 1.txt
![capt](creamos_1txt.png)
- git add 1.txt
![capt](añadimos_1txt.png)
# Visualizar los commits realizados hasta el momento
- git log
![capt](visualizar_commits.png)
### Crear el tag v0.1
- git tag -a v0.1
![capt](creamos_tag.png)
### Subir el tag v0.1
Subir los cambios al repositorio remoto.
- git push --tags
![capt](subir_tags.png)
# Visualizar de nuevo los commits realizados hasta el momento
- git log
![capt](visualizar_commits2.png)
### Crear una tabla
Crear una tabla de este estilo en el fichero README.md con la información del docente del módulo:
| Nombre | Github |
| ------ | ------ |
| Maximo | [enlace github](https://github.com/maximofernandezriera) |
### Colaboradores
Poner a github.com/maximofernandezriera como colaborador del repositorio masterpidgey-examen
![capt](añadir_colaborador.png)
# Contribución guiada a un proyecto (Simulación examen parte 2)
### Contribución al proyecto first-contributions