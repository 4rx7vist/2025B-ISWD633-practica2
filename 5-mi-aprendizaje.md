# COMPLETAR  
Comparando sus conocimientos antes de hacer la práctica con sus conocimientos después de hacer la tarea, explicar los principales aprendizajes logrados para beneficio de su formación profesional.  
Si solucionó un problema presentado al realizar la práctica también se debe documentar.

Consultar: Cómo se gestionan datos confidenciales con los secretos de Docker (Docker Secrets).

## Reflexión 
Antes de realizar esta práctica, tenía conocimientos generales sobre la ejecución de contenedores en Docker y el uso básico de imágenes como PostgreSQL o WordPress. Sin embargo, a través del desarrollo de esta actividad logré comprender con mayor profundidad cómo se gestionan los servicios y la comunicación entre contenedores utilizando variables de entorno, puertos y enlaces (--link), así como la persistencia de datos en bases de datos externas (por ejemplo, MySQL o PostgreSQL) independientemente del contenedor de aplicación.

Uno de los principales aprendizajes fue entender que los contenedores son efímeros, y que la información crítica no debe almacenarse dentro de ellos, sino en un servicio persistente o en volúmenes externos. Al eliminar y recrear el contenedor de WordPress, observé que la información del sitio se mantenía, lo que evidenció que los datos realmente estaban en la base de datos MySQL. Este ejercicio permitió visualizar de forma práctica la separación entre la capa de aplicación y la de datos.

Respecto a Docker Secrets.

Docker gestiona datos confidenciales (como contraseñas, claves privadas o tokens) mediante una característica llamada Docker Secrets.
Esta funcionalidad permite almacenar de manera segura información sensible y distribuirla solo a los contenedores que la necesitan, evitando exponer credenciales en texto plano dentro de variables de entorno o archivos.

Ventajas:

- Los secretos están encriptados en reposo y en tránsito.
- Solo los contenedores autorizados pueden acceder a ellos.
- Evita el riesgo de exponer credenciales en los comandos docker inspect o en el historial del sistema.
