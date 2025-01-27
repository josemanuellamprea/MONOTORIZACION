
# <h1 align="center"> Monitorización del Almacenamiento de Sistemas </h> 

La monitorización del almacenamiento de sistemas se refiere al proceso de supervisar y gestionar el uso de los recursos de almacenamiento en un entorno informático. Su objetivo es garantizar la disponibilidad, integridad y rendimiento de los datos almacenados en discos duros, unidades SSD, sistemas de archivos, redes de almacenamiento (SAN) y otros medios.
En esta Actividad veremos unos cuantos:

# Comandos para la Monitorización de Almacenamiento de Sistemas

## 1. Comando `free`

El comando `free` proporciona toda la información sobre la RAM, incluyendo cuánta RAM se está utilizando, cuánta está disponible, etc. El comando sin opciones muestra los resultados para la memoria Total, Usada y Libre en tu ordenador o servidor.

- `free`: Muestra la memoria total, usada y libre.
  ![Free](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/Captura%20de%20pantalla%202025-01-27%20171205.png?raw=true)
- `free -h`: El comando free -h muestra información sobre el uso de la memoria del sistema en un formato legible para humanos.
  ![Free -h](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/Captura%20de%20pantalla%202025-01-27%20171430.png?raw=true)
- `free -b`: El comando free -b en Linux se utiliza para mostrar información sobre el uso de la memoria en el sistema, pero con la diferencia de que en lugar de mostrar los valores en un formato legible (como en KB, MB o GB), muestra el uso de la memoria en bytes.
  ![Free -b](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/Captura%20de%20pantalla%202025-01-27%20171357.png?raw=true)

## 2. Comando `df`

El comando `df` (disk free) se utiliza para obtener un informe del espacio total, usado y disponible en los sistemas de archivos montados.

- `df`: Muestra el uso del espacio en disco.
  ![df](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/df.png?raw=true)
- `df -h`: Muestra el uso del espacio en disco en un formato legible (ej. GB).
  ![df](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/df%20-h.png?raw=true)
- `df T`: Este comando muestra la información del espacio en disco, pero también indica el tipo de sistema de archivos para cada partición, como ext4, xfs, btrfs, entre otros.
![df](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/df%20-T.png?raw=true)

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


