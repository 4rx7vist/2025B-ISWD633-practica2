### Crear contenedor de Postgres sin que exponga los puertos. Usar la imagen: postgres:15-alpine3.21
# COMPLETAR

### Crear un cliente de postgres. Usar la imagen: dpage/pgadmin4

# COMPLETAR

La figura presenta el esquema creado en donde los puertos son:
- a: (80)
- b: (8080)
- c: (5432)

![Imagen](esquema-2-ejercicio.PNG)

## Desde el cliente
### Acceder desde el cliente al servidor postgres creado.
# COMPLETAR CON UNA CAPTURA DEL LOGIN
<img width="1770" height="785" alt="image" src="https://github.com/user-attachments/assets/02147832-3986-4b52-beff-888e9cabd768" />

<img width="1919" height="926" alt="image" src="https://github.com/user-attachments/assets/cb4d0384-b17e-4add-8e3b-da6eb24c2412" />

### Crear la base de datos info, y dentro de esa base la tabla personas, con id (serial) y nombre (varchar), agregar un par de registros en la tabla, obligatorio incluir su nombre.

Dentro del cliente de postgres ya ingeresado a la base de datos de postgres:
<img width="1845" height="796" alt="image" src="https://github.com/user-attachments/assets/d2251440-1d23-43dd-8f5d-96225c33f33e" />

Con la insersion de la base de datos con el esquema y un par del registro se visualiza de esta manera:
<img width="1847" height="850" alt="image" src="https://github.com/user-attachments/assets/0ba17556-9921-49b2-bb9f-432b3135a292" />

## Desde el servidor postgresl
### Acceder al servidor
### Conectarse a la base de datos info

# COMPLETAR

Desde el contenedor de pg_postgres para la instancia de postgres, se visualiza de la siguiente manera al realizar la consulta desde el contenedor de postgres:

### Realizar un select *from personas
<img width="725" height="335" alt="image" src="https://github.com/user-attachments/assets/50d891f3-2969-4319-b194-ac067177affa" />


# AGREGAR UNA CAPTURA DE PANTALLA DEL RESULTADO

