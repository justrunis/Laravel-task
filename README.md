# Laravel with Docker, Caddy, PostgreSQL and Redis

## Setup

- Clone the repository
- Create `.env` file from the `.env.example` file
- Go to `laravel-docker` folder and also create `.env` file from the `.env.example` file
- Change values of `.env` file in `laravel-docker` to match the ones in the root `.env` file
- Run the project
```bash
docker-compose up --build -d
```
- SSH into the app container to run migrations
```bash
docker-compose exec app bash
php artisan migrate
```