# Limitar uso de procesador
Limitar la cantidad de núcleos de CPU:
```
--cpus=<número de núcleos>
```

Asignar núcleos de CPU específicos:
```
--cpuset-cpus=<lista de núcleos>
```

**¿Como saber el numero de procesadores virtuales que tiene una máquina?**
Para conocer el número de procesadores virtuales en Linux, el comando `nproc` en la terminal te proporciona el número de procesadores o núcleos lógicos disponibles.<br>
En Mac se puede verificar el número de núcleos en la aplicación "Utilidad de sistema" bajo la sección "Hardware". Otra opción es mediante la terminal de Mac se puede ejecutar `sysctl -n hw.logicalcpu`. <br>
En Windows esta información se obtiene mediante el Administrador de tareas en la pestaña "Rendimiento" al mostrar la información bajo la sección "Núcleos". Alternativamente mediante Powershell se puede ejecutar `(Get-WmiObject -Class Win32_ComputerSystem).NumberOfLogicalProcessors`


## Ejemplos
_Puedes copiar y ejecutar directamente cada uno de los comandos_

Limitar el uso de CPU a 1.5 núcleos
```
docker run -d --name server-nginx --cpus="1.5" nginx:alpine
```

Restringir el contenedor para que use los núcleos de CPU 0 a 2:
```
docker run -d --name server-nginx --cpuset-cpus="0-2" nginx:alpine
```

Restringir el contenedor para que use los núcleos de CPU 1 y 3:
```
docker run -d --name server-nginx --cpuset-cpus="1,3" nginx:alpine
```
