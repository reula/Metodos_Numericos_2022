# Tutorial sobre cómo hacer un security copy `scp` desde y hacia *atom*

Asumamos, por ejemplo, que en mi computadora personal mi usuario es `juan` y en la super-compu *atom* mi usuario es `jperotti`. 

## Para copiar desde *laptop* a *atom*

Supongamos que en mi computadora personal existe un archivo llamado `archivo-en-laptop.txt` en la carpeta `Desktop/mis-archivos/` dentro de mi home, y lo deseamos copiar a una carpeta llamada `parcial` que se encuentra dentro de mi carpeta home en *atom*. Entonces, desde una terminal en la latop ejecutamos el comando

      juan@laptop $ scp ~/Desktop/mis-archivos/archivo-en-laptop.txt jperotti@atom.famaf.unc.edu.ar:~/parcial/
      
Aquí, `scp` es el nombre del comando *security copy*, y se utiliza para copiar archivos entre máquinas via internet.
      
**Recuerde:** El camino completo de la carpeta `parcial` en atom es `/home/jperotti/parcial/`. De manera análoga, el camino completo de la carpeta `mis-archivos` en mi laptop es `/home/juan/mis-archivos/`

## Para copiar desde *atom* a *latop*

Supongamos que en *atom* existe un archivo `notebook-en-atom.ipynb` dentro de la carpeta `parcial` y lo queremos copiar a nuestra carpeta `mis-archivos` dentro de `Desktop`. Entonces ingresamos el siguiente comando en una terminal de nuestra laptop.

      juan@laptop $ scp jperotti@atom.famaf.unc.edu.ar:~/parcial/notebook-en-atom.ipynb ~/Desktop/mis-archivos/

**Note:** Siempre trabajamos en nuestra laptop. Lo que cambia es el orden en que especificamos los directorios/archivos. Primero origen y luego destino.

