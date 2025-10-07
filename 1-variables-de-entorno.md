# Variables de Entorno
### ¿Qué son las variables de entorno?
Es un valor dinámico con un nombre que reside en el sistema operativo y que influencia el comportamiento de los programas, este proporcionando información sobre el sistema o la sesión en curso.
Normalmente, las variables de entorno almacenan valores predeterminado y permanecen de manera oculta configuradas en el sistema.

# COMPLETAR

### Para crear un contenedor con variables de entorno

```
docker run -d --name <nombre contenedor> -e <nombre variable1>=<valor1> -e <nombre variable2>=<valor2>
```

### Crear un contenedor a partir de la imagen de nginx:alpine con las siguientes variables de entorno: username y role. Para la variable de entorno rol asignar el valor admin.

Para mi caso, ejecuto este comando: 
```
$  docker run -d --name jenkins -e username=alexis -e role=admin -p 50000:50000 -p 8080:8080 jenkins/jenkins
```

# COMPLETAR

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR

<img width="1275" height="355" alt="image" src="https://github.com/user-attachments/assets/b0541506-a521-4940-ac82-2d2c72c6e941" />

### Crear un contenedor con la imagen de mysql, mapear todos los puertos


# COMPLETAR

### ¿El contenedor se está ejecutando?
# COMPLETAR

### Identificar el problema
# COMPLETAR

### Para crear un contenedor con variables de entorno especificadas
- Portabilidad: Las aplicaciones se vuelven más portátiles y pueden ser desplegadas en diferentes entornos (desarrollo, pruebas, producción) simplemente cambiando el archivo de variables de entorno.
- Centralización: Todas las configuraciones importantes se centralizan en un solo lugar, lo que facilita la gestión y auditoría de las configuraciones.
- Consistencia: Asegura que todos los miembros del equipo de desarrollo o los entornos de despliegue utilicen las mismas configuraciones.
- Evitar Exposición en el Código: Mantener variables sensibles como contraseñas, claves API, y tokens fuera del código fuente reduce el riesgo de exposición accidental a través del control de versiones.
- Control de Acceso: Los archivos de variables de entorno pueden ser gestionados con permisos específicos, limitando quién puede ver o modificar la configuración sensible.

### Crear un contenedor con mysql, mapear todos los puertos y configurar las variables de entorno mediante un archivo

# COMPLETAR

# CAPTURA CON LA COMPROBACIÓN DE LA CREACIÓN DE LAS VARIABLES DE ENTORNO DEL CONTENEDOR ANTERIOR 

### ¿Qué bases de datos existen en el contenedor creado?
Se verifica através del comando:

```
$ docker exec -it mysql bash
```
A posterior se ingresa con el comando de 

```
# mysql -u root -p 
```
para ingreesar al gestor de base de datos.

<img width="356" height="228" alt="image" src="https://github.com/user-attachments/assets/c435dd81-b33a-406d-bf58-201ace69d999" />

Se muestran 4 bases de datos.

# COMPLETAR
