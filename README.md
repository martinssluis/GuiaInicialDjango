# Guia Básico para Iniciar com Django

Este guia é voltado para iniciantes que desejam aprender sobre desenvolvimento web utilizando o Django, um dos principais frameworks em Python. Django segue o padrão Model-View-Template (MVT), que é ótimo para criar aplicações web escaláveis, seguras e de fácil manutenção. Neste documento, você encontrará as informações necessárias para começar a desenvolver projetos em Django, desde a criação de um projeto até a organização das principais funcionalidades.

## Introdução ao Django

Django é um framework de alto nível para desenvolvimento web em Python, que fornece ferramentas prontas para autenticação, gerenciamento de sessões, rotas, e mais. Seu padrão de desenvolvimento, o Model-View-Template (MVT), é dividido em três camadas principais:

- **Model**: Camada responsável pela estruturação e manipulação dos dados da aplicação. Define campos e comportamentos essenciais dos dados que serão armazenados.
- **View**: Função em Python que recebe uma requisição web e retorna uma resposta, podendo ser HTML, JSON, entre outros.
- **Template**: Arquivo de texto que gera a interface da aplicação em formatos baseados em texto, como HTML, XML ou CSV, através do uso da Django Template Language (DTL).

## Principais Vantagens do Django

- Sistema de autenticação robusto.
- Rotas fáceis de configurar.
- ORM (Object-Relational Mapping) para facilitar interações com o banco de dados.
- Sistema de migrações para controle de alterações no banco de dados.
- Princípio DRY (Don't Repeat Yourself), que incentiva a reutilização de código.

## Primeiros Passos no Django

### Instalando e Criando um Projeto Django

Para criar um novo projeto Django, abra o terminal no Visual Studio Code ou no seu editor preferido e execute os seguintes comandos:

# Iniciar um novo projeto Django
django-admin startproject nome_do_projeto

# Navegar até a pasta do projeto
cd nome_do_projeto

# Executar o servidor de desenvolvimento
python manage.py runserver

Ao criar um projeto com Django, diversos arquivos e estruturas já são gerados automaticamente:

- Sistema administrativo para gerenciamento de dados.
- Sistema de autenticação para controle de acesso de usuários.
- Banco de dados inicial configurado por padrão com o SQLite.
- Controle de sessões para gerenciar usuários autenticados.

## Estrutura do Projeto Django

Um projeto Django inclui diversos arquivos e pastas com funções específicas:

- `__init__.py`: Arquivo vazio que informa ao Python que a pasta é um módulo Python.
- `asgi.py` e `wsgi.py`: Configurações para ASGI e WSGI, necessárias quando o projeto for colocado em um servidor de produção.
- `urls.py`: Define as URLs do site, associando caminhos específicos a funções de visualização.
- `settings.py`: Contém todas as configurações do projeto, como conexão com o banco de dados e registro de novos aplicativos.

## Aplicativos no Django

Dentro de um projeto Django, é possível criar diversos aplicativos, cada um com sua própria lógica, como um aplicativo de loja, blog, entre outros. Para criar um aplicativo, execute:
# Criar um novo aplicativo
python manage.py startapp nome_do_aplicativo
Após isso, registre o novo aplicativo em settings.py para que o Django possa reconhecê-lo.

## Principais Pastas de um Aplicativo Django
Cada aplicativo Django inclui pastas e arquivos padrão para facilitar o desenvolvimento:

- migrations/: Controla as modificações no banco de dados.

- admin.py: Configura o que será exibido na interface administrativa.

- apps.py: Configurações do aplicativo.

- models.py: Define a estrutura de dados que será armazenada no banco.

- views.py: Contém a lógica do site, controlando o que será retornado para o usuário.

- templates/: Diretório onde são armazenados os arquivos de frontend, como HTML.

## Conclusão

Django é uma excelente ferramenta para quem deseja iniciar no desenvolvimento web com Python. Este guia cobre os conceitos básicos e fornece uma introdução à estrutura e aos comandos fundamentais para criar e gerenciar projetos Django. Com a prática, você poderá construir aplicações web robustas e escaláveis.

