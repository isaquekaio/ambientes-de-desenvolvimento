# AMBIENTE DE DESENVOLVIMENTO LARAVEL

## Ambiente de desenvolvimento

* PHP 7.2
* PostgreSQL 10
* composer 1.10.1 
* Laravel 6

## Passos para configurar o ambiente de desenvolvimento

#### Instalação do PHP

* Abra o terminal e cole o seguinte comando: 

`sudo apt-get update && apt install php7.2-cli php7.2 php7.2-pgsql php7.2-sqlite3 php7.2-gd php7.2-curl php-memcached php7.2-imap php7.2-mysql php7.2-mbstring php7.2-zip php7.2-bcmath php7.2-soap php7.2-intl php7.2-readline php7.2-xml git libmcrypt4 libpcre3`

* Digite a sua senha

* Após concluir a instalação, digite no terminal: `php -v`

#### Instalação do PostgreSQL

* Para instalar o postgres, abra o terminal e cole o seguinte comando: 

`sudo apt-get update && apt-get install postgresql`

* Após instalação digite o seguinte comando para alterar a senha do servidor postgres:

`sudo -u postgres psql -c "ALTER USER postgres PASSWORD 'SUA_SENHA';"`

* Para criar o banco de dados, copie e cole no terminal o comando a baixo:

`sudo -u postgres psql -c "CREATE DATABASE nome-db;"`

* Para iniciar o servidor postgres, digite no terminal:

`sudo service postgresql start`

#### Instalação do Composer

* Para instalar o composer, copie e cole os seguintes comandos no terminal:

`curl -sS https://getcomposer.org/installer | php`

`sudo mv composer.phar /usr/local/bin/composer`

* Para verificar a versão do composer, digite no terminal:

`composer --version`

#### Para clonar e executar

* Abra o terminal, escolha uma pasta de sua preferência e clone o projeto: 

`git clone https://git...`

* Ao terminar de clonar o repositorio, entre na pasta do projeto 

* Dentro da pasta projeto, digite o seguinte comando: 

`composer install`

* Ao terminar de instalar as dependências do laravel no projeto, crie o arquivo .env e cole o conteúdo do arquivo .env.exemplo.

* Em seguinda digite o comando: 

`php artisan key:generate`

* Configure o acesso local ao servidor postgres através do arquivo .env, na seção de conexão ao banco. exemplo a seguir:

`DB_CONNECTION=pgsql`

`DB_HOST=127.0.0.1`

`DB_PORT=5432`

`DB_DATABASE=nome-db`

`DB_USERNAME=usuario-postgres`

`DB_PASSWORD=senha-postgres`

* Por fim, digite o comando: `php artisan serve` para starta o servidor interno do laravel.  
