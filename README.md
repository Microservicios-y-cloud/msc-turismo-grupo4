# msc-turismo-grupo4

## Integrantes
 - Kevin Estiven Velasco Pinto
 - Nicolás Reyes
 - Juan Diego Echeverry Plazas


## Comandos para clonar el proyecto
```bash
git submodule init
```

```bash
git submodule update
```

## Instrucciones de Docker
1. Asegurarse de contenerizar la version del proyecto correcta:
```bash
mvn clean
```
```bash
mvn install
```

2. Construir el contenedor
    ```bash
    docker build -t {nombre_del_contenedor} .
    ```

3. Correr el contenedor
    ```bash
    docker run -p port:port {nombre_del_contenedor} .
    ```

Asegurate de borrar los contenedores que no utilices, o que esten desactualizados, el siguiente comando borra un solo contenedor:

```bash
docker rm -f <containerId/Name>
```

El siguiente comando borra todos los contenedores:

```bash
docker rm $(docker ps -aq)
```


## Como levantar los microservicios

### Por terminal
 - El comando para inicializar es el siguiente:

    ```bash
    mvn spring-boot:run
    ```
1. Inicializar config-server
2. Inicializar los demás servicios

### Por extensión de vsCode
1. Descargar la extensión Spring Boot: Dashboard
2. Cerrar y abrir nuevamente VSCode
3. inicializar desde la extensión primero config-server
4. Inicializar los demás servicios

## Historias de usuario
### Link: https://docs.google.com/document/d/1AuXA7oklvI9T2SzBfv9hUQvsC7KEiy8zRfKN6rRYDDo/edit?usp=sharing

## Diagramas
### Link: https://lucid.app/lucidchart/b86b097d-f3db-4712-8977-6b2767f2ba59/edit?viewport_loc=2570%2C-64%2C2500%2C1024%2C7Vy9Px8OXLNV&invitationId=inv_460007cd-89a0-4f22-987c-66b1a09df58d
### Diagrama de datos
![MSC-Diagramas - Diagrama ER (1)](https://github.com/user-attachments/assets/4c21a7f8-5e70-4aeb-a93c-5c34988910b0)
### Diagrama de clases
![MSC-Diagramas - Diagrama Clases](https://github.com/user-attachments/assets/6f70bdb7-d6ad-4af9-8008-98e068c5a0f2)
### Diagrama de componentes
![MSC-Diagramas - Diagrama Componentes](https://github.com/user-attachments/assets/f23734a6-885c-4bd6-b2a6-4c9713a92b71)
### Diagrama de despliegue
![MSC-Diagramas - Diagrama Despliegue](https://github.com/user-attachments/assets/6a506c12-9497-4167-bd44-79888095c8fa)
### Diagrama de arquitectura
![Animation](https://github.com/user-attachments/assets/e3c875e3-abcb-449b-bad1-bc02d4ec80ad)

