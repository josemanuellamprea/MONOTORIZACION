# <h1 align="center"> Monitorización de Procesos de Sistemas </h> 

La **monitorización de procesos** es esencial para conocer el comportamiento de los programas y servicios en ejecución en un sistema. Permite a los administradores identificar procesos que consumen demasiados recursos (como CPU o memoria), y gestionar su ejecución para mantener el rendimiento del sistema.

## Herramientas principales

### PS
Proporciona una instantánea de los procesos en ejecución en el sistema. Se utiliza para obtener información sobre procesos activos y sus recursos asociados.

- `ps`: Muestra todos los procesos actuales.
- `ps -a`: Muestra los procesos que están ejecutándose en el terminal actual, pero no incluye los procesos de otros usuarios.
- `ps aux`: Combinación de tres opciones que proporciona una lista más completa de todos los procesos en ejecución en el sistema.

### TOP
Muestra una lista dinámica y en tiempo real de los procesos en ejecución, permitiendo observar qué procesos consumen más recursos del sistema. A diferencia de `ps`, `top` se actualiza continuamente.

- `top`: Muestra en tiempo real los procesos más activos.
- `top -m`: Muestra información de la memoria activada y desactivada.
- `top -u root`: Muestra los procesos del usuario root.

### HTOP
Es una versión mejorada de `top`, con una interfaz gráfica más amigable, que también muestra información en tiempo real de los procesos y recursos del sistema. Ofrece opciones interactivas como ordenar por diferentes columnas y visualizar los procesos en un árbol.

- `htop`: Muestra una interfaz interactiva para monitorear los procesos.
- `htop -t`: Muestra los procesos en forma de árbol.
- `htop --sort-key PERCENT_MEM`: Ordena los procesos por uso de memoria.

### ATOP
Es una herramienta avanzada que ofrece una monitorización más detallada, mostrando estadísticas sobre el uso de CPU, disco, memoria, red y más. También puede almacenar registros históricos para su posterior análisis.

- `atop`: Muestra el uso de recursos del sistema en tiempo real.
- `atop -d 2`: Actualiza la información de los recursos cada 2 segundos.
- `atop -a`: Muestra solo los procesos activos.

