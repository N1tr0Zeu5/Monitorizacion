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
- `-h` 
- `-s`
- `- d` 

---
### 1.4 El comando iostat: Estadísticas de CPU y Disco
El comando iostat forma parte del paquete sysstat y ofrece
información estadística sobre el uso del procesador y la actividad
de los dispositivos de almacenamiento. 

**Uso básico**:  
- `-x` 
- `-d`
- `- c`

**Nota**: Recuerda instalar el paquete antes de usar el comando.
