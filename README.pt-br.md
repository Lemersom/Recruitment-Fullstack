# Sistema de Gerenciamento de Currículos

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Lemersom/Recruitment-Fullstack/blob/main/README.md)
[![pt-br](https://img.shields.io/badge/lang-pt--br-green.svg)](https://github.com/Lemersom/Recruitment-Fullstack/blob/main/README.pt-br.md)

Este projeto é uma aplicação full-stack projetada para gerenciar currículos de forma eficiente, permitindo aos usuários adicionar dados pessoais, experiências profissionais, formações acadêmicas e informações de contato.

## Tecnologias

* Back-End: Django com Django REST Framework (DRF) para criação da API
* Front-End: React.js com Vite para uma interface rápida e responsiva
* Containerização: Docker para containerizar a aplicação

## Funcionalidades do Projeto

* Backend em Django fornecendo uma API RESTful utilizando DRF para gerenciar dados de currículos
* Frontend em React.js permitindo que os usuários adicionem e atualizem informações pessoais, profissionais e acadêmicas
* Validação básica dos dados de entrada, como formatos de email, números de telefone e formatos de data
* Painel administrativo do Django para gerenciar os currículos cadastrados

## Executando Localmente Com Docker
**Pré-requisitos:** Certifique-se de ter o Docker e Docker Compose instalados na sua máquina.

Clone o projeto
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

Navegue até o diretório clonado
```
cd Recruitment-Fullstack
```

Contrua os containers
```
docker-compose build
```

Suba os containers
```
docker-compose up
```

Execute as migrações do banco de dados
```
docker-compose exec backend python manage.py migrate
```

Crie um SuperUsuário
```
docker-compose exec backend python manage.py createsuperuser
```

## Executando Localmente Sem Docker
**Pré-requisitos:** Certifique-se de ter o Python e o Node.js instalados na sua máquina.

Clone o projeto
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

### Configuração do Backend

Navegue até o diretório do backend
```
cd Recruitment-Fullstack\backend
```

Crie e ative um ambiente virtual
```
python -m venv venv
source venv/bin/activate  # Para Windows use `venv\Scripts\activate`
```

Instale as dependências
```
pip install -r requirements.txt
```

Execute as migrações do banco de dados
```
python manage.py migrate
```

Crie um SuperUsuário
```
python manage.py createsuperuser
```

Inicie o servidor Django
```
python manage.py runserver
```

### Configuração do Frontend

Navegue até o diretório do frontend
```
cd Recruitment-Fullstack\frontend
```

Instale as dependências
```
npm install
```

Inicie o servidor de desenvolvimento
```
npm run dev
```

## Acessando a Aplicação

* API do Backend: http://localhost:8000
* Painel Admin: http://localhost:8000/admin
* Frontend: http://localhost:5173
