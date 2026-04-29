# Concurso
## Tecnologias utilizadas
Para el desarrollo se utilizo nestJS para manejar una Api rest, y usamos NextJS para nuestro cliente frontend, a su vez usamos
TypeORM para la conexion con la base de datos y class-validator y class-transformer para la validación y formato de las peticiones
por ultimo para la autenticación utilizamos JWT.


## Setup
Primero se debe clonar el monorepo donde esta orquestado tanto el front como el back https://github.com/sebatihm/Concurso-de-Programacion-2026.git

```bash
  git clone --recurse-submodules https://github.com/sebatihm/Concurso-de-Programacion-2026.git
```
Una vez clonado el repositorio crear un archivo .env para el manejo de variables de entorno, los cuales son:

```.env

DATABASE_ROOT_PASSWORD=
DATABASE=
DATABASE_USER=
DATABASE_PASSWORD=
DATABASE_PORT=
SECRET=
SALT_ROUNDS=
ADMIN_EMAIL=
ADMIN_PASSWORD=
ALLOWED_CORS_URLS=

```

Una vez creado este archivo y configurada la variable de entorno ya se puede ejecutar el servicio con el siguiente comando.

```bash
  docker compose up
```


Para ejecutarlo en segundo plano

```bash
  docker compose up -d
```


Para reconstruir las imagenes cuando se necesiten cambios

```bash
  docker compose up -d –build
```
