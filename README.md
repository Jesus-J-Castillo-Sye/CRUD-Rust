# CRUD-Rust
La creación de un codigo RUST, usando las tegnologias de Cargo, Dockers, postgresql y RUST
/* =======================================
FUNCION DEL SITIO
======================================== */

Create
Read all
Read one
Update
Delete

/* =======================================
REQUISITOS DE IMPLEMENTACION Y EJECUCION
======================================== */

Requisitos previos
Compilador Rust 
Cargo
Docker instalado

/* =======================================
EJECUCION DEL SITIO
======================================== */

1) Ejecute el contenedor de Postgres
Primero, ejecute el contenedor de Postgres:

docker-compose up -d db

//Nota personal debe tener el demonio "Docker"corriendo // abierto par oir la petición anterior

2) Esto construirá la imagen usando el Dockerfile que creamos antes.

docker compose build

3) Ejecute el contenedor Rust

docker compose up rustapp

4) 
docker exec -it db psql -U postgres
\dt
select * from users;

// Se puede ejecutar todas los comandos crud desde consala & consultarlos en navegador en "http://localhost:8080/users"


