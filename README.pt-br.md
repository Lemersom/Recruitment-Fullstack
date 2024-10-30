# Sistema de Gerenciamento de Currículos

Este projeto é uma aplicação full-stack projetada para gerenciar currículos de forma eficiente, permitindo aos usuários adicionar dados pessoais, experiências profissionais, formações acadêmicas e informações de contato.

## Tecnologias

* Back-End: Django com Django REST Framework (DRF) para criação da API
* Front-End: React.js com Vite para uma interface rápida e responsiva

## Funcionalidades do Projeto

* Backend em Django fornecendo uma API RESTful utilizando DRF para gerenciar dados de currículos
* Frontend em React.js permitindo que os usuários adicionem e atualizem informações pessoais, profissionais e acadêmicas
* Validação básica dos dados de entrada, como formatos de email, números de telefone e formatos de data
* Painel administrativo do Django para gerenciar os currículos cadastrados

## Executando Localmente
**Pré-requisitos:** Certifique-se de ter o Python e o Node.js instalados na sua máquina.

### Configuração do Backend

Clone o projeto
```
git clone --recurse-submodules https://github.com/Lemersom/Recruitment-Fullstack.git
```

Navegue até o diretório do backend
```
cd backend
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
cd frontend  # Caso você esteja no diretório backend, use `cd ../frontend`
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

* API do Backend: Rodando em http://localhost:8000
* Frontend: Rodando em http://localhost:5173
