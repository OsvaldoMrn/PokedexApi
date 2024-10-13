# Pokedex API

Esta es una API REST para gestionar una pokedex, con operaciones CRUD para los pokemones. 
Incluye una depuración exhaustiva de los códigos HTTP, así como paginación para los resultados que lo requieren
y manejo de caché con redis


## Requisitos

- Docker
- Docker Compose
- Node.js

## Para la instalación de los requisitos
Instalar node.js desde su página oficial: https://nodejs.org/en

Instalar  docker y docker-compose desde su página oficial: https://www.docker.com/get-started


## Para la instalación de la API

1. Clona este repositorio en el directorio de tu preferencia:
    git clone https://github.com/OsvaldoMrn/PokedexApi
2. Instala las dependencias de node.js:
    npm install
3. Construye y levanta los contenedores usando docker-compose:
    docker-compose build
    docker-compose up -d

# Uso 
Una vez que los contenedores estén en marcha (app-1, db-1 y redis-1) la API estará disponible en:

http://localhost:3000

Para verificar los endpoint y la documentación de Swagger, ingresa a:

http://localhost:3000/swaggerIndex

# Para detener los contenedores:
docker-compose down

# Para detener los contenedores, borrar el volumen utilizado y borrar la imagen construida localmente:
docker-compose down --rmi local -v



