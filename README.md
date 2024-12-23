# Pokemon API

## Descripción

API RESTful para una Pokédex utilizando Express.js, con autenticación JWT y MongoDB.

## Endpoints

### Autenticación

- `POST /auth/register`: Registro de un nuevo entrenador.
- `POST /auth/login`: Inicio de sesión y generación de JWT.

### Gestión de Pokémon

- `GET /pokemon`: Listar todos los Pokémon (público).
- `GET /pokemon/:id`: Ver detalles de un Pokémon específico (público).
- `GET /pokemon/trainer/mypokemons`: Listar los Pokémon del entrenador autenticado.
- `POST /pokemon`: Crear un nuevo Pokémon (autenticado).
- `PUT /pokemon/:id`: Actualizar un Pokémon (autenticado).
- `DELETE /pokemon/:id`: Eliminar un Pokémon (autenticado).

## Configuración del Proyecto

### Instalación

```bash
npm init -y
npm install express mongoose jsonwebtoken bcrypt dotenv express-validator
