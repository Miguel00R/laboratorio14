Preparar el entorno (Instalar requisitos)
Un programa basado en YOLOv8 y PyTorch requiere un entorno de Python con ciertas librerías instaladas, siendo las más comunes:

Python (versión 3.7 o superior).

PyTorch (la librería de deep learning).

Ultralytics (la librería oficial de YOLOv8).

Generalmente, estas librerías se instalan a través del gestor de paquetes pip de Python, o a partir de un archivo de requisitos (requirements.txt) que debería estar dentro de tu carpeta extraída.

Si necesitas instalar la librería Ultralytics (YOLOv8) y sus dependencias, el comando típico es:

Bash

pip install ultralytics
3. Ejecutar el programa
Hay dos métodos principales para ejecutar un programa que usa un modelo YOLOv8:

Opción A: Usando el comando yolo (el método más fácil)
Si has instalado la librería ultralytics, puedes ejecutar la detección directamente desde la línea de comandos usando el modelo yolov8n.pt que se encuentra en tu carpeta.

Sintaxis general para detectar objetos en una imagen o video:

Bash

yolo predict model=yolov8n.pt source='ruta/a/tu/imagen.jpg'
# O para un video:
yolo predict model=yolov8n.pt source='ruta/a/tu/video.mp4'
Reemplaza ruta/a/tu/imagen.jpg con la ruta del archivo que quieres analizar.

El archivo de modelo yolov8n.pt debe estar en el directorio actual o debes especificar su ruta completa.

Opción B: Ejecutando un script de Python
Si dentro de tu archivo LAB14.rar hay un script de Python (ej. detect.py, run.py, etc.), este script contendrá la lógica de ejecución.

Sintaxis general:

Bash

python nombre_del_script.py
A menudo, estos scripts aceptan argumentos para especificar el modelo y la fuente. Revisa la documentación o el código fuente del script para ver los argumentos específicos que requiere.
