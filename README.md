Configurar VSC para Django (Actualizado 03/2024)
[Ver documento original aquí](https://gist.github.com/hcosta/6e4066adb1938c888546c5f0a9616c48)
***LAS IMAGENES Y EXPLICACION***

Actualmente no es necesario configurar el proyecto en el directorio .vscode/settings.json, es mucho más fácil. Solo hay que seguir estos pasos:

Antes de nada instalad estas extensiones en vuestro Visual Studio Code:

Python: https://marketplace.visualstudio.com/items?itemName=ms-python.python
Pylance: https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance
Pylint: https://marketplace.visualstudio.com/items?itemName=ms-python.pylint
Django: https://marketplace.visualstudio.com/items?itemName=batisteo.vscode-django
Djaneiro: https://marketplace.visualstudio.com/items?itemName=thebarkman.vscode-djaneiro
En vuestro entorno virtual (o lo que uséis) instalad los paquetes pylint y pylint-django

pipenv install pylint pylint-django
A continuación abrid la configuración de VSC en File > Preferences > Settings.

En el filtro poned pylint y en los Args añadid una línea como la siguiente

"pylint.args": ["--load-plugins", "pylint_django"]
Os deberá quedar como en esta captura:
image

Aquí un GIF del entorno configurado:
image

Más adelante al crear un fichero html con templates de Django recordad seleccionar el tipo Django Template en la sintaxis y listo:
image

@FernPS
FernPS commented on Jun 22, 2024
Perfecto, configuración realizada. Tenia un error en mi archivo settings.json, lo cual, no me dejaba ejecutar el paso 4, pero luego de poner una coma que me faltaba, pude ejecutarlo sin problema.

@Twinkym
Twinkym commented 2 weeks ago
Hecho, creo que me va a gustar este curso.
