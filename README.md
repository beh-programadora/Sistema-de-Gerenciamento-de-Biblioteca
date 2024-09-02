# Sistema de Gerenciamento de Biblioteca

## Descrição

Este projeto é um sistema de gerenciamento de uma biblioteca desenvolvido utilizando SQL. Ele permite organizar e acompanhar os livros disponíveis, os autores, e os empréstimos realizados. O banco de dados facilita a administração dos recursos da biblioteca e a interação com os usuários.

## Funcionalidades

- **Gerenciamento de Autores**: Armazena informações sobre os autores, incluindo nome e nacionalidade.
- **Gerenciamento de Livros**: Armazena informações sobre os livros, como título, autor, ano de publicação e gênero.
- **Gerenciamento de Empréstimos**: Acompanha os empréstimos de livros, incluindo a data de empréstimo, data de devolução (se aplicável) e o nome do usuário que fez o empréstimo.

## Estrutura do Banco de Dados

O banco de dados contém três tabelas principais:

- **Autores**:
  - `AutorID`: Identificador único do autor.
  - `Nome`: Nome do autor.
  - `Nacionalidade`: Nacionalidade do autor.

- **Livros**:
  - `LivroID`: Identificador único do livro.
  - `Titulo`: Título do livro.
  - `AutorID`: Referência ao autor do livro.
  - `AnoPublicacao`: Ano de publicação do livro.
  - `Genero`: Gênero do livro.

- **Emprestimos**:
  - `EmprestimoID`: Identificador único do empréstimo.
  - `LivroID`: Referência ao livro emprestado.
  - `DataEmprestimo`: Data do empréstimo.
  - `DataDevolucao`: Data de devolução do livro (se devolvido).
  - `NomeUsuario`: Nome do usuário que fez o empréstimo.

## Instruções

1. Clone o repositório.
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
2. Importe o arquivo SQL no seu servidor de banco de dados.
 mysql -u usuario -p < caminho/para/o/arquivo/biblioteca.sql
3. Execute as consultas fornecidas para testar as funcionalidades do sistema.

Consultas Incluídas
Listar todos os livros com os nomes de seus autores.
Listar os empréstimos que ainda estão em aberto.
Atualizar a data de devolução de um empréstimo específico.
Remover um livro e os registros de empréstimos associados a ele.
Contribuições
Sinta-se à vontade para contribuir com o projeto, enviando pull requests ou relatando issues.

Licença
Este projeto está licenciado sob a MIT License.
