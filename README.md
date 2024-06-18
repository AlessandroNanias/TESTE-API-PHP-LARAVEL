## Importante!! Crie o Arquivo .env atualizando as variaveis de ambiente a seguir:
```
APP_NAME=app-laravel
APP_URL=http://localhost:8989

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_db
DB_USERNAME=nome_usuario
DB_PASSWORD=senha

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```
Suba os containers do projeto
```
docker-compose up -d
```
Acesso do container
```
docker-compose exec app bash
```
Instale as dependências do projeto:
```
composer install
```
Gerar a chave do projeto:
```
php artisan key:generate
```
Acesso do projeto:
[http://localhost:8989/users](http://localhost:8989/users)
