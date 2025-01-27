
# <h1 align="center"> Monitorización del Almacenamiento de Sistemas </h> 

La monitorización del almacenamiento de sistemas se refiere al proceso de supervisar y gestionar el uso de los recursos de almacenamiento en un entorno informático. Su objetivo es garantizar la disponibilidad, integridad y rendimiento de los datos almacenados en discos duros, unidades SSD, sistemas de archivos, redes de almacenamiento (SAN) y otros medios.
En esta Actividad veremos unos cuantos:

# Comandos para la Monitorización de Almacenamiento de Sistemas

## 1. Comando `free`

El comando `free` proporciona toda la información sobre la RAM, incluyendo cuánta RAM se está utilizando, cuánta está disponible, etc. El comando sin opciones muestra los resultados para la memoria Total, Usada y Libre en tu ordenador o servidor.

- `free`: Muestra la memoria total, usada y libre.
- `free -m`: Muestra la memoria en megabytes.
- `free -s 1`: Actualiza la información de la memoria cada segundo.

## 2. Comando `df`

El comando `df` (disk free) se utiliza para obtener un informe del espacio total, usado y disponible en los sistemas de archivos montados.

- `df`: Muestra el uso del espacio en disco.
- `df -h`: Muestra el uso del espacio en disco en un formato legible (ej. GB).
- `df /`: Muestra el uso del espacio en disco del sistema de archivos raíz.

## 3. Comando `du`

El comando `du` (Disk Usage) muestra el espacio en disco utilizado por archivos y directorios en el sistema.

- `du /ruta/al/directorio`: Muestra el tamaño de un directorio.
- `du -h /ruta/al/directorio`: Muestra el tamaño del directorio en un formato legible.
- `du -a /ruta/al/directorio`: Muestra el tamaño de todos los archivos y subdirectorios.

## 4. Comando `iostat`

El comando `iostat` proporciona estadísticas sobre la utilización de la CPU y los dispositivos de almacenamiento (discos duros, SSDs, etc.). Es muy útil para analizar el rendimiento de los discos y la carga de la CPU.

- `iostat`: Muestra estadísticas básicas de la utilización de CPU y discos.
- `iostat 1`: Actualiza las estadísticas cada segundo.
- `iostat -d`: Muestra estadísticas detalladas de todos los dispositivos de almacenamiento.


