# Práctica 2: Modelado de Amenazas STRIDE y Diagrama de Flujo

## Escenario 1: Sistema de Autenticación de Usuarios

### Diagrama de Flujo (Mermaid)

```mermaid
graph TD
    A[Usuario / Navegador Web] -->|1. Envía credenciales de acceso| B[Servidor Web / API de Autenticación]
    B -->|2. Consulta credenciales| C[(Base de Datos de Usuarios)]
    C -->|3. Retorna resultado de validación| B
    B -->|4. Genera y responde con Token de Sesión| A
    ```
