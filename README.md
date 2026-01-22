# Entorno virtual

Este proyecto usa Torch para crear/usar redes neuronales. Esta librería no es compatible con la última versión de python (3.13), así que tenemos que usar la última compatible (3.10) para el entorno.

Si ya habéis conseguido instalar torch, torchvision y numpy, no hace falta que hagáis nada. Esta guía es para quienes no lo hayan conseguido por un error con torch al intentar instalar torch.

1. Lo primero es instalar la versión 3.10 de Python. Vamos a dejar la versión que teníamos de antes. Es normal tener varias versiones diferentes de Python. Podéis bajar la versión 3.10.11 de aqui´:

    - Windows: https://www.python.org/ftp/python/3.10.11/python-3.10.11-amd64.exe

    - MacOS: https://www.python.org/ftp/python/3.10.11/python-3.10.11-macos11.pkg

2. Lo instalamos. En Windows, sin seleccionar "Add to path" (si lo añadimos al path, ésta pasará a ser la versión por defecto del sistema y puede que algo deje de funcionar)

En MacOS no hace falta cambiar ninguna de las opciones por defecto. Bajamos el .pkg del link y ejecutamos el instalador hasta el final.

3. Una vez instalada, abrimos un terminal y comprobamos qué versiones tenemos instaladas de python haciendo:

    - En Windows: py -0p (un cero, no una letra O)

    - En Linux/MacOS: which python3 o which python

Si da error el comando, probamos a reiniciar el equipo y a ejecutarlo otra vez.

4. Copiamos el path donde está instalada la versión 3.10 (en mi caso, C:\Users...\Python310\python.exe).

    - En Windows, botón derecho sobre la cabecera del terminal, Edit/Mark, seleccionáis con el botón derecho el path en el terminal, botón derecho otra vez, y queda copiado en el portapapeles.

    - En Linux/MacOS, selecciónamos el path en el terminal, botón y Copiar.

5. Ahora vamos al directorio donde tenemos el código del proyecto bajado de GitHub

6. Si tenéis una carpeta de entorno env de antes (porque ya habéis intentado crear el entorno virtual antes), la borráis.

    - En Windows: rmdir env /S

    - En Linux/MacOS: rm -rf env

7. Y ahora volvemos a crear el entorno virtual pero usando la versión 3.10 de Python (sustituid mi path al ejecutable de python por el que habéis copiado vosotr@s):

    C:\Users\bortx\AppData\Local\Programs\Python\Python310\python.exe -m venv env

8. Activamos el entorno virtual

    - En Windows: env\Scripts\activate

    - En Linux/MacOS: source env/bin/activate

9. Instalamos torch, torchvision y numpy:

     python -m pip install torch numpy torchvision scikit-learn matplotlib seaborn

Si todo ha ido bien, tendremos ya un entorno virtual con Python 3.10 y Torch/Torchvision/Numpy