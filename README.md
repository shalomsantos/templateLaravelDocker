# Laravel 10, Docker, bootstrap

## Passo a passo para rodar o projeto

Clone o projeto
```sh
git clone https://github.com/shalomsantos/templateLaravelDocker.git
```
```sh
cd templateLaravelDocker/
```


Crie o Arquivo .env *ubuntu
```sh
touch .env
```


Atualize essas variáveis de ambiente no arquivo .env
```dosini
APP_NAME="<NamePorject>"
APP_URL=http://localhost:8989

DB_CONNECTION=***
DB_HOST=***
DB_PORT=***
DB_DATABASE=***
DB_USERNAME=***
DB_PASSWORD=***


Suba os containers do projeto
```sh
docker-compose up -d
```


Acesse o container
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```


Gere a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:8989](http://localhost:8989)
