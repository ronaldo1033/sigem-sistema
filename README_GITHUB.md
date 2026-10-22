# SIGEM — Sistema Integral de Gestión de Flotas y Maquinaria

Repositorio de trabajo académico que integra backend, interfaz web, recursos, documentación y evidencias disponibles en el paquete entregado.

## Estructura

- `src/main/java`: código Java de la aplicación.
- `src/main/resources/templates`: vistas Thymeleaf.
- `src/main/resources/static`: CSS, JavaScript e imágenes estáticas.
- `src/test`: pruebas incluidas en el proyecto.
- `docs`: arquitectura, seguridad, inventario documental, evidencias y material de avance.
- `docker-compose.yml`: configuración de servicios para desarrollo local, si aplica.

## Requisitos

- JDK compatible con la versión configurada en `pom.xml`.
- Maven (o Maven Wrapper incluido).
- PostgreSQL.

## Ejecución local

1. Crear la base de datos indicada en `application.properties` o `README.md`.
2. Configurar `DB_URL`, `DB_USERNAME`, `DB_PASSWORD` y `JWT_SECRET` con valores locales.
3. Ejecutar `./mvnw spring-boot:run` en Linux/macOS o `mvnw.cmd spring-boot:run` en Windows.
4. Abrir `http://localhost:8080`.

Consulta también `README.md`, `README_SIGEM.md` y la documentación dentro de `docs/`. Los detalles exactos pueden variar según la configuración de la máquina.

## Versionado

- Versión inicial: `v1.0.0`.
- Rama principal: `main`.
- Rama de desarrollo de Ronaldo: `ronal-desarrollo`.

## Aviso

Las cuentas documentadas como demostración son para uso local/académico. No las uses en producción. Configura secretos propios mediante variables de entorno.
