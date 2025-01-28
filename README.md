# Comandos en Git y Github. 
 
## Mi proyecto Local a GitHub: 

-Creo mi proyecto en local.  
-Desde mi carpeta del proyecto, abro vs code:
```
code .
```
-Dentro de la raíz mi proyecto añado un archivo llamado **README.md**
-Dónde los apuntes para escribirlo correctamente se encuentrán aquí:
https://github.com/im-luka/markdown-cheatsheet?tab=readme-ov-file#headings

-Para subirlo a GitHub: 
1.Dentro de mi cuenta : "new repository".   
2.Añadir nombre y descripción.  
3. Ya tengo mi dirección a este repositorio. 
4.Dentro de Bash en la ruta a mi proyecto: 
(Symfony crea el git init directamente). 
```
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/im-luka/proyecto-local.git
git push origin main
```

## Mi proyecto de GitHub a Local. 
-Dentro de mi GitHub en mi proyecto, en la pestaña "code", copiar la URL del repositorio. 
-Abro GitBush en la ruta donde quiero almacenar mi proyecto. 
Comandos: 
```
git clone https://github.com/im-luka/proyecto-local.git
cd nombre-archivo (será el nombre del proyecto). 
code . (Abrir el proyecto en vs Code).
composer install.
```
-Llamo a composer install porque en ese momento el proyecto no funciona, le falta los archivos 'vendor' y 'var' y necesitamos reconstruir el proyecto para que vaya al archivo composer.json y descargue las librerías necesarias. 
-Realizo un add y un commit para guardar los cambios y enviarlos a GitHub: 
```
git add .
git commit -m "ADD Vendor and Var". 
```
## Mi proyecto en Local y en GitHub. 
-Si hago cambios en mi proyecto local y quiero subirlos a GitHub: 
```
git add .
git commit -m "Cambios"
git push origin main
```
-Si hago cambios en GitHub y quiero subirlos a mi proyecto local: 
```
git pull origin main
``` 



