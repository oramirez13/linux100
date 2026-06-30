# Guía de comandos básicos de Linux y Arch Linux

## 1. Información del sistema

| Comando       | Explicación                                                              |
| ------------- | ------------------------------------------------------------------------ |
| `uname -a`    | Muestra información completa del kernel y del sistema.                   |
| `hostname`    | Muestra el nombre del equipo.                                            |
| `hostnamectl` | Muestra información detallada del sistema y permite cambiar el hostname. |
| `arch`        | Muestra la arquitectura del sistema.                                     |
| `lscpu`       | Muestra información del procesador.                                      |
| `free -h`     | Muestra el uso de memoria RAM y swap.                                    |
| `uptime`      | Muestra el tiempo que lleva encendido el sistema.                        |
| `date`        | Muestra la fecha y hora actual.                                          |
| `whoami`      | Muestra el usuario actual.                                               |
| `id`          | Muestra el UID, GID y grupos del usuario.                                |

---

# 2. Navegación por el sistema de archivos

| Comando  | Explicación                                             |
| -------- | ------------------------------------------------------- |
| `pwd`    | Muestra el directorio actual.                           |
| `ls`     | Lista el contenido del directorio.                      |
| `ls -la` | Lista todos los archivos con detalles.                  |
| `cd`     | Cambia de directorio.                                   |
| `tree`   | Muestra la estructura de directorios en forma de árbol. |
| `mkdir`  | Crea un directorio.                                     |
| `rmdir`  | Elimina un directorio vacío.                            |
| `touch`  | Crea un archivo vacío.                                  |
| `cp`     | Copia archivos o directorios.                           |
| `mv`     | Mueve o renombra archivos.                              |
| `rm`     | Elimina archivos o directorios.                         |
| `find`   | Busca archivos y directorios.                           |
| `locate` | Busca archivos usando una base de datos indexada.       |

---

# 3. Visualización de archivos

| Comando   | Explicación                                  |
| --------- | -------------------------------------------- |
| `cat`     | Muestra el contenido completo de un archivo. |
| `less`    | Visualiza archivos página por página.        |
| `head`    | Muestra las primeras líneas de un archivo.   |
| `tail`    | Muestra las últimas líneas de un archivo.    |
| `tail -f` | Sigue un archivo en tiempo real.             |
| `file`    | Identifica el tipo de archivo.               |
| `stat`    | Muestra información detallada de un archivo. |

---

# 4. Búsqueda y procesamiento de texto

| Comando   | Explicación                             |
| --------- | --------------------------------------- |
| `grep`    | Busca texto mediante patrones.          |
| `grep -r` | Busca texto de forma recursiva.         |
| `awk`     | Procesa texto por columnas.             |
| `sed`     | Edita y transforma texto.               |
| `cut`     | Extrae columnas de texto.               |
| `sort`    | Ordena líneas.                          |
| `uniq`    | Elimina líneas duplicadas consecutivas. |
| `tr`      | Sustituye caracteres.                   |
| `wc`      | Cuenta líneas, palabras y caracteres.   |

---

# 5. Permisos

| Comando | Explicación                                    |
| ------- | ---------------------------------------------- |
| `chmod` | Cambia los permisos de archivos y directorios. |
| `chown` | Cambia el propietario.                         |
| `chgrp` | Cambia el grupo propietario.                   |
| `umask` | Define los permisos por defecto.               |

---

# 6. Usuarios

| Comando  | Explicación                                       |
| -------- | ------------------------------------------------- |
| `who`    | Muestra usuarios conectados.                      |
| `w`      | Muestra usuarios y procesos activos.              |
| `groups` | Muestra los grupos del usuario.                   |
| `passwd` | Cambia la contraseña de un usuario.               |
| `sudo`   | Ejecuta comandos con privilegios administrativos. |
| `visudo` | Edita de forma segura el archivo sudoers.         |

---

# 7. Procesos

| Comando   | Explicación                          |
| --------- | ------------------------------------ |
| `ps`      | Muestra procesos en ejecución.       |
| `ps aux`  | Lista todos los procesos.            |
| `top`     | Monitor de procesos en tiempo real.  |
| `htop`    | Monitor de procesos interactivo.     |
| `kill`    | Finaliza un proceso mediante su PID. |
| `killall` | Finaliza procesos por nombre.        |
| `pgrep`   | Busca procesos por nombre.           |
| `pkill`   | Finaliza procesos por nombre.        |

---

# 8. Servicios (systemd)

| Comando                      | Explicación                       |
| ---------------------------- | --------------------------------- |
| `systemctl status servicio`  | Muestra el estado de un servicio. |
| `systemctl start servicio`   | Inicia un servicio.               |
| `systemctl stop servicio`    | Detiene un servicio.              |
| `systemctl restart servicio` | Reinicia un servicio.             |
| `systemctl enable servicio`  | Activa el inicio automático.      |
| `systemctl disable servicio` | Desactiva el inicio automático.   |

---

# 9. Logs

| Comando          | Explicación                                |
| ---------------- | ------------------------------------------ |
| `journalctl`     | Muestra los registros del sistema.         |
| `journalctl -b`  | Muestra los registros del arranque actual. |
| `journalctl -xe` | Muestra errores recientes.                 |
| `journalctl -f`  | Sigue el log en tiempo real.               |
| `dmesg`          | Muestra mensajes del kernel.               |

---

# 10. Redes

| Comando     | Explicación                                |
| ----------- | ------------------------------------------ |
| `ip addr`   | Muestra las interfaces de red.             |
| `ip route`  | Muestra la tabla de rutas.                 |
| `ping`      | Comprueba conectividad con un host.        |
| `ss -tulnp` | Muestra puertos abiertos y conexiones.     |
| `curl`      | Realiza peticiones HTTP.                   |
| `wget`      | Descarga archivos desde Internet.          |
| `dig`       | Consulta registros DNS.                    |
| `host`      | Resuelve nombres DNS.                      |
| `nmcli`     | Gestiona NetworkManager desde la terminal. |

---

# 11. SSH

| Comando            | Explicación                         |
| ------------------ | ----------------------------------- |
| `ssh usuario@host` | Conecta a un servidor remoto.       |
| `scp`              | Copia archivos mediante SSH.        |
| `sftp`             | Transfiere archivos mediante SSH.   |
| `ssh-keygen`       | Genera claves SSH.                  |
| `ssh-copy-id`      | Copia la clave pública al servidor. |

---

# 12. Discos

| Comando          | Explicación                                 |
| ---------------- | ------------------------------------------- |
| `lsblk`          | Lista discos y particiones.                 |
| `df -h`          | Muestra el espacio en disco.                |
| `du -sh carpeta` | Muestra el tamaño de una carpeta.           |
| `blkid`          | Muestra UUID y tipo de sistema de archivos. |
| `mount`          | Monta un sistema de archivos.               |
| `umount`         | Desmonta un sistema de archivos.            |

---

# 13. Compresión

| Comando  | Explicación                |
| -------- | -------------------------- |
| `tar`    | Empaqueta archivos.        |
| `gzip`   | Comprime archivos.         |
| `gunzip` | Descomprime archivos GZIP. |
| `zip`    | Comprime en formato ZIP.   |
| `unzip`  | Extrae archivos ZIP.       |

---

# 14. Administración de paquetes (Arch Linux)

## Pacman

| Comando               | Explicación                                     |
| --------------------- | ----------------------------------------------- |
| `pacman -Syu`         | Actualiza completamente el sistema.             |
| `pacman -S paquete`   | Instala un paquete.                             |
| `pacman -R paquete`   | Elimina un paquete.                             |
| `pacman -Rns paquete` | Elimina un paquete y dependencias innecesarias. |
| `pacman -Qs nombre`   | Busca paquetes instalados.                      |
| `pacman -Qi paquete`  | Muestra información de un paquete.              |
| `pacman -Q`           | Lista todos los paquetes instalados.            |
| `pacman -Sc`          | Limpia la caché de paquetes.                    |

## Yay

| Comando            | Explicación                                                 |
| ------------------ | ----------------------------------------------------------- |
| `yay -Syu`         | Actualiza paquetes oficiales y del AUR.                     |
| `yay -S paquete`   | Instala un paquete del AUR o de los repositorios oficiales. |
| `yay -Rns paquete` | Elimina un paquete y sus dependencias.                      |
| `yay -Qs nombre`   | Busca paquetes.                                             |

---

# 15. Auditoría y seguridad

| Comando      | Explicación                            |
| ------------ | -------------------------------------- |
| `auditctl`   | Administra las reglas de auditoría.    |
| `ausearch`   | Busca eventos registrados por auditd.  |
| `aureport`   | Genera informes de auditoría.          |
| `journalctl` | Revisa eventos del sistema.            |
| `sha256sum`  | Calcula el hash SHA-256 de un archivo. |
| `gpg`        | Firma y cifra archivos.                |

---

# 16. Diagnóstico

| Comando   | Explicación                                    |
| --------- | ---------------------------------------------- |
| `lsof`    | Lista archivos abiertos por procesos.          |
| `strace`  | Muestra las llamadas al sistema de un proceso. |
| `tcpdump` | Captura tráfico de red.                        |
| `vmstat`  | Muestra estadísticas de memoria y CPU.         |
| `iostat`  | Muestra estadísticas de discos.                |

---

# 17. Ayuda

| Comando           | Explicación                                        |
| ----------------- | -------------------------------------------------- |
| `man comando`     | Abre el manual del comando.                        |
| `comando --help`  | Muestra la ayuda rápida del comando.               |
| `info comando`    | Abre la documentación GNU si está disponible.      |
| `apropos palabra` | Busca comandos relacionados con una palabra clave. |
