# Práctica 2: Modelado de Amenazas STRIDE y Diagrama de Flujo

## Escenario 1: Sistema de Autenticación de Usuarios

### Diagrama de Flujo (Mermaid)

```mermaid
graph TD
    A[Usuario / Navegador Web] -->|1. Envía credenciales| B[Servidor Web / API]
    B -->|2. Consulta credenciales| C[(Base de Datos)]
    C -->|3. Valida datos| B
    B -->|4. Responde con Token| A
