# Monitorización de Almacenamiento

La **monitorización de almacenamiento** consiste en supervisar el uso y rendimiento de los dispositivos de almacenamiento, como discos duros y SSD, para garantizar un funcionamiento óptimo del sistema y prevenir problemas como la falta de espacio o fallos de hardware.

## 1. Uso de espacio en disco
   - Se monitoriza cuánto espacio está siendo utilizado y cuánto queda disponible. Esto ayuda a evitar quedarse sin espacio, lo que podría afectar el funcionamiento del sistema.

## 2. Rendimiento del disco
   - Se supervisa la velocidad de lectura y escritura en el disco, así como la latencia (tiempo de respuesta) y las operaciones de entrada/salida (I/O). Esto es clave para identificar cuellos de botella que puedan reducir el rendimiento general del sistema.

## 3. Comandos
### 3.1 Comando `free` (Memoria RAM)  
El comando `free` muestra información sobre el uso de la memoria RAM (libre y utilizada).  

**Opciones comunes**:  
- `-h`: Muestra la información en formato legible (human-readable).  
- `-t`: Incluye el total de memoria.  
- `-s [segundos]`: Actualiza la información cada cierto tiempo.
![free.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/Free.png)

---

### 3.2 Comando `df` (Espacio en Disco)  
El comando `df` permite conocer el uso y la disponibilidad del espacio en los sistemas de archivos (espacio de disco libre y utilizado).  

**Opciones comunes**:  
- `-h`: Muestra los valores en un formato legible.
- `-T`: Muestra el tipo de sistema de archivos.  
- `-x [tipo]`: Excluye un tipo específico de sistema de archivos.  
![df.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/Df.png)
---

### 3.3 Comando `du` (Uso de Espacio en Directorios)  
El comando `du` calcula el espacio ocupado por directorios y archivos concretos.  
![du.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/Comando%20du.png)  
**Uso básico**:  
- `-h`: Muestra el tamaño de los archivos y directorios en un formato legible para los humanos,
  ![du -h.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/Du%20-h.png)
- `-s` : Muestra solo el total del espacio utilizado por un directorio o archivo
- `- d` : Especifica la profundidad del nivel de directorios que se quiere analizar
  ![du -s y -d.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/Du%20-s%20y%20-d.png)

---
### 3.4 El comando iostat: Estadísticas de CPU y Disco
El comando `iostat` forma parte del paquete sysstat y ofrece
información estadística sobre el uso del procesador y la actividad
de los dispositivos de almacenamiento. 

**Uso básico**:  
- `-x`: Muestra estadísticas detalladas sobre los dispositivos de almacenamiento.
- `-d` : Muestra estadísticas de los dispositivos de disco específicos.
- `- c` : Muestra estadísticas relacionadas con el uso de la CPU.
![iostat.png](https://github.com/N1tr0Zeu5/Monitorizacion/blob/main/Img*/Monitorizacion/Almacenamiento/iostat.png)


> [!NOTE]
> Conclusion: -free: Monitorea el estado de la memoria RAM y swap. -df: Verifica el espacio disponible en disco. -du: Identifica directorios que consumen mucho espacio. -iostat: Analiza el rendimiento del CPU y los discos. 
