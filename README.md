# **cities-api-db** 🏙️ #

## Proyecto de Entornos de Desarrollo. ##
### Trabajar con Node.js, una base de datos SQLite, knex como librería para gestionar el acceso a la base de datos y **organizado en capas**. ###

![Arquitectura API Node.js](https://entornos-desarrollo.codeandcoke.com/_media/apuntes:nodejs_api_structure.png?cache=&w=741&h=362&tok=4bd41b "Arquitectura API Node.js")
---

## API de ciudades con las siguientes funcionalidades: ##

- **CRUD COMPLETO**
   - GET `/cities`
   - GET `/cities/:id`
   - POST `/cities`
   - PUT `/cities/:id`
   - DELETE `/cities/:id`


## **FUNCIONALIDADES** ##

- Utiliza una base de datos *SQLite* (no incluida en el repositorio) que contiene una tabla **`cities`** con las columnas: `id`, `name`, `population`, `altitude` y `capital`.
- Utiliza la libreria **`knex`** para gestionar el acceso a la base de datos.
- Control de errores.
- En nuestro caso trabajaremos con las siguientes capas:
   - **`route`**: Se definen las rutas o endpoints disponibles para cada uno de los elementos del modelo de datos.
   - **`controller`**: Se definen las funciones que reciben las peticiones de las rutas definidas en la capa `route`.
   - **`service`**: Funciones que definen la lógica de aplicación.
   - **`configuration`**: Incluy el fichero de configuración de la base de datos, indicando el tipo (SQLite) y la ubicación (el fichero `cities.db`).
