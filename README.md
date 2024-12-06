# Catálogo Musical 🎵

Este é um sistema de gerenciamento de álbuns, artistas e gêneros musicais, desenvolvido com foco na praticidade e eficiência. A aplicação permite controlar dados musicais, realizar buscas inteligentes e exibir informações detalhadas de forma organizada.

---

## Funcionalidades do Projeto

### 1. Controle de Álbuns
- **Cadastro, edição e exclusão de álbuns**: Permite a manipulação completa dos dados no banco de dados.
- **Vincular álbuns a categorias musicais**: Estabelece conexões entre álbuns e seus gêneros por meio de tabelas associativas.
- **Exibição detalhada de álbuns**: Mostra informações como ano de lançamento, capa, faixas e gênero.

### 2. Gerenciamento de Artistas
- **Adicionar, atualizar e remover artistas**: Facilita a administração dos dados relacionados aos artistas.
- **Relacionar artistas a álbuns**: Cria conexões entre artistas e seus trabalhos no sistema.
- **Visualização detalhada de artistas**: Exibe informações como nome, estilo musical e álbuns associados.

### 3. Gestão de Gêneros Musicais
- **Cadastro de novos gêneros**: Possibilita a inclusão de categorias musicais na base de dados.
- **Listagem de gêneros com informações associadas**: Exibe os gêneros junto aos artistas e álbuns que pertencem a eles.

### 4. Pesquisa Inteligente
- **Busca por álbuns, artistas e gêneros**: Uma ferramenta prática que facilita a navegação e melhora a experiência do usuário.

---

## Tecnologias Utilizadas

### Back-end
- **Node.js**: Plataforma utilizada para desenvolver a lógica do servidor.
- **Express**: Framework que simplifica a criação de rotas e funcionalidades no servidor.
- **Sequelize ORM**: Biblioteca que gerencia o acesso ao banco de dados de forma orientada a objetos.
- **PostgreSQL**: Banco de dados relacional utilizado para armazenar as informações do sistema.

### Front-end
- **EJS**: Template engine usada para criar páginas HTML dinâmicas.
- **CSS customizado**: Estilização das páginas para atender às necessidades visuais do projeto.

### Banco de Dados
- **PostgreSQL**: Sistema de banco de dados que armazena informações sobre álbuns, artistas e gêneros.

---

## Configuração do Banco de Dados

### 1. Criar o banco de dados no PostgreSQL
Execute o seguinte comando no seu terminal para criar o banco de dados:

CREATE DATABASE music_catalog;


### 2. Configurar as credenciais do banco no arquivo .env
Crie um arquivo .env na raiz do projeto e insira as credenciais do banco:

DB_HOST=localhost
DB_PORT=5432
DB_USER=seu_usuario
DB_PASSWORD=sua_senha
DB_NAME=music_catalog

### 3. Executar migrações e seeds
Para criar as tabelas e populá-las com dados iniciais, execute os comandos abaixo:


npx sequelize db:migrate
npx sequelize db:seed:all
