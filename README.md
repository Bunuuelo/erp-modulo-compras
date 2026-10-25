# erp-modulo-compras (Tribu Egresos)

Este repositorio contiene el Módulo de Compras, el subsistema encargado de gestionar el ciclo de aprovisionamiento de bienes y contratación de servicios de la organización. Asegura el control comercial y el cumplimiento de las normativas tributarias peruanas (Generación del Registro de Compras 8.1 - PLE SUNAT).

## Integrantes del Equipo y Roles

| Nombre | Rol |
| :--- | :--- |
| **Rodrigo Estefanero Palma** | Product Owner |
| **Emanuel Hilacondo Begazo** | Scrum Master |
| **Christian Yanna Huanca** | Arquitecto de Software |
| **Zarun Castillo Lazo** | Desarrollador Backend |
| **Mauro Sullca Mamani** | Desarrollador Frontend |
| **Sergio Estrada Arce** | QA |
| **Alberth Riveros Vilca** | Analista Odoo |
| **Renzo Mamani Quispe** | Business Intelligence |

## Tecnologías Utilizadas

*   **Frontend:** React, TypeScript, Vite, Tailwind CSS
*   **Backend:** Python + FastAPI (REST, JSON)
*   **Base de Datos:** PostgreSQL (Relacional + JSONB)
*   **Infraestructura:** Docker y Docker Compose
*   **Pruebas (QA):** pytest, Playwright, Postman
*   **BI & Data:** Pandas, Statsmodels, Metabase/Power BI

## Estructura del Proyecto

El código está organizado siguiendo una estructura de _Clean Architecture_:

```text
/
├── backend/              # API en Python/FastAPI, validación de reglas de negocio y generador de archivos TXT (PLE).
├── frontend/             # Pantallas de proveedores, solicitudes, órdenes y comprobantes.
├── database/             # Scripts SQL y migraciones (Esquema aislado `compras`).
├── docs/                 # Diccionarios de datos SUNAT, arquitectura y diagramas.
└── tests/                # Casos de prueba tributarios y de integración.
