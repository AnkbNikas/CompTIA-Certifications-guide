## **Guía de Estudio para la Certificación CompTIA Linux+ (XK0-005)**

---

### **1. Introducción a Linux**
- **¿Qué es Linux?**
  - Sistema operativo de código abierto basado en Unix.
  - Desarrollado por Linus Torvalds en 1991.
  - Licenciado bajo GPL (General Public License).

- **Distribuciones (Distros)**:
  - **Ubuntu**: Ideal para principiantes y entornos de escritorio.
  - **Debian**: Conocida por su estabilidad.
  - **CentOS/RHEL**: Ampliamente utilizada en servidores empresariales.
  - **Fedora**: Versión comunitaria de RHEL.
  - **Arch Linux**: Para usuarios avanzados, enfoque en personalización.

- **Componentes clave**:
  - **Kernel**: Núcleo del sistema operativo.
  - **Shell**: Intérprete de comandos (Bash, Zsh, etc.).
  - **Sistema de archivos**: Jerarquía de directorios y tipos de sistemas de archivos (ext4, XFS, Btrfs).

---

### **2. Comandos Esenciales de Linux**
- **Estructura de comandos**:
  - Formato: `comando [opciones] [argumentos]`.
  - Ejemplo: `ls -l /home`.

- **Comandos básicos**:
  - `ls`: Listar archivos y directorios.
  - `cd`: Cambiar de directorio.
  - `pwd`: Mostrar el directorio actual.
  - `mkdir`: Crear directorios.
  - `rm`: Eliminar archivos o directorios.
  - `cp`: Copiar archivos.
  - `mv`: Mover o renombrar archivos.
  - `cat`: Mostrar contenido de archivos.
  - `grep`: Buscar patrones en archivos.
  - `find`: Buscar archivos y directorios.

- **Comandos avanzados**:
  - `awk`: Procesamiento de texto.
  - `sed`: Edición de flujos de texto.
  - `tar`: Comprimir y descomprimir archivos.
  - `rsync**: Sincronizar archivos y directorios.

---

### **3. Sistema de Archivos y Gestión de Discos**
- **Estructura del sistema de archivos**:
  - `/`: Directorio raíz.
  - `/home`: Directorios de usuarios.
  - `/etc`: Archivos de configuración.
  - `/var`: Archivos variables (logs, bases de datos).
  - `/bin` y `/sbin`: Comandos esenciales del sistema.
  - `/dev`: Dispositivos del sistema.
  - `/proc`: Información del sistema y procesos.

- **Gestión de discos**:
  - Comandos: `fdisk`, `lsblk`, `parted`.
  - Sistemas de archivos: ext4, XFS, Btrfs.
  - Montaje: `mount`, `/etc/fstab`.

---

### **4. Administración de Usuarios y Grupos**
- **Archivos clave**:
  - `/etc/passwd`: Información de usuarios.
  - `/etc/shadow`: Contraseñas de usuarios.
  - `/etc/group`: Información de grupos.

- **Comandos**:
  - `useradd`: Crear usuarios.
  - `usermod`: Modificar usuarios.
  - `userdel`: Eliminar usuarios.
  - `groupadd`: Crear grupos.
  - `passwd`: Cambiar contraseñas.

- **Permisos y propiedad**:
  - `chmod`: Cambiar permisos (ej. `chmod 755 archivo`).
  - `chown`: Cambiar propietario (ej. `chown usuario:grupo archivo`).
  - `umask`: Establecer permisos por defecto.

---

### **5. Redes en Linux**
- **Configuración de red**:
  - Comandos: `ifconfig`, `ip`, `ping`, `netstat`, `ss`.
  - Archivos de configuración: `/etc/network/interfaces`, `/etc/hosts`.

- **Herramientas**:
  - `ssh`: Conexión remota segura.
  - `scp`: Copiar archivos de forma segura.
  - `ftp`: Transferencia de archivos.
  - `nslookup` y `dig`: Resolución de DNS.

---

### **6. Seguridad en Linux**
- **Firewall**:
  - `iptables`: Configuración de reglas de firewall.
  - `ufw`: Interfaz simplificada para `iptables`.

- **Autenticación**:
  - Claves SSH: Generar con `ssh-keygen`.
  - Autenticación de dos factores (2FA).

- **Auditoría**:
  - `auditd`: Herramienta de auditoría del sistema.
  - Revisión de logs en `/var/log`.

---

### **7. Automatización y Scripting**
- **Shell scripting**:
  - Crear scripts en Bash.
  - Ejemplo básico:
    ```bash
    #!/bin/bash
    echo "Hola, mundo!"
    ```

- **Cron**:
  - Programar tareas con `crontab -e`.
  - Ejemplo: `0 * * * * /ruta/al/script.sh`.

---

### **8. Virtualización y Contenedores**
- **Virtualización**:
  - Herramientas: KVM, VirtualBox.
  - Comandos: `virsh`, `virt-manager`.

- **Contenedores**:
  - Docker: Crear y gestionar contenedores.
  - Kubernetes: Orquestación de contenedores.

---

### **9. Solución de Problemas**
- **Logs**:
  - Revisar archivos en `/var/log`.
  - Herramientas: `dmesg`, `journalctl`.

- **Rendimiento**:
  - Comandos: `top`, `htop`, `vmstat`, `iostat`.

---

### **10. Buenas Prácticas**
- Realizar copias de seguridad periódicas.
- Usar permisos y roles adecuados.
- Monitorear el rendimiento del sistema.
- Mantener el sistema actualizado.
