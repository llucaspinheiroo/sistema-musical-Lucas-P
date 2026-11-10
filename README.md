# 🎵 Sistema Musical

## Sobre o Projeto

O **Sistema Musical** é uma aplicação web desenvolvida em PHP, HTML, CSS e MySQL, com o objetivo de organizar e gerenciar informações sobre artistas e músicas.

O sistema permite cadastrar artistas, adicionar músicas à biblioteca, armazenar imagens, editar informações e consultar os registros cadastrados. Também possui um sistema de login para controlar o acesso às funcionalidades.

## Funcionalidades

### 🔐 Sistema de Login
- Autenticação de usuários.
- Verificação de senha utilizando `password_verify()`.
- Controle de sessões.
- Proteção das páginas para usuários não autenticados.
- Opção de encerrar a sessão (logout).

### 🎤 Cadastro de Artistas
- Cadastrar novos artistas.
- Informar nome, gênero musical e país.
- Adicionar imagem do artista.
- Editar informações cadastradas.
- Excluir artistas.
- Impedir a exclusão de artistas que possuem músicas vinculadas.

### 🎶 Cadastro de Músicas
- Cadastrar músicas vinculadas a artistas.
- Informar título, álbum e gênero musical.
- Adicionar link de vídeo do YouTube.
- Inserir letra da música.
- Adicionar imagem de capa.
- Editar e excluir músicas cadastradas.

### 📚 Biblioteca Musical
- Visualizar as músicas cadastradas.
- Consultar informações dos artistas.
- Pesquisar músicas por título, álbum ou artista.
- Filtrar por artista e gênero musical.

## Tecnologias Utilizadas

- **HTML5:** estrutura das páginas.
- **CSS3:** estilização e organização visual.
- **PHP:** processamento das informações e funcionalidades do sistema.
- **MySQL:** armazenamento e gerenciamento dos dados.
- **MySQLi:** comunicação entre PHP e banco de dados.
- **JavaScript:** recursos complementares da interface.

## Organização dos Arquivos

| Arquivo | Função |
|---|---|
| `index.php` | Menu principal do sistema. |
| `login.php` | Tela de autenticação. |
| `logout.php` | Encerramento da sessão. |
| `cadastro_artista.php` | Cadastro e gerenciamento de artistas. |
| `cadastro_musica.php` | Cadastro e gerenciamento de músicas. |
| `listagem_musicas.php` | Biblioteca e listagem de músicas. |
| `conexao.php` | Conexão com o banco de dados. |
| `valida_sessao.php` | Verificação de autenticação. |
| `bd.sql` | Script de criação do banco de dados e das tabelas. |
| `styles.css` | Estilização das páginas. |
| `img/` | Armazenamento das imagens utilizadas. |

## Como Executar o Projeto

1. Inicie o Apache e o MySQL pelo XAMPP.
2. Coloque a pasta `sistema_musical` dentro do diretório `htdocs`.
3. Abra o phpMyAdmin.
4. Importe o arquivo `bd.sql` para criar o banco de dados e suas tabelas.
5. Confira as configurações de conexão no arquivo `conexao.php`.
6. Acesse pelo navegador:

`http://localhost/sistema_musical/login.php`

## Acesso ao Sistema

**Usuário padrão:** `admin`

**Senha:** `123`

## Segurança

O projeto utiliza algumas medidas para proteger as informações, como:

- Senhas armazenadas com hash.
- Consultas preparadas com MySQLi.
- Controle de acesso por sessões.
- Validação de informações enviadas pelos formulários.
- Uso de `htmlspecialchars()` para evitar problemas na exibição de dados.

## Objetivo

O objetivo da atividade é desenvolver uma aplicação web integrada a um banco de dados, colocando em prática conhecimentos de PHP, HTML, CSS e MySQL, além de trabalhar com operações CRUD (Create, Read, Update e Delete), autenticação de usuários e organização de informações.

---

**Projeto acadêmico – Sistema Musical.**
