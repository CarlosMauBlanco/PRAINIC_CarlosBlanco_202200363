
# 📘 Manual de Instalación y Configuración de Linux Mint en VirtualBox

Este documento describe el procedimiento completo para instalar **Linux Mint** en una máquina virtual usando **VirtualBox** en Windows, sin eliminar el sistema operativo Windows, y detalla las configuraciones posteriores y soluciones a problemas encontrados.

---

## 1. 💻 Sobre Linux Mint
Linux Mint es una distribución de **GNU/Linux** basada en Ubuntu y Debian, diseñada para ser fácil de usar, estable y eficiente.  
Características principales:
- **Entorno de escritorio Cinnamon, MATE o XFCE**.
- Basada en Ubuntu LTS para estabilidad y soporte prolongado.
- Soporte para una gran variedad de software libre y propietario.
- Sistema ligero y adaptable a computadoras con pocos recursos.

**Beneficios:**
- Interfaz amigable para usuarios nuevos en Linux.
- Excelente soporte de hardware.
- Seguridad y actualizaciones frecuentes.
- Comunidad activa y documentación abundante.

---

## 2. 🌐 Cómo conseguir Linux Mint
La distribución puede descargarse desde el sitio oficial:
🔗 [https://linuxmint.com/download.php](https://linuxmint.com/download.php)

**Pasos para descargar:**
1. Ingresar a la página oficial.
2. Elegir la versión deseada (recomendado Cinnamon para usuarios nuevos).
3. Seleccionar un **mirror** cercano a tu ubicación para una descarga más rápida.
4. Descargar el archivo `.iso`.
5. (Opcional) Verificar la integridad de la descarga usando el hash SHA256 provisto en la web.

---

## 3. 🖥️ Instalando Linux Mint en VirtualBox
> **Objetivo:** Mantener Windows como sistema principal y ejecutar Linux Mint de forma virtualizada.

**Pasos:**
1. Descargar e instalar **VirtualBox** desde [https://www.virtualbox.org/](https://www.virtualbox.org/).
2. Abrir VirtualBox y hacer clic en **"Nueva"**.
3. Asignar un nombre a la máquina virtual, elegir **Tipo: Linux** y **Versión: Ubuntu (64-bit)**.
4. Asignar memoria RAM (recomendado: 4096 MB mínimo).
5. Crear un disco duro virtual (VDI) con al menos 20 GB.
6. Seleccionar el archivo `.iso` de Linux Mint en **Configuración > Almacenamiento > Controlador IDE**.
7. Iniciar la máquina virtual.
8. En el instalador de Linux Mint:
   - Seleccionar idioma.
   - Configurar teclado.
   - Elegir instalación normal.
   - Seleccionar instalación en disco virtual (no afecta Windows).
   - Configurar usuario y contraseña.
9. Finalizar instalación y reiniciar.

---

## 4. ⚙️ Configuración Posterior
Después de la instalación, realizar:
- **Actualización del sistema:**  
  ```bash
  sudo apt update && sudo apt upgrade -y
  ```
- **Instalar Guest Additions** para mejor integración con Windows (pantalla completa, carpetas compartidas, portapapeles bidireccional).
- **Configurar red:** Asegurar que la VM esté en modo **Adaptador puente** o **NAT** para conexión a Internet.
- **Configurar idioma y zona horaria** en **Configuración del sistema**.
- **Instalar software necesario** desde el Gestor de Software.

---

## 5. 🛠️ Ayuda y Solución de Problemas
**Problemas encontrados y soluciones:**
- **No detecta el archivo ISO:** Verificar que esté seleccionado en Configuración > Almacenamiento.
- **Pantalla pequeña:** Instalar Guest Additions (`Devices > Insert Guest Additions CD image`).
- **Sin Internet:** Cambiar el adaptador de red a **NAT** o **puente**.
- **Teclado incorrecto:** Ajustar en Configuración > Teclado.

**Fuentes de documentación utilizadas:**
- [Documentación oficial de Linux Mint](https://linuxmint.com/documentation.php)
- [Manual de VirtualBox](https://www.virtualbox.org/manual/)
- Comunidad de foros de Linux Mint y Stack Overflow.

---
## 7. 🎥 Videos de referencia

[🔗 Ver tutorial en YouTube](https://youtu.be/UorI5IJ44WE)


✍️ Autores: Carlos Mauricio Blanco Valencia  
✍️ Autores: Marvin Francisco Paz Linares  
📅 Fecha: 12/08/2025
