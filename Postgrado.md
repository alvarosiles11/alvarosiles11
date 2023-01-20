### Diseño Dirigido por el Dominio y Arquitectura Limpia

- Diseño Dirigido por el Dominio.
  <!-- - Diseño Estratégico. -->
  <!-- - Diseño Táctico. -->
- Arquitectura Limpia y CQRS.

### TESTING

<!-- - Estrategias de testing según arquitectura. -->
<!-- - Tipos de tests y como utilizarlo. -->

- capa de Unit tests
  - reporte de code coverage
- capa integration tests
  - Postman/Cucumber
    <!-- * Métricas para determinar el código probado. -->
    <!-- * Automatización y pruebas sobre UI. -->

### INTEGRACIÓN CONTÍNUA

- Aplicación de la integración continua.
  - compile y ejecute los tests
- Aplicación de la entrega continua.
  - suba a producción cuando se ejecute el ciclo para todos los microservicios
  - keys github, deploy
- Testeo continuo y monitoreo
  - pre-commit con testing y formateo de código
  - Agregar sonarlint y un linter (.editorconfig)
  - Hooks para pre-commit que realicen el formateo del código
  - Hooks para pre-commit que ejecuten los unit tests

### Contenerización de Aplicaciones

<!-- - Fundamentos y Contenedores
  - diferenciar entre una máquina virtual y un contenedor -->

- Imágenes y Docker File

  - crecación de un archivo Dockerfile para levantar su entorno de proyecto
  - Creacion de imagen a partir de dicho archivo
    - imagen postgresql (data base)
    - imagen ubuntu (app servidor)
    - imagen nginx (app frontend)

- Docker Compose / Swarm
  - crecación de archivos docker-compose.yml para levantar su entorno de proyecto.
- Publicar la imagen en el registry oficial.
  <!-- - Kubernetes -->

### INTEGRACIÓN CONTÍNUA

##### Continuous Integration y Continuous Delivery

<!-- * Definición de un ciclo de CI/CD. -->

- Aplicación de la integración continua.

  - Husky y lint-staged en sus proyectos
  - linting / code formatting instalada anteriormente antes del commit
  - Luego de hacer push al repositorio el ciclo de continuous integration sobre github actions

  - Compilación del código fuente
  - Ejecución de los unit tests
  - Análisis de código mediante sonarcloud
  - Reporte de code coverage para el código en sonarcloud.

- Aplicación de la Continuous delivery.

  - Continuous delivery que suba a producción cuando se ejecute el
    ciclo para todos los microservicios

    - google cloud
    - digitalocean
    - upcloud
    - Heroku
    - Railway
    - Amazon WS
    - AWS

### COMUNICACION ENTRE MICROSERVICIOS

comunicación que permita comunicar microservicios de manera interna y externa.

- Comunicacion externa
  API Gateway,agregación de servicios ´C# OCELOT´.
- Comunicación Interna entre Microservicios.
  El deployment y uso de docker
  - google cloud
  - digitalocean
  - upcloud
  - Heroku
  - Railway
  - Amazon WS
  - AWS

<!-- * Pratron Productor/Consumidor. -->
<!-- * Arquitectura Dirigida por Eventos. -->
<!-- * Sagas -->
