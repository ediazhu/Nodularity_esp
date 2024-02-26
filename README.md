# nodularity.py

## Descripcion General

**nodularity.py**nodularity.py es un programa que calcula la tasa de nodularidad del grafito utilizando el método ISO JIS G5502-2022 y el método JIS para productos de hierro fundido de grafito esferoidal (FCD). Aquí, la imagen del tejido se muestra a continuación.


<br><br>

<img src="https://user-images.githubusercontent.com/91704559/202900113-c0a879b3-b298-4bd7-a2df-a03c2ddf4c07.jpg" width=400>
<br>
Figura: Imagen de la estructura de productos de fundición de grafito esferoidal
<br><br>

## Entorno operativo

**nodularity.py**は、[Python](https://www.python.jp/)Funciona en una computadora con instalado. Para ejecutar este programa, se requiere una biblioteca de procesamiento de imágenes.

Ícono de validado por la comunidad[OpenCV](https://opencv.org/)se requiere.
<br><br>

## 使い方

1. Coloque **nodularity.py** en una carpeta adecuada.
2. Establezca los valores de **iDir** y **min_grainsize** en la configuración del entorno a partir de la línea 18 de **nodularity.py**. <br>
Aquí, **iDir** establece la carpeta que desea mostrar primero en el cuadro de diálogo "Seleccione un archivo de imagen", y **min_grainsize** es el valor de "tamaño mínimo de grafito" ÷ "ancho de imagen".
3. Guarde la imagen del tejido que se muestra arriba en la carpeta configurada en **iDir** en 2. arriba y ejecute **nodularity.py**. Guarde **nodularity.py** y las imágenes de la organización en una carpeta que no contenga caracteres de doble byte.
4. Cuando ejecute el programa, primero se mostrará el cuadro de diálogo "Seleccione un archivo de imagen", así que seleccione la imagen del tejido para la que desea determinar la tasa de esferoidización. Puede seleccionar varias imágenes de tejido con el mismo **min_grainsize**. Seleccione el archivo de imagen, haga clic en Abrir y espere un momento para calcular la tasa de esferoidización y crear el archivo a continuación.


**nodularity_datetime.csv**... Datos como el nombre del archivo y la tasa de esferoidización
- **Nombre del archivo de imagen_ISO.jpg** ... Resultado de la determinación de la forma del grafito (ISO)
- **Nombre del archivo de imagen_JIS.jpg** ... Resultado de la determinación de la forma del grafito (JIS)

## Respecto al uso

No somos responsables de los resultados del uso.

## Entorno de desarrollo
- Windows11
- VSC 1.7.3.1
- Python 3.8.10
- OpenCV 4.5.4
