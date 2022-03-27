## Cómo usar notebooks de Julia en google colab.

Lamentablemente todavía Google Colab no tiene sus máquinas virtuales instaladas por defecto con Julia.
Por lo tanto cada vez que se accede a una máquina virtual hay que instalar Julia en la misma. 
Esto se hace mediante una serie de comandos (en Python) que se ejecutan en la primer celda del notebook. 
Luego de que esos comandos se ejecuten **debe recargar nuevamente la página** y a partir de ese momento 
ya podrá seguir con los comandos usuales de Julia. 

A modo de ejemplo podrá en contrar [aquí](https://colab.research.google.com/drive/19TQkEccGqs4F3xsqMIqZf-wEsAJMH36F?usp=sharing)
una versión de la guía 1 lista para ejecutar en google colab. 

### Instrucciones:
1. Trabaje con una copia de este notebook: _File_ > _Save a copy in Drive_ (necesitará una cuenta de Google, por ejemplo la que provee la UNC). Alternativamente puede bajar localmente una copia del notebook, _File_ > _Download .ipynb_, y luego subirla a Google Colab [Colab](https://colab.research.google.com/).
2. Ejecute la primer celda (clickee en la misma y luego ingrese `Ctrl+Enter` o clickee el triangulito en la parte superior derecha de la celda. De esa forma instalará  Julia, IJulia and otros paquetes de interés. (De ser necesario cambie la versión de Julia modificando los valores de `JULIA_VERSION` y otros parámetros que crea conveniente). La instalación demorará unos minutos.
3. Una vez finalizada la instalación (y completa la ejecución de la celda) cargue nuevamente la página (`Ctrl+R`, o `⌘+R`, o `F5`) y continúe a las próximas celdas. Las 3 celdas siguientes son para controlar que la instalación haya sido exitosa y posteriormente encontrará la **Guía 1** propiamente dicha.

