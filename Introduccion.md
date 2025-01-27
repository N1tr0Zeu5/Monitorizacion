![Monitorización del sistema](https://solucions-im.com/media/images/Blog/monitoritzacio-sistemes-8-passos.jpg)
# Monitorización del Sistema mediante Comandos

La monitorización del sistema mediante comandos se refiere al uso de herramientas y utilidades de línea de comandos para supervisar el estado y rendimiento de un sistema operativo, sus recursos y servicios. Es especialmente útil en sistemas Linux/Unix, pero también puede aplicarse en Windows con herramientas específicas.

## Aspectos que se pueden supervisar:
- **Uso de CPU**: Qué porcentaje de los núcleos se está utilizando.
- **Memoria RAM**: Uso total, libre y disponible de la memoria.
- **Almacenamiento**: Espacio ocupado y libre en discos duros o particiones.
- **Procesos**: Procesos en ejecución, sus estados y consumo de recursos.
- **Red**: Velocidad de transferencia, conexiones activas y errores.

---

## Comandos comunes en Linux para monitorizar:

### 1. CPU y memoria:
- `top` / `htop`: Proporciona una visión en tiempo real de los procesos que consumen más recursos,
como la CPU y la memoria.
- `ps`: Muestra información de los procesos activos.
- `atop`: Registra e informa de la actividad de todos los procesos del servidor.

### 2. Disco y almacenamiento:
- `free`: Muestra la cantidad de memoria libre y utilizada en el sistema
- `df`: Muestra el espacio utilizado y disponible en los sistemas d .
- `du `: Muestra el espacio ocupado por un fichero o directorio..
- `iostat`: Se utiliza para rastrear los problemas de rendimiento de los dispositivos de
almacenamiento.

### 3. Procesos:
- `ps`: Muestra los procesos en ejecución.
- `kill` o `pkill`: Finaliza procesos específicos.

### 4. Red:
- ` tcpdump`: Permite capturar y analizar el tráfico de red que pasa a
través de una interfaz de red
- `tcptrack` : Herramienta de monitorización en tiempo real
que muestra conexiones TCP activas
- `netstat`: Es una herramienta clásica para inspeccionar conexiones
de red, sockets y estadísticas.
- ` iptraf-ng`: Es una herramienta interactiva que proporciona
estadísticas detalladas sobre el tráfico de red en tiempo real.

---

## Ventajas:
- **Ligero**: Consume pocos recursos.
- **Rápido**: Responde en tiempo real.
- **Detallado**: Permite personalizar las salidas.
- **Automatizable**: Se puede integrar con scripts.

---
