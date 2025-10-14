# Redes
Las redes son un componente fundamental que permite la comunicación entre contenedores, así como la comunicación de los contenedores con el mundo exterior. 
![Imagen](redes.PNG)
- Bridge: Esta es la red por defecto en Docker. Permite la comunicación entre contenedores en el mismo host. Cada contenedor conectado a la red bridge tiene una IP propia en la subred de la red bridge.
    -  Brige por default: Cuando se ejecuta un contenedor, Docker crea automáticamente una red de tipo bridge por default. Esta red se utiliza para permitir la comunicación entre contenedores en el mismo host. Cada contenedor conectado a esta red obtiene su propia dirección IP en la subred de la red bridge.
    - Bridge creada por nosotros: Un usuario también puede crear sus propias redes de tipo bridge en Docker. Esto puede ser útil para organizar y segmentar los contenedores de una aplicación de manera más controlada. Al crear una red bridge personalizada, se puede especificar un rango de direcciones IP y otras configuraciones de red específicas. Los contenedores conectados a esta red utilizarán las direcciones IP de la subred definida por el usuario.
- Host: Con esta red, los contenedores comparten la red del host en lugar de tener su propia interfaz de red. Esto puede mejorar el rendimiento de red, pero los contenedores pueden entrar en conflicto con los puertos del host si intentan utilizar los mismos puertos.
- None: Con esta red, se deshabilita la configuración de red. Los contenedores que usan esta red tienen su propia red de loopback y no pueden comunicarse con otros contenedores a menos que se conecten explícitamente a una red.

### Crear una red de tipo bridge

```
docker network create <nombre red> -d bridge
```
<img width="639" height="145" alt="image" src="https://github.com/user-attachments/assets/1b368295-5978-4429-be55-8a375d32e68f" />


### Crear un contenedor vinculado a una red

```
docker run -d --name <nombre contenedor> --network <nombre red> <nombre imagen>
```

<img width="1179" height="89" alt="image" src="https://github.com/user-attachments/assets/69dd3120-628e-44bc-bf47-7286a8279c24" />


### Para saber a qué red está conectado un contenedor

```
docker inspect <nombre contenedor>
```

<img width="1105" height="527" alt="image" src="https://github.com/user-attachments/assets/27234db0-ade3-476b-b9ca-6f99a500459a" />


ó
```
docker network inspect <nombre red> 
```

<img width="1027" height="703" alt="image" src="https://github.com/user-attachments/assets/33bf19e6-5492-426b-b1ec-4f9efdb1b77e" />
<img width="1161" height="542" alt="image" src="https://github.com/user-attachments/assets/a3f3865d-7f38-4fe6-b9a1-cabbc3630c01" />


### Vincular contenedor a una red
```
docker network connect <nombre red> <nombre contenedor>
```

<img width="1233" height="75" alt="image" src="https://github.com/user-attachments/assets/40aeb21f-73ab-406d-bb01-f4de32b063ea" />


### Para desvincular un contenedor de una red
```
docker network disconnect <nombre red> <nombre contenedor>
```
<img width="998" height="32" alt="image" src="https://github.com/user-attachments/assets/32ccd7ce-8c16-443d-b3d9-ecab65930de8" />

### Para listar las redes existentes
```
docker network ls
```
<img width="622" height="148" alt="image" src="https://github.com/user-attachments/assets/4c9ec1da-aa16-4159-a0ba-96f02878ea70" />


### Crear los contenedores y las redes que se presentan en el esquema. Usar para todos los contenedores la imagen de nginx:alpine

![Imagen](esquema-ejercicio-redes.PNG)

# COLOCAR UNA CAPTURA DE LAS REDES EXISTENTES CREADAS

# COLOCAR UNA(S) CAPTURAS(S) DE LOS CONTENEDORES CREADOS EN DONDE SE EVIDENCIE A QUÉ RED ESTÁN VINCULADOS

### Para eliminar las redes creadas
```
docker network rm <nombre de la red>
```

<img width="661" height="56" alt="image" src="https://github.com/user-attachments/assets/a92c4513-8469-4eb2-b268-aa929b10b83b" />

