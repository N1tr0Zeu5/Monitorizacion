# Monitorizacion de la Red
### 1. **tcpdump**
`tcpdump` permite capturar y analizar el tráfico de red que pasa a través de una interfaz de red.

#### Opciones:
- **`-i <nombre_interfaz>`**: Especifica la interfaz de red a monitorizar (por ejemplo, `eth0` o `wlan0`).
- **`port <nº_puerto>`**: Filtra el tráfico para capturar solo el que pasa por el puerto indicado.

### 2. **tcptrack**
`tcptrack` es una herramienta de monitorización en tiempo real que muestra conexiones TCP activas, direcciones IP origen y destino, puertos, estado de la conexión y cantidad de datos transmitidos en un formato visual.

#### Opciones:
- **`-i <nombre_interfaz>`**: Permite especificar la interfaz de red a monitorizar.

### 3. **iptraf-ng**
`iptraf-ng` es una herramienta interactiva que proporciona estadísticas detalladas sobre el tráfico de red en tiempo real.

#### Opciones:
- La interfaz gráfica de `iptraf-ng` permite seleccionar diferentes tipos de monitorización, como ver estadísticas generales, por protocolo o flujos de red específicos.

### 4. **netstat**
`netstat` es una herramienta clásica para inspeccionar conexiones de red, sockets y estadísticas del sistema.

#### Opciones:
- **`-a`**: Muestra todas las conexiones y puertos de escucha, incluyendo las conexiones activas y los puertos en espera de conexiones.
- **`-n`**: Muestra las direcciones IP y los números de puerto en formato numérico, sin realizar la resolución de nombres de host.
- **`-tp`**: Muestra las conexiones TCP activas junto con los PID y los nombres de los procesos que las están utilizando.
- **`-l`**: Muestra únicamente las conexiones que están en estado de "escucha", es decir, los puertos que están esperando recibir conexiones entrantes.
