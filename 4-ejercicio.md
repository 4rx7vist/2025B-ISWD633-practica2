## Esquema para el ejercicio
![Imagen](esquema-4-ejercicio.PNG)

### Crear la red
<img width="752" height="181" alt="image" src="https://github.com/user-attachments/assets/0c9aff15-ae6e-4f77-b75e-b55d1e586725" />

# COMPLETAR
### Crear el contenedor mysql a partir de la imagen mysql:8, configurar las variables de entorno necesarias
<img width="1174" height="170" alt="image" src="https://github.com/user-attachments/assets/aad8c1c6-56ce-4c9d-97d5-6186c3abff4a" />


# COMPLETAR
### Crear el contenedor wordpress a partir de la imagen: wordpress, configurar las variables de entorno necesarias
<img width="1691" height="144" alt="image" src="https://github.com/user-attachments/assets/ad248845-7e07-4e13-b3eb-8f400a374f18" />


# COMPLETAR

De acuerdo con el trabajo realizado, en el esquema del ejercicio el puerto a es **(completar con el valor)**

Ingresar desde el navegador al wordpress y finalizar la configuración de instalación.
<img width="1305" height="762" alt="image" src="https://github.com/user-attachments/assets/47acccb2-b828-4e0f-aa80-529e0e706944" />


# COLOCAR UNA CAPTURA DE LA CONFIGURACIÓN

Desde el panel de admin: cambiar el tema y crear una nueva publicación.
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress
# COLOCAR UNA CAPTURA DEL SITO EN DONDE SEA VISIBLE LA PUBLICACIÓN.

<img width="1834" height="962" alt="image" src="https://github.com/user-attachments/assets/b03c9561-e71b-41b6-be55-a4f03a3320ae" />


<img width="1813" height="843" alt="image" src="https://github.com/user-attachments/assets/8ffccd43-151f-4dca-afc1-145e0fe8468f" />

Aqui se visualiza una pagina creada en wordpress

### Eliminar el contenedor wordpress
# COMPLETAR

### Crear nuevamente el contenedor wordpress
Ingresar a: http://localhost:9300/ 
recordar que a es el puerto que usó para el mapeo con wordpress

### ¿Qué ha sucedido, qué puede observar?
El contenedr puede visualizar la pagina, de worpdress, sin embargo aunque haya existido el contenido de wordpress aun siguen las configuraciones debido a la base de datos con la información anterior (tema, configuraciones, etc.) aunque haya eliminado el contenedor de WordPress.

# COMPLETAR

