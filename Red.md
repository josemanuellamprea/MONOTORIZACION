# <h1 align="center"> Monitorización de la Red </h> 

La **monitorización de la red** permite observar el tráfico de datos que fluye a través de las interfaces de red, así como gestionar conexiones activas y analizar el rendimiento de la red. Esto es útil para detectar problemas de conectividad, optimizar el tráfico y realizar auditorías de seguridad.

## Herramientas principales

### TCPDUMP
Es una herramienta cuya utilidad principal es analizar el tráfico que circula por la red. Permite al usuario capturar y mostrar en tiempo real los paquetes transmitidos y recibidos por la red a la cual el ordenador está conectado.

- `tcpdump`: Captura todos los paquetes en la interfaz de red predeterminada.
- ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump.png?raw=true)
- `tcpdump port`: Captura todos los paquetes que pasan por el puerto 80 (HTTP) en la interfaz
  ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump%20port%2080.png?raw=true)
- `tcpdump -i eth0`: Captura solo los paquetes ICMP (utilizados por el comando ping y mensajes de control de red).
- ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump%20-i.png?raw=true)



### TCPTRACK
Muestra las conexiones TCP activas en tiempo real, indicando las direcciones IP de origen y destino, el estado de la conexión y la cantidad de datos transmitidos.

- `sudo tcptrack`: Muestra las conexiones TCP activas en la interfaz de red predeterminada.
- `sudo tcptrack -i eth0`: Muestra todas las conexiones TCP activas en tiempo real en la interfaz `eth0`.
- `sudo tcptrack -i eth0 -v`: Muestra estadísticas detalladas de las conexiones TCP activas en la interfaz `eth0`.

### IPTRAF-NG
Es una herramienta interactiva que ofrece estadísticas detalladas sobre el tráfico de red en tiempo real. Se utiliza para supervisar y analizar conexiones de red, tráfico de datos y más.

- `sudo iptraf-ng -d`: Muestra estadísticas de tráfico en modo automático.
- `sudo iptraf-ng -i eth0`: Muestra estadísticas de tráfico para la interfaz `eth0`.
- `sudo iptraf-ng -B`: Ejecuta `iptraf-ng` en segundo plano y genera un informe de tráfico.

### NETSTAT
Es una herramienta clásica para inspeccionar las conexiones de red, los puertos abiertos y las estadísticas de red.

- `netstat -n`: Muestra todas las conexiones establecidas con direcciones numéricas.
- `netstat -p`: Muestra las conexiones de red y los programas asociados.
- `netstat -i`: Muestra estadísticas detalladas de las interfaces de red.

