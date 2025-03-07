# manager-jiu-jitsu
🥋 API de Gestão de Alunos de Jiu Jitsu com Interface Multiplataforma
<p>
  <img src="https://img.shields.io/badge/made%20by-Miguel%20Marostica-04D361?style=flat-square">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/yMiguelzin/manager-jiu-jitsu?color=04D361&style=flat-square">
  <img alt="GitHub Top Language" src="https://img.shields.io/github/languages/top/yMiguelzin/manager-jiu-jitsu?color=04D361&style=flat-square">
  <a href="https://opensource.org/licenses/MIT">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-04D361?style=flat-square">
  </a>
</p>

## Tópicos

[Sobre o Projeto](#sobre-o-projeto)

[Tecnologias](#tecnologias)

[Instalação e Uso](#instalação-e-uso)

[Licença](#licença)

<br>

## Sobre o Projeto

Este projeto foi desenvolvido para gerenciar uma acadêmia de jiu-jitsu utilizando Python e Django com Flet sendo multiplataforma. O objetivo é permitir que os professores registrem os alunos de forma organizada, podendo criar, editar, listar e excluir, aulas pra subir de faixa e o progresso do aluno. O projeto utiliza Django-Ninja uma biblioteca api para o back-end como framework principal para o desenvolvimento da aplicação web usado django e foi pensado para fornecer uma interface simples e intuitiva para os usuários com flet multiplataforma e uma biblioteca de requests para ligar o front-end com o back-end.

<p align="center">
  <img src="image1.png" alt="Imagem 1">
  <img src="image2.png" alt="Imagem 2">
</p>

<br>

## Tecnologias

As seguintes tecnologias foram utilizadas no desenvolvimento do projeto:

- [Python](https://www.python.org/)
- [Django](https://www.djangoproject.com/)
- [Django-Ninja](https://django-ninja.dev/) ( api )
- [Pillow](https://python-pillow.org/) (para manipulação de imagens)
- [https://flet.dev/](https://www.sqlite.org/index.html) (biblioteca multiplataforma)

<br>

## Instalação e Uso

### Pré-requisitos

Antes de começar, você precisa ter o Python 3.x instalado no seu sistema. Você pode baixar o Python [aqui](https://www.python.org/downloads/).

### Passos para Configuração e Execução

1. **Clone o repositório**:

  Abra seu terminal e clone o repositório do projeto:

  ```bash
  git clone https://github.com/yMiguelzin/manager-jiu-jitsu.git

  ```
2. **Ative o ambiente virtual (opcional, mas recomendado)**:

  Navegue até a pasta do projeto e crie/ative um ambiente virtual:

  ```bash
  # Criar
    
  #Linux
  python3 -m venv venv
    
  #Windows
  python -m venv venv
  ```

<br>

Após a criação do venv vamos ativa-lo:

  ```bash
  #Ativar

  #Linux
  source venv/bin/activate
  
  #Windows
  venv\Scripts\Activate

  # Caso algum comando retorne um erro de permissão execute o código e tente novamente:
  Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned

  ```

3. **Instale as dependências**:

  Navegue até a pasta do projeto e instale as dependências necessárias:

  ```bash
  #Dependências Front-end / Back-end

  Front-end:

  pip install flet
  pip install requests

  Back-end:

  pip install django
  pip install pillow
  pip install django-ninja


  ```

4. **Configuração do Banco de Dados back-end**:

  Agora, configure o banco de dados. Execute os comandos abaixo para criar as migrações necessárias e aplicá-las ao banco de dados:
  
  ```bash
  python manage.py makemigrations
  python manage.py migrate

  ```
5. **Execute o Back-end**:

  Inicie o servidor de desenvolvimento para rodar a aplicação localmente:
  
  ```bash
  python manage.py runserver
  O servidor será executado em http://localhost:8000/api/docs
  Abra esse endereço no seu navegador para começar a usar a aplicação.
  
  ```

5. **Execute o Front-end**:

  Inicie o front-end de desenvolvimento para rodar a aplicação localmente:
  
  ```bash
  flet run app.py
  
  ```

  <br>
  
## Licença
<a href="https://opensource.org/licenses/MIT">
    <img alt="License" src="https://img.shields.io/badge/license-MIT-04D361?style=flat-square">
</a>

<br>

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](/LICENSE) para mais detalhes.

---

Feito com 💚 por [Miguel Marostica](https://github.com/yMiguelzin)

