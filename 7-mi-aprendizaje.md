_Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Si solucionó un problema presentado al realizar la práctica también se debe documentar._

# Mi aprendizaje

<br>

En esta práctica puedo destacar los temas y aprendizajes:

### Limitación de recursos en Docker (memoria y procesador)
Aprendí cómo gestionar eficazmente los recursos en Docker mediante la configuración de límites de memoria y procesador para los contenedores. Esto incluye el uso de los parámetros `-m` para limitar la memoria y `--cpus` para limitar la cantidad de CPU que un contenedor puede utilizar.<br> Estas prácticas son fundamentales para asegurar que los contenedores operen de manera eficiente sin afectar negativamente a otros servicios en el mismo host. Además, comprendí la importancia de monitorear y ajustar estos límites según las necesidades específicas de las aplicaciones desplegadas.

### Healthcheck
Implementé healthchecks en Docker para monitorear el estado de mis aplicaciones en tiempo real. Aprendí a definir comandos de healthcheck en el Dockerfile utilizando la instrucción `HEALTHCHECK`, lo cual permite a Docker verificar automáticamente si una aplicación dentro del contenedor está funcionando correctamente. Esto es crucial para garantizar la disponibilidad continua de los servicios y facilitar la detección temprana de problemas, lo que mejora la fiabilidad y la resiliencia de las aplicaciones en entornos de producción.

### Dockerfile
Dominé la creación y configuración de Dockerfiles para la construcción de imágenes personalizadas. Aprendí a estructurar paso a paso la construcción de una imagen Docker, desde la selección de la imagen base adecuada hasta la instalación de dependencias y la configuración del entorno de ejecución. Esto incluye la optimización de capas de construcción, la copia de archivos necesarios al contenedor, y la configuración de variables de entorno y comandos de inicio. <br> Esta habilidad es fundamental para estandarizar el proceso de despliegue y asegurar la reproducibilidad del entorno de desarrollo y producción.

### Políticas de reinicio (no always, unless-stopped y on-failure)
Exploré diferentes políticas de reinicio de contenedores en Docker más allá de `no`, `always`, `unless-stopped` y `on-failure`. Aprendí cómo configurar estas políticas en la creación de contenedores o en la gestión posterior utilizando el parámetro `--restart`. Entendí las implicaciones de cada política en la disponibilidad y el manejo de fallos de los servicios en producción, permitiéndome diseñar estrategias de recuperación robustas y mejorar la estabilidad operativa de las aplicaciones.
<br>
Estos temas son fundamentales para mi formación como Ingeniero de Software, ya que me equipan con habilidades prácticas para diseñar, desplegar y mantener aplicaciones de manera eficiente y segura en entornos Dockerizados.

