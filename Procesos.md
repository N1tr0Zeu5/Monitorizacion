
# Monitorización de Procesos

## 1. Comando ps
El comando `ps` proporciona una instantánea de los procesos en ejecución. Es útil para obtener información específica sobre procesos.

### Opciones comunes:
- `ps`: Muestra los procesos del terminal actual.
- `ps a`: Muestra todos los procesos del sistema.
- `ps aux`: Muestra todos los procesos, incluyendo aquellos sin terminal asociado.
- `ps -C <comando>`: Muestra los procesos que coinciden con el nombre del comando dado.

## 2. Comando top
El comando `top` permite monitorizar el sistema en tiempo real y detectar procesos que consumen muchos recursos, proporcionando una vista dinámica y en tiempo real de los procesos en ejecución y el uso de recursos del sistema (CPU, memoria y procesos en ejecución).

### Opciones comunes:
- `top T`: Ordena los procesos por tiempo de ejecución.
- `top M`: Ordena los procesos por uso de memoria.
- `top P`: Ordena los procesos por uso de CPU.
- `top p <PID>`: Muestra solo el proceso con el PID especificado.
- `top R`: Muestra los procesos en orden inverso.
- `top U <usuario>`: Muestra los procesos de un usuario específico.
- `top q`: Salir del comando `top` rápidamente.
- `top k`: Permite terminar un proceso especificando su PID.

### ¿Qué es el PID?
El PID (Process ID o Identificador de Proceso) es un número único asignado por el sistema operativo a cada proceso en ejecución. Este identificador permite al sistema y a los administradores distinguir y gestionar procesos individuales.

## 3. Comando htop
`htop` es una versión mejorada y más amigable de `top`, con una interfaz interactiva y funcionalidad adicional.

### Opciones:
- `htop -u <usuario>`: Muestra los procesos de un usuario específico.
- `htop --tree`: Muestra los procesos en una vista jerárquica (árbol).
- `htop -p <PID1,PID2>`: Muestra solo los procesos especificados por sus PIDs.

### Atajos de Teclado:
- F2 (Setup) - Configuración
- F3 (Search) - Búsqueda
- F4 (Filter) - Filtro
- F5 (Tree) - Vista en árbol
- F6 (Sort) - Ordenar
- F9 (Kill) - Terminar un Proceso

## 4. Comando atop
`atop` es una herramienta avanzada para monitorizar no solo procesos, sino también otros recursos del sistema, como disco, red y memoria.

### Uso básico:
- Ejecutar en tiempo real: Muestra información detallada del sistema en tiempo real.
- Consultar registros guardados: Permite ver información histórica de los registros guardados.
