# 📡 Manual de Configuración y Conexión de Redes

Este manual describe los conceptos, configuraciones y procedimientos para trabajar con **redes cableadas e inalámbricas** entre distintos sistemas operativos. Incluye materiales, configuraciones paso a paso, problemas comunes y consejos útiles.

---

## 1. 🖧 Redes Cableadas
Las **redes cableadas** utilizan cables físicos (como Ethernet) para conectar dispositivos, garantizando **estabilidad**, **alta velocidad** y **baja latencia**.

**Características principales:**
- Mayor velocidad que las redes inalámbricas.
- Más seguras al no emitir señales por el aire.
- Menor interferencia.
- Requieren infraestructura física.

**Ventajas:**
- Ideal para transferencias grandes de datos.
- Mejor rendimiento en juegos en línea y streaming.
- Menos propensas a caídas por interferencia.

**Desventajas:**
- Menos movilidad para los dispositivos.
- Instalación más costosa y complicada.

---

## 2. ⚙️ Configuración de Redes Cableadas

### 2.1 Windows ↔ Windows
1. Conectar ambos equipos con un cable Ethernet.
2. Asignar IP estática en ambos PCs:
   - **Equipo 1:** `192.168.1.1` – Máscara `255.255.255.0`
   - **Equipo 2:** `192.168.1.2` – Máscara `255.255.255.0`
3. Activar **uso compartido de archivos e impresoras**.
4. Compartir la carpeta deseada (click derecho → "Compartir con").
5. Acceder desde el otro equipo con `\IP_DEL_PC`.

### 2.2 Linux ↔ Linux
1. Conectar ambos equipos con un cable Ethernet.
2. Asignar IP manual en cada equipo desde "Configuración de red".
3. Instalar y configurar **Samba** o usar **Nemo** para compartir carpetas.
4. Desde el otro equipo, abrir el explorador de archivos y escribir:  
   `smb://IP_DEL_PC`

### 2.3 Windows ↔ Linux
1. Conectar ambos dispositivos con cable Ethernet.
2. Configurar IP estática en ambos.
3. En Linux, instalar **Samba** y compartir carpeta.
4. En Windows, abrir **Ejecutar (Win+R)** y escribir `\IP_DEL_PC`.

---

## 3. 📶 Redes Inalámbricas
Las **redes inalámbricas (Wi-Fi)** permiten la conexión sin cables usando ondas de radio.

**Características:**
- Movilidad total dentro del rango de la señal.
- Facilidad de conexión.
- Menor velocidad que una conexión cableada.
- Mayor susceptibilidad a interferencias.

**Ventajas:**
- Portabilidad.
- Fácil configuración.
- Compatibilidad con la mayoría de dispositivos.

**Desventajas:**
- Menor estabilidad.
- Riesgo de intrusión si no está bien protegida.

---

## 4. ⚙️ Configuración de Redes Inalámbricas

### 4.1 Windows ↔ Windows
1. Conectar ambos equipos a la misma red Wi-Fi.
2. Activar **uso compartido de archivos**.
3. Compartir la carpeta deseada.
4. Acceder mediante `\NOMBRE_PC` o `\IP_DEL_PC`.

### 4.2 Linux ↔ Linux
1. Conectar ambos equipos a la misma red Wi-Fi.
2. Instalar **Samba** o usar **Nemo**.
3. Compartir carpeta y acceder desde el otro equipo con `smb://IP_DEL_PC`.

### 4.3 Windows ↔ Linux
1. Conectar ambos equipos a la misma red inalámbrica.
2. En Linux, habilitar Samba y compartir carpeta.
3. En Windows, acceder por `\IP_DEL_PC`.

---

## 5. 🆘 Ayuda y Solución de Problemas

**Problema:** No puedo acceder a la carpeta compartida.  
**Solución:** Verificar que ambos equipos estén en el mismo rango IP y que el firewall permita el tráfico SMB.

**Problema:** Error de permisos.  
**Solución:** Cambiar permisos de carpeta a "Lectura y escritura" para "Otros".

**Problema:** No aparece el equipo en la red.  
**Solución:** Usar la IP en vez del nombre del PC.

---

## 6. 📚 Fuentes y Recursos
- **Documentación oficial de Samba**
- Tutoriales de Ubuntu y Linux Mint
- Foros de Microsoft y Linux.org

-  **Libros**
- Guía Práctica de Redes LAN (2023)
- *Redes de Computadoras – Tanenbaum*
---
## 7. 🎥 Videos de referencia

[🔗 Ver tutorial en YouTube](https://www.youtube.com/watch?v=rGwhYPmcLeM)


✍️ Autores: Carlos Mauricio Blanco Valencia  
✍️ Autores: Marvin Francisco Paz Linares  
📅 Fecha: 12/08/2025
