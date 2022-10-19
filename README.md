# ArqDeSisOperativos

- ¿Qué es un interpretador?

        Es el encargado de traducir código fuente a código máquina.

- ¿Qué es un framework?

        Un framework es un esquema o marco de trabajo que ofrece una estructura 
        base para elaborar un proyecto con objetivos específicos, una especie de plantilla 
        que sirve como punto de partida para la organización y desarrollo de software.

- Enumere, leguajes interpretados que haya visto hasta ahora en la carrera

        Javascript.

- ¿Qué es un compilador?

        Es el encargado de transformar el código fuente de la aplicación en código de máquina
        que les posible de interpretar por el sistema.

- ¿Cuál sería el kernel de Windows?

        El kernel de Windows es cerrado.

- ¿Cómo obtengo información del Hardware?

        lscpu ó lshw 

- ¿Cuáles son los elementos fundamentales de un sistema operativo?

        Los elementos fundamentales son: Kernel, terminal, interfaz gráfica, librerías y 
        programas varios.

- ¿Qué es el GPL?

        Es una licencia de software libre y código abierto.

- ¿Cuál es la memoria más cara?

        L3

- ¿Qué tipos de memorias podemos tener en el micro?

        Caché l1, l2 y l3.

- ¿Qué son los archivos compartidos?

        Archivos entre varios ordenadores conectados a una misma red local.

- ¿Qué es un enlace con el comando ln?

        Es la abreviación de un enlace.

- ¿Qué estructura de directorios respeta linux y qué implica ésto?

        Linux respeta la estructura de directorios FHS, ésto implica estandarizar la jerarquía 
        de directorios.

- ¿Cuál es path por excelencia donde se encuentran los archivos de configuración globales de Linux?

        /etc/

- ¿Cuál es el path por excelencia donde se encuentran los logs?

        /$ var/log/

- Se pretende generar un archivo vacío (0 byte). 
- Tílde los comandos correctos (tener en cuenta que se ejecutan desde un usuario sin privilegios de root).

        .touch /tmp/archivo_vacio
        .cat /dev/null > /tmp/archivo_vacio
¿Qué es el software libre?

        El software libre es aquel que expone su código y no establece restricciones.
¿Cuáles son las libertades que establece la Free Software Foundation o Fundación por el Software Libre?

          Libertad de usar el software para cualquier propósito
          Libertad de examinar el código fuente y modificarlo para adecuarse a las necesidades
          Libertad de redistribuir el software
          Libertad de redistribuir el software modificado
¿Cuántas particiones primarias puedo tener? *

         1 a 4
¿Cuántas particiones Logicas puedo tener?

        Todas las que entren en la particion extendida
La particion extendida es utilizable para almacenar datos? *

         No.
¿Qué utilidad tiene particionar disco en lugar de solo crear directorios?

         Facilita el mantenimiento del disco duro, la comprobación de errores o la optimización y desfragmentación de las unidades.


---

Arq_Comandos
 
 COMANDOS INFORMACION DEL SISTEMA

        arch arquitectura del ordenador
        uname -r version del kernel
        unane -a sistema operativo, usuario, kernel
        cat /proc/cpuinfo informacion sobre la CPU
        cat /proc/meminfo verifica uso de la memoria RAM
        free -m muestra el estado y uso de la RAM
        cat /proc/net/dev adaptadores de red
        cat /proc/mounts sistema de archivos montado
COMANDOS NAVEGACION DEL SISTEMA

        cd /home/usuario lleva hasta la ruta indicada, ejemplo usuario
        cd.. retrocede un nivel de jerarquia de directorios
        cd../.. retrocede dos niveles
        cd lleva al directorio raiz
        cd ~usuario lleva al directorio principal del usuario indicado
        cd - lleva al direcotrio anterior
        pwd mostrara la ruta del directorio actual
        ls muestra los archivos y carpetas
        ls -l muestra el detalle de los archivos y carpetas
        ls -a muestra los archivos ocultos
        
    cat /proc/cpuinfo > home/1erexamen/CPU.txt
    echo -n "Marca=" > cpu.txt && cat /proc/cpuinfo | grep vendor | uniq | cut -d ":" -f2 >> cpu.txt 
    && echo -n "Modelo de CPU=" >> cpu.txt && cat /proc/cpuinfo | grep model | grep name | uniq | cut -d ":" -f2 >> cpu.txt 
    && echo -n "Frecuencia=" >> cpu.txt && cat /proc/cpuinfo | grep MHz | uniq | cut -d ":" -f2 >> cpu.txt 
    && echo -n "Procesadores=" >> cpu.txt  &&  cat /proc/cpuinfo | grep cores | uniq | cut -d ":" -f2 >> cpu.txt
        CREACION DE PARTICIONES

    sudo fdisk -l Lista todos los discos
    sudo fdisk /dev/disco
    n
    sudo mkfs.ext4 /dev/disco
    sudo mount /dev/disco /home/mount
    lsblk
        
 -Comando VirtualBox importantes
        
        du -sh /etc > /tmp/1erExamen/peso.txt && du -sh /home >> /tmp/1erExamen/peso.txt
        mkdir -p /Ejercicio_D/{uba,utnfra}/clase{1..5}/
        mkdir -p /Ejercicio_E/{utnba/clases{1..5},utnfra/{clases{1..9},examen}}
        top Es para ver la ram,etc..
        lscpu es para ver el modelo de la cpu, la marca,etc...
        mkdir -p /2022-09-19/pandemia/{provincial,nacional}/{informes,fotos} En este sigue la continuidad 
        mkdir -p /2022-09-19/pandemia/{provincial,nacional}/informes/fotos  En este salta de linea
        mkdir -p /2022-10-19/{Desarrollo/{Fuentes,Imagenes}/Backup,Testing/{Fuentes,Imagenes,Final}/Backup}
        



