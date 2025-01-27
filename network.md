# Monitorización de la Red

La **monitorización de la red** es la supervisión del tráfico y rendimiento de la red, con el fin de asegurar su funcionamiento eficiente, detectar problemas de conectividad y garantizar la seguridad y el rendimiento óptimo.

## 1. Aspectos clave de la monitorización de la red

1.1 **Tráfico de red**:
   - Se supervisa la cantidad de datos que fluyen hacia y desde los dispositivos en la red para detectar cuellos de botella y asegurar el uso eficiente del ancho de banda.

1.2 **Rendimiento de la red**:
   - **Velocidad de transmisión**: Se mide la rapidez con la que los datos viajan por la red.
   - **Latencia**: El tiempo que tarda un paquete de datos en llegar a su destino. Alta latencia afecta negativamente a aplicaciones en tiempo real.
   - **Pérdida de paquetes**: Se mide la cantidad de paquetes perdidos durante la transmisión, lo que indica posibles problemas en la red.

1.3 **Disponibilidad de la red**:
   - Se asegura que los dispositivos y servicios de la red estén disponibles y accesibles para los usuarios.

1.4 **Seguridad de la red**:
   - Se supervisan intentos de intrusión, tráfico no autorizado y ataques como DDoS, para garantizar la integridad y seguridad de la red.

1.5 **Dispositivos y topología de red**:
   - Se hace un seguimiento del estado de los dispositivos conectados y su interconexión, incluidos routers, switches, firewalls y servidores.

## 2. Beneficios de la monitorización de la red

- **Optimización del rendimiento**: Ayuda a identificar y resolver cuellos de botella, mejorando la eficiencia de la red.
- **Detección temprana de problemas**: Permite identificar problemas antes de que afecten gravemente la conectividad o los servicios.
- **Mejora de la seguridad**: Ayuda a detectar accesos no autorizados y vulnerabilidades en la red.
- **Prevención de caídas de red**: Permite intervenir antes de que ocurran problemas graves que puedan causar la caída de la red.


## 3 Comandos
### 3.1 **tcpdump**
`tcpdump` permite capturar y analizar el tráfico de red que pasa a través de una interfaz de red.  
![tcpdump.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/tcpdump.png)

#### Opciones:
- **`-i <nombre_interfaz>`**: Especifica la interfaz de red a monitorizar (por ejemplo, `eth0` o `wlan0`).
![tcpdum -i.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/tcpdum%20-i.png)
- **`port <nº_puerto>`**: Filtra el tráfico para capturar solo el que pasa por el puerto indicado.
![tcpdump.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/tcpdump.png)

### 3.2 **tcptrack**
`tcptrack` es una herramienta de monitorización en tiempo real que muestra conexiones TCP activas, direcciones IP origen y destino, puertos, estado de la conexión y cantidad de datos transmitidos en un formato visual.

#### Opciones:
- **`-i <nombre_interfaz>`**: Permite especificar la interfaz de red a monitorizar.
![tcp track.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/tcp%20track.png)

### 3.3 **iptraf-ng**
`iptraf-ng` es una herramienta interactiva que proporciona estadísticas detalladas sobre el tráfico de red en tiempo real.
![iptraf-ng.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/iptraf-ng.png)
![opcion de iptraf-ng.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/opcion%20de%20iptraf-ng.png)

#### Opciones:
- La interfaz gráfica de `iptraf-ng` permite seleccionar diferentes tipos de monitorización, como ver estadísticas generales, por protocolo o flujos de red específicos.

### 3.4 **netstat**
`netstat` es una herramienta clásica para inspeccionar conexiones de red, sockets y estadísticas del sistema.  
![netstat.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/netstat.png)

#### Opciones:
- **`-a`**: Muestra todas las conexiones y puertos de escucha, incluyendo las conexiones activas y los puertos en espera de conexiones.
![netstat -a.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/netstat%20-a.png)
- **`-n`**: Muestra las direcciones IP y los números de puerto en formato numérico, sin realizar la resolución de nombres de host.
![netstat -n.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/netstat%20-n.png)
- **`-tp`**: Muestra las conexiones TCP activas junto con los PID y los nombres de los procesos que las están utilizando.
![netstat -tcp.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/netstat%20-tcp.png)
- **`-l`**: Muestra únicamente las conexiones que están en estado de "escucha", es decir, los puertos que están esperando recibir conexiones entrantes.
![netstat -l.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Network/netstat%20-l.png)
