## 1. Monitorización del Almacenamiento  

### 1.1 Comando `free` (Memoria RAM)  
El comando `free` muestra información sobre el uso de la memoria RAM (libre y utilizada).  

**Opciones comunes**:  
- `-h`: Muestra la información en formato legible (human-readable).  
- `-t`: Incluye el total de memoria.  
- `-s [segundos]`: Actualiza la información cada cierto tiempo.  

---

### 1.2 Comando `df` (Espacio en Disco)  
El comando `df` permite conocer el uso y la disponibilidad del espacio en los sistemas de archivos (espacio de disco libre y utilizado).  

**Opciones comunes**:  
- `-h`: Muestra los valores en un formato legible.  
- `-T`: Muestra el tipo de sistema de archivos.  
- `-x [tipo]`: Excluye un tipo específico de sistema de archivos.  

---

### 1.3 Comando `du` (Uso de Espacio en Directorios)  
El comando `du` calcula el espacio ocupado por directorios y archivos concretos.  

**Uso básico**:  
- `-h`: Muestra el tamaño de los archivos y directorios en un formato legible para los humanos, 
- `-s` : Muestra solo el total del espacio utilizado por un directorio o archivo
- `- d` : Especifica la profundidad del nivel de directorios que se quiere analizar

---
### 1.4 El comando iostat: Estadísticas de CPU y Disco
El comando iostat forma parte del paquete sysstat y ofrece
información estadística sobre el uso del procesador y la actividad
de los dispositivos de almacenamiento. 

**Uso básico**:  
- `-x`: Muestra estadísticas detalladas sobre los dispositivos de almacenamiento.
- `-d` : Muestra estadísticas de los dispositivos de disco específicos.
- `- c` : Muestra estadísticas relacionadas con el uso de la CPU.

> [!NOTE]
> Conclusion: -free: Monitorea el estado de la memoria RAM y swap. -df: Verifica el espacio disponible en disco. -du: Identifica directorios que consumen mucho espacio. -iostat: Analiza el rendimiento del CPU y los discos. 
