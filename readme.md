# Pasos seguidos para la creación de un repositorio

1. En primer lugar hemos inicializado un repositorio de manera local mediante git init repo01
2. A continuación, nos hemos movido al directorio en cuestión mediante cd repo01
3. Una vez estamos en el directorio, creamos un archivo readme.md mediante 
   ```
   touch readme.md
   ```
4. Con el archivo creado, abrimos el archivo readme.md para documentar el procedimiento
   ```
   code readme.md
   ```
5. Dado que hemos realizado modificaciones en el directorio de trabajo, añadimos estas a nuestro staging area
    ```
    git add readme.md
    ```
6. Con el siguiente comando comprobamos que hay cambios listos para hacer commit
    ```
    git status
    ```
7. Realizamos un snapshot hacia el repositorio en local
    ```
    git commit -m "Primer snapshot"
    ```
8. Accedemos a GitHub y creamos el repositorio remoto (con la configuración por defecto).
9. Asociamos el repositorio remoto al local cogiendo la dirección HTTPS.
    ```
    git remote add origin https://github.com/Mil4n0r/repo01.git
    ```
10. Comprobamos que se ha asociado correctamente
    ```
    git remote -v
    ```
11. Creamos la rama main
    ```
    git branch -M main
    ```
12. Subimos los cambios del commit al repositorio remoto
    ```
    git push -u origin main
    ```