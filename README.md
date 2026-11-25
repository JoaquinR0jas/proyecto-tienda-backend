# FreshFits - Backend

Microservicios en Spring Boot de la tienda FreshFits (DSY1104 Desarrollo FullStack II).

Integrantes: Joaquin Rojas, Andres Cereno, Julian Silva y Diego Rivera.

## Modulos

- `eureka-server` (8761): registro de servicios.
- `api-gateway` (8080): unica entrada, seguridad JWT y rutas.
- `auth-service` (8091): login, refresh y tokens.
- `ms-usuarios` (8090), `ms-catalogo` (8081), `ms-contenido` (8083), `ms-pedidos` (8087), `ms-pagos` (8086).

## Como levantar

1. Tener Java 21 o superior y MySQL en el puerto 3307 (root sin clave) o XAMPP.
2. Compilar: `mvnw.cmd -DskipTests package`
3. Arrancar Eureka y despues cada servicio con `java -jar <modulo>/target/<modulo>-1.0.0.jar`
4. Swagger: http://localhost:8080/swagger-ui.html

El frontend esta en el repositorio `proyecto-tienda-frontend`.
