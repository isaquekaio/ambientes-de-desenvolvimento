# AMBIENTE DE DESENVOLVIMENTO LARAVEL

## Ambiente de desenvolvimento

* Python 3.7.7
* SQLite 
* Django 3.0.8
* Pip
* Venv

## Passos para configurar o ambiente de desenvolvimento

#### Python

* Geralmente no linux o python em intalado por padrão, digite no terminal: `python --version`

#### Instalação do Pip

* Para intalar o pip (gerenciador de pacotes do python) digite:

`sudo apt install -y python3-pip`

* Para verificar, digite no terminal:

`pip --version`

#### Instalação da Venv

* Para intalar a venv digite:

`sudo apt install -y python3-venv`

* Para criar uma venv, digite no terminal:

`python3 -m venv my_envn`

* Para ativar a venv, digite:

`source my_env/bin/activate`

#### Instalação do Django

* Com a venv ativada, digite o seguinte comando para instalar o django:

`python -m pip install Django` 

#### Para clonar e executar

* ... : 

* Por fim, digite o comando: `python manager runserver` para starta o servidor interno do django.  
