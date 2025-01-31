# Guía Completa de Comandos de Linux

Este archivo contiene una lista de los comandos básicos de Linux más utilizados junto con su explicación detallada. Es una referencia rápida para gestionar archivos, sistemas, redes y tareas comunes en un entorno Linux.

---

## Índice

1. [Comandos Básicos de Linux](#comandos-básicos-de-linux)
2. [Comandos de Gestión de Archivos](#comandos-de-gestión-de-archivos)
3. [Comandos de Gestión de Directorios](#comandos-de-gestión-de-directorios)
4. [Comandos de Gestión de Procesos](#comandos-de-gestión-de-procesos)
5. [Comandos de Red](#comandos-de-red)
6. [Comandos de Gestión de Usuarios y Permisos](#comandos-de-gestión-de-usuarios-y-permisos)
7. [Comandos de Compresión y Descompresión](#comandos-de-compresión-y-descompresión)
8. [Comandos de Manejo de Paquetes](#comandos-de-manejo-de-paquetes)

---

## Comandos Básicos de Linux

1. **`pwd`**  
   Muestra el directorio de trabajo actual.

2. **`cd <directorio>`**  
   Cambia al directorio especificado.

3. **`ls`**  
   Lista los archivos y directorios del directorio actual.

4. **`mkdir <directorio>`**  
   Crea un nuevo directorio.

5. **`rm <archivo>`**  
   Elimina un archivo específico.

6. **`rm -rf <directorio>`**  
   Elimina un directorio y su contenido de forma recursiva sin pedir confirmación.

7. **`cp <archivo_origen> <archivo_destino>`**  
   Copia un archivo de una ubicación a otra.

8. **`mv <archivo_origen> <archivo_destino>`**  
   Mueve un archivo de un directorio a otro o cambia su nombre.

9. **`cat <archivo>`**  
   Muestra el contenido de un archivo.

10. **`nano <archivo>`**  
    Abre un archivo en el editor de texto `nano`.

11. **`touch <archivo>`**  
    Crea un archivo vacío o actualiza la fecha de modificación de un archivo existente.

12. **`find <directorio> -name <nombre_archivo>`**  
    Busca un archivo dentro del directorio especificado.

13. **`locate <archivo>`**  
    Realiza una búsqueda rápida de archivos por su nombre en el sistema.

14. **`which <comando>`**  
    Muestra la ruta completa de un comando ejecutable.

15. **`file <archivo>`**  
    Muestra el tipo de archivo (texto, imagen, etc.).

---

## Comandos de Gestión de Archivos

1. **`chmod <permisos> <archivo>`**  
   Cambia los permisos de un archivo o directorio. Ejemplo: `chmod 755 archivo.sh` (lectura, escritura y ejecución para el propietario, solo lectura y ejecución para otros).

2. **`chown <usuario>:<grupo> <archivo>`**  
   Cambia el propietario y el grupo de un archivo o directorio.

3. **`tar -czf <archivo.tar.gz> <directorio>`**  
   Crea un archivo comprimido en formato `.tar.gz` del directorio especificado.

4. **`tar -xzf <archivo.tar.gz>`**  
   Extrae el contenido de un archivo `.tar.gz`.

5. **`zip <archivo.zip> <archivo_o_directorio>`**  
   Comprime un archivo o directorio en formato `.zip`.

6. **`unzip <archivo.zip>`**  
   Extrae los contenidos de un archivo `.zip`.

7. **`gzip <archivo>`**  
   Comprime un archivo utilizando el formato `.gz`.

8. **`gunzip <archivo.gz>`**  
   Descomprime un archivo `.gz`.

9. **`bzip2 <archivo>`**  
   Comprime un archivo usando el formato `.bz2`.

10. **`bunzip2 <archivo.bz2>`**  
    Descomprime un archivo `.bz2`.

---

## Comandos de Gestión de Directorios

1. **`cd ~`**  
   Cambia al directorio home del usuario.

2. **`cd ..`**  
   Cambia al directorio superior (padre) al directorio actual.

3. **`rmdir <directorio>`**  
   Elimina un directorio vacío.

4. **`ls -l`**  
   Muestra los archivos en formato detallado, incluyendo permisos, propietario, tamaño y fecha de modificación.

5. **`ls -a`**  
   Muestra todos los archivos, incluidos los ocultos (que comienzan con un punto).

6. **`ls -lh`**  
   Muestra los archivos en formato detallado con tamaños legibles por humanos (por ejemplo, KB, MB).

7. **`du -sh <directorio>`**  
   Muestra el tamaño total de un directorio.

8. **`du -ah <directorio>`**  
   Muestra el tamaño de todos los archivos dentro de un directorio.

---

## Comandos de Gestión de Procesos

1. **`ps`**  
   Muestra los procesos en ejecución en el sistema.

2. **`top`**  
   Muestra los procesos activos y su consumo de recursos en tiempo real.

3. **`htop`**  
   Versión mejorada de `top`, con interfaz interactiva.

4. **`kill <pid>`**  
   Envía una señal para terminar un proceso con el ID de proceso especificado.

5. **`killall <nombre_proceso>`**  
   Termina todos los procesos con el nombre especificado.

6. **`bg`**  
   Pone un proceso suspendido en segundo plano.

7. **`fg`**  
   Trae un proceso de segundo plano al primer plano.

8. **`sleep <tiempo>`**  
   Detiene la ejecución durante un número específico de segundos.

---

## Comandos de Red

1. **`ifconfig`**  
   Muestra las configuraciones de red del sistema.

2. **`ping <ip_o_dominio>`**  
   Envía paquetes ICMP para verificar la conectividad de red.

3. **`netstat`**  
   Muestra las conexiones de red, puertos y estadísticas de red.

4. **`ssh <usuario>@<ip>`**  
   Se conecta a un servidor remoto utilizando el protocolo SSH.

5. **`scp <archivo> <usuario>@<ip>:<directorio_destino>`**  
   Copia archivos entre sistemas de forma segura a través de SSH.

6. **`wget <url>`**  
   Descarga un archivo desde la web.

7. **`curl <url>`**  
   Realiza una solicitud HTTP o muestra el contenido de una URL.

8. **`netcat <ip> <puerto>`**  
   Realiza una conexión de red simple (herramienta útil para pruebas).

9. **`traceroute <ip_o_dominio>`**  
   Muestra el recorrido que siguen los paquetes a través de la red hasta llegar a su destino.

---

## Comandos de Gestión de Usuarios y Permisos

1. **`sudo <comando>`**  
   Ejecuta un comando con privilegios de superusuario.

2. **`useradd <nombre_usuario>`**  
   Crea un nuevo usuario en el sistema.

3. **`usermod -aG <grupo> <usuario>`**  
   Añade un usuario a un grupo.

4. **`passwd <usuario>`**  
   Cambia la contraseña de un usuario.

5. **`groupadd <nombre_grupo>`**  
   Crea un nuevo grupo.

6. **`whoami`**  
   Muestra el nombre de usuario actual.

7. **`id`**  
   Muestra la información de usuario, incluyendo el UID, GID y grupos.

8. **`groups`**  
   Muestra los grupos a los que pertenece el usuario actual.

9. **`chmod 777 <archivo>`**  
   Da todos los permisos (lectura, escritura y ejecución) a todos los usuarios.

10. **`chown root:root <archivo>`**  
    Cambia el propietario y el grupo del archivo a `root`.

---

## Comandos de Compresión y Descompresión

1. **`tar -cvf <archivo.tar> <directorio>`**  
   Crea un archivo tar del directorio especificado.

2. **`tar -xvf <archivo.tar>`**  
   Extrae el contenido de un archivo tar.

3. **`tar -czvf <archivo.tar.gz> <directorio>`**  
   Comprime un directorio en un archivo `.tar.gz`.

4. **`tar -xzvf <archivo.tar.gz>`**  
   Extrae el contenido de un archivo `.tar.gz`.

5. **`tar -cjvf <archivo.tar.bz2> <directorio>`**  
   Comprime un directorio en un archivo `.tar.bz2`.

6. **`tar -xjvf <archivo.tar.bz2>`**  
   Extrae el contenido de un archivo `.tar.bz2`.

---

## Comandos de Manejo de Paquetes

1. **`apt-get update`**  
   Actualiza la lista de paquetes disponibles (Ubuntu/Debian).

2. **`apt-get upgrade`**  
   Actualiza los paquetes instalados a sus últimas versiones disponibles (Ubuntu/Debian).

3. **`apt-get install <paquete>`**  
   Instala un paquete en el sistema (Ubuntu/Debian).

4. **`apt-get remove <paquete>`**  
   Elimina un paquete instalado (Ubuntu/Debian).

5. **`yum install <paquete>`**  
   Instala un paquete en sistemas basados en RedHat (CentOS, Fedora).

6. **`dnf install <paquete>`**  
   Instala un paquete en Fedora.

7. **`pacman -S <paquete>`**  
   Instala un paquete en Arch Linux.

---

## Conclusión

Esta guía contiene los comandos más utilizados para gestionar un sistema Linux, desde la administración de archivos y procesos hasta la red y la compresión de archivos. Es un excelente punto de partida para dominar el sistema operativo y trabajar de manera más eficiente. Si necesitas más detalles sobre algún comando, consulta la documentación o utiliza el comando `man <comando>` para obtener más información.
