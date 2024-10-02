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

## Como levantar los microservicios (posteriormente esto se hará automático con Docker)

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

## Diagramas
### Diagrama de datos
![MSC-Diagramas - Diagrama ER (1)](https://github.com/user-attachments/assets/4c21a7f8-5e70-4aeb-a93c-5c34988910b0)
### Diagrama de clases
![MSC-Diagramas - Diagrama Clases](https://github.com/user-attachments/assets/6f70bdb7-d6ad-4af9-8008-98e068c5a0f2)
### Diagrama de componentes
![MSC-Diagramas - Diagrama Componentes](https://github.com/user-attachments/assets/f23734a6-885c-4bd6-b2a6-4c9713a92b71)
### Diagrama de despliegue
![MSC-Diagramas - Diagrama Despliegue](https://github.com/user-attachments/assets/6a506c12-9497-4167-bd44-79888095c8fa)
