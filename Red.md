# <h1 align="center"> Monitorización de la Red </h> 

La **monitorización de la red** permite observar el tráfico de datos que fluye a través de las interfaces de red, así como gestionar conexiones activas y analizar el rendimiento de la red. Esto es útil para detectar problemas de conectividad, optimizar el tráfico y realizar auditorías de seguridad.

## Herramientas principales

### TCPDUMP
Es una herramienta cuya utilidad principal es analizar el tráfico que circula por la red. Permite al usuario capturar y mostrar en tiempo real los paquetes transmitidos y recibidos por la red a la cual el ordenador está conectado.

- `tcpdump`: Captura todos los paquetes en la interfaz de red predeterminada.
  ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump.png?raw=true)
- `tcpdump port`: Captura todos los paquetes que pasan por el puerto 80 (HTTP) en la interfaz
  ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump%20port%2080.png?raw=true)
- `tcpdump -i eth0`: Captura solo los paquetes ICMP (utilizados por el comando ping y mensajes de control de red).
  ![tcpdump](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcpdump%20-i.png?raw=true)



### TCPTRACK
Muestra las conexiones TCP activas en tiempo real, indicando las direcciones IP de origen y destino, el estado de la conexión y la cantidad de datos transmitidos.

- `sudo tcptrack -i enp0s3`: Muestra las conexiones TCP activas en la interfaz de red predeterminada.
  ![tcptrack](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcptrack%20-i.png?raw=true)
- `sudo tcptrack -i enp0s3 -v`: Muestra las conexiones con detalles de los datos transmitidos.
  ![tcptrack](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcptrack%20-v.png?raw=true)
- `sudo tcptrack -i enp0s3 -n`: Muestra las conexiones en formato numérico.
  ![tcptrack](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/tcptrack%20-n.png?raw=true)

### IPTRAF-NG
Es una herramienta interactiva que ofrece estadísticas detalladas sobre el tráfico de red en tiempo real. Se utiliza para supervisar y analizar conexiones de red, tráfico de datos y más.

- `sudo iptraf-ng Opcion: Ip traffic monitor`: Muestra estadísticas de tráfico en modo automático.
  ![iptraf-ng](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/iptraf-ng.png?raw=true)
- `sudo iptraf-ng General Interface`: Muestra estadísticas de tráfico para la interfaz `eth0`.
  ![iptraf-ng](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/iptraf-ng%20general.png?raw=true)
- `sudo iptraf-ng detailed interface`: Muestra los detalles explicadas numericamente
  ![iptraf-ng](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/iptraf-ng%20detailed.png?raw=true)

### NETSTAT
Es una herramienta clásica para inspeccionar las conexiones de red, los puertos abiertos y las estadísticas de red.

- `netstat -n`: Muestra todas las conexiones establecidas con direcciones numéricas.
- ![netstat](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/netstat%20-n.png?raw=true)
- `netstat -p`: Muestra las conexiones de red y los programas asociados.
- ![netstat](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/netstat%20-p.png?raw=true)
- `netstat -i`: Muestra estadísticas detalladas de las interfaces de red.
- ![netstat](https://github.com/josemanuellamprea/MONOTORIZACION/blob/main/Img/netstat%20-i.png?raw=true)

