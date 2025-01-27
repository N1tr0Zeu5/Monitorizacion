# Monitorización de Procesos

La **monitorización de procesos** es la supervisión de los procesos en ejecución en un sistema operativo, para conocer su estado, uso de recursos y rendimiento. Esto es esencial para garantizar que los procesos no afecten la estabilidad del sistema y para detectar posibles problemas antes de que se conviertan en fallos graves.

## 1. Uso de recursos por proceso
   - **CPU**: Se monitoriza el tiempo que un proceso utiliza de la unidad de procesamiento central. Un alto consumo de CPU puede afectar el rendimiento general del sistema.
   - **Memoria**: Se supervisa la cantidad de memoria utilizada por cada proceso. Un uso excesivo de memoria puede agotar los recursos y causar ralentización o fallos.

## 2. Estado de los procesos
   - Los procesos pueden estar en diferentes estados como **ejecutándose**, **esperando**, **suspendidos** o **terminados**. Monitorizar estos estados permite detectar bloqueos o procesos inactivos.

## Beneficios de la monitorización de procesos
   - **Optimización de recursos**: Permite identificar procesos ineficientes que consumen recursos excesivamente, optimizando el rendimiento.
   - **Detección de problemas**: Ayuda a identificar problemas como procesos bloqueados o errores de rendimiento.
   - **Prevención de fallos**: La monitorización continua permite prever y prevenir problemas antes de que afecten gravemente al sistema.

# 3 Comandos
## 3.1 Comando ps
El comando `ps` proporciona una instantánea de los procesos en ejecución. Es útil para obtener información específica sobre procesos.

### Opciones comunes:
- `ps`: Muestra los procesos del terminal actual.
- `ps a`: Muestra todos los procesos del sistema.
- `ps aux`: Muestra todos los procesos, incluyendo aquellos sin terminal asociado.
![ps -a aux.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/ps%2C%20-a%20aux.png)
- `ps -C <comando>`: Muestra los procesos que coinciden con el nombre del comando dado.
![ps -c.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/ps%20-c.png)

## 3.2 Comando top
El comando `top` permite monitorizar el sistema en tiempo real y detectar procesos que consumen muchos recursos, proporcionando una vista dinámica y en tiempo real de los procesos en ejecución y el uso de recursos del sistema (CPU, memoria y procesos en ejecución).  
![Top.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/Top.png)

### Opciones comunes:
- `top T`: Ordena los procesos por tiempo de ejecución.
![top t.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/top%20f.png)
- `top M`: Ordena los procesos por uso de memoria.
![top m.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/top%20m.png)
- `top P`: Ordena los procesos por uso de CPU.
- `top p <PID>`: Muestra solo el proceso con el PID especificado.
- `top R`: Muestra los procesos en orden inverso.
- `top U <usuario>`: Muestra los procesos de un usuario específico.
- `top q`: Salir del comando `top` rápidamente.
- `top k`: Permite terminar un proceso especificando su PID.

### ¿Qué es el PID?
El PID (Process ID o Identificador de Proceso) es un número único asignado por el sistema operativo a cada proceso en ejecución. Este identificador permite al sistema y a los administradores distinguir y gestionar procesos individuales.

## 3.3 Comando htop
`htop` es una versión mejorada y más amigable de `top`, con una interfaz interactiva y funcionalidad adicional.  
![htop.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/htop.png)

### Opciones:
- `htop -u <usuario>`: Muestra los procesos de un usuario específico.
- `htop --tree`: Muestra los procesos en una vista jerárquica (árbol).
- `htop -p <PID1,PID2>`: Muestra solo los procesos especificados por sus PIDs.

### Atajos de Teclado:
- F2 (Setup) - Configuración
![htop f2.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/htop%20f2.png)
- F3 (Search) - Búsqueda
- F4 (Filter) - Filtro
- F5 (Tree) - Vista en árbol
![htop f5.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/htop%20f5.png)
- F6 (Sort) - Ordenar
- F9 (Kill) - Terminar un Proceso

## 3.4 Comando atop
`atop` es una herramienta avanzada para monitorizar no solo procesos, sino también otros recursos del sistema, como disco, red y memoria.
![atop.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Procesos/atop.png)

### Uso básico:
- Ejecutar en tiempo real: Muestra información detallada del sistema en tiempo real.
- Consultar registros guardados: Permite ver información histórica de los registros guardados.
