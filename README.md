# sublime-text-terminal
Abrir Sublime Text desde la terminal en OSX
---

Vamos a crear un comando para abrir archivos o carpetas desde la terminal con Sublime text. 

Requisitos 
---
- Sublime text 2 o 3 instalado en la carpeta ´Aplicaciones´

Setup
---
Para poder abrir sublime desde la Terminal lo unico que hay que hacer es crear un symlink `/usr/local/bin/subl` apuntando a la App de Sublime. Para ello haremos lo siguente:

### Sublime Text 2


	ln -sv "/Applications/Sublime Text 2.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl

### Sublime Text 3


	ln -sv "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/local/bin/subl


### Test

Abrir un nuevo archivo desde la Terminal:

	subl test.rb

*Esto deberia abrir un nuevo archivo `test.rb` en Sublime Text*

Abrir una carpeta de Proyecto.

	subl dir/project
	
Abrir la App en si misma.

	subl
	
Para mostrar la ayuda.
	
	subl -h


### NOTA: No soy responsable si por alguna razon se produce algun daño en tu sistema por el uso de este tutorial. (No deberia pasar nada malo igualmente).

Mas info [sublime docs](https://www.sublimetext.com/docs/2/osx_command_line.html)
