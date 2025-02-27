# <h1 align="center"> Monitorización de Procesos de Sistemas </h> 

La **monitorización de procesos** es esencial para conocer el comportamiento de los programas y servicios en ejecución en un sistema. Permite a los administradores identificar procesos que consumen demasiados recursos (como CPU o memoria), y gestionar su ejecución para mantener el rendimiento del sistema.

## Herramientas principales

### PS
Proporciona una instantánea de los procesos en ejecución en el sistema. Se utiliza para obtener información sobre procesos activos y sus recursos asociados.

- `ps`: Muestra todos los procesos actuales del sistema actualmente.
  ![ps](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/ps.png?raw=true)
- `ps -a`: Muestra los procesos que están ejecutándose en el terminal actual pero no incluye los procesos de otros usuarios.
  ![ps -a](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/ps%20-a.png?raw=true)
- `ps aux`: Combinación que proporciona una lista más completa de todos los procesos en ejecución en el sistema.
  ![ps aux](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/ps%20aux.png?raw=true)

### TOP
Muestra una lista dinámica y en tiempo real de los procesos en ejecución, permitiendo observar qué procesos consumen más recursos del sistema. A diferencia de `ps`, `top` se actualiza continuamente.

- `top`: Muestra en tiempo real los procesos más activos del sistema.
  ![top](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/top.png?raw=true)
- `top -p`: Muestra solo el proceso con el ID especificado (PID) del sistema actualmente.
  ![top -p](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/top%20-p.png?raw=true)
- `top -i root`: Ignora los procesos inactivos. Muestra solo los procesos activos en el sistema.
  ![top -i](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/top%20-i.png?raw=true)

### HTOP
Es una versión mejorada de `top`, con una interfaz gráfica más amigable, que también muestra información en tiempo real de los procesos y recursos del sistema. Ofrece opciones interactivas como ordenar por diferentes columnas y visualizar los procesos en un árbol.

- `htop`: Muestra una interfaz interactiva para monitorear los procesos.
  ![htop](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/htop.png?raw=true)
- `htop -u`: Se utiliza para mostrar solo los procesos que están siendo ejecutados por un usuario específico en el sistema.
  ![htop -u](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/htop%20-u.png?raw=true)
- `htop --tree`: Cambia la forma en que se muestran los procesos, mostrándolos en forma de árbol.
  ![htop --tree](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/htop%20--tree.png?raw=true)

### ATOP
Es una herramienta avanzada que ofrece una monitorización más detallada, mostrando estadísticas sobre el uso de CPU, disco, memoria, red y más. También puede almacenar registros históricos para su posterior análisis.

- `atop`: Muestra el uso de recursos del sistema en tiempo real.
  ![atop](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/atop.png?raw=true)
- `atop -d 2`: Actualiza la información de los recursos cada 2 segundos.
  ![atop -d](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/atop%20-d.png?raw=true)
- `atop -a`: Muestra solo los procesos activos.
  ![atop -a](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/atop%20-a.png?raw=true)

