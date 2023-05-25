# 001_HTML_CSS

## para usar el Liver Server desde la terminal del Visual Studio Code

npm install live-server -g

despues escribir:

live-server  .\claseIndex\

## para subir los repositorios.

git init 
git add .
git commit -m "empezando a subir ejercicios"
git branch -M main  
git remote add origin https://github.com/CanarioEchazu/001_HTML_CSS.git
git push -u origin main 



# Errores solucionados
Efectué modificaciones con el proyecto en la nube, a la vez, hice correcciones en la PC de los archivos html.
Pero me daba error de no poder subir.
Atiné a poner 
git pull
a lo que ahora funciona correctamente.

Hice consulta al chat GPT por estos hechos, y aqui me dio la respuesta.

## Respuestas del CHAT GPT

El error que experimentaste al intentar hacer push a tu repositorio remoto en GitHub se debió a que había diferencias entre la rama local y la rama remota. La terminal te informó que la punta de tu rama local estaba detrás de su contraparte remota y te sugirió que integraras los cambios remotos antes de intentar hacer push nuevamente.

Para resolver este problema, ejecutaste el comando git pull, que fusionó los cambios remotos en tu rama local. Luego de hacer el pull, pudiste hacer push sin problemas.

Aquí está el registro de los comandos que ejecutaste:

PS D:\Estudio2\Platzy\001_HTML_CSS> git branch -M main
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
PS D:\Estudio2\Platzy\001_HTML_CSS> git remote add origin https://github.com/CanarioEchazu/001_HTML_CSS.git
PS D:\Estudio2\Platzy\001_HTML_CSS> git push -u origin main
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git add .
PS D:\Estudio2\Platzy\001_HTML_CSS> git commit -m "2da"
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git push -u origin main
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git remote add origin https://github.com/CanarioEchazu/001_HTML_CSS.git 
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git add .
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git pull
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git push -u origin main
...
PS D:\Estudio2\Platzy\001_HTML_CSS> git status
...


Después de ejecutar git pull, se fusionaron los cambios remotos en tu rama local, y luego pudiste hacer push exitosamente sin obtener el error de "non-fast-forward". La terminal indicó que tu rama estaba actualizada y no había cambios adicionales para confirmar.
