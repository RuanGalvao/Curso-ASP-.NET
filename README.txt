# Curso MVC

### O que é Entity Framework?

- Entity framework - ORM permite que os desenvolvedores de .NET trabalhem com banco de dados usando objetos .NET

- Utiliza 3 Linhas Principais de Utilização:

  - <b>Database First</b> - utilizado quando o banco de dados é criado antes.

  - <b>Model First</b> - primeiro o modelo é gerado e depois o banco de dados.

  - <b>Code First</b> - primeiro é criado as classes e a responsabilidade do banco fica com o entity framework

    

- Neste Projeto utilizamos o metodo Code First para criação de uma aplicação ASP.NET
- Middlewares - São componentes que são executados em todas as solicitações
- Foram instalados 2 pacotes:
  - Entity Framework utilizandoSQL-SERVER
  - Ferramentas do Entity Framework para utilizar o Migrations(**recurso que oferece uma maneira de atualizar de forma incremental o esquema de banco de dados para manter em sincronia com o modelo de classe do seu projeto preservando dados existentes no banco de dados. pode faze downgrade com histórico de modificações.**)

- Utilizamos o metodo OnConfiguring para configurar o  Entity Framework e dentro dele informamos qual o Banco de Dados sera utilizado.

- Utilizamos o recurso Scafold  que  gera uma controller com as telas e as operaçoes crud(para isso é necessario possuir model e context).

  

A aplicação do projeto se trata de um menu onde é possivel cadastra uma categoria que sera atribuida a um tipo de produto, onde este produto tera a quantidade, tipo do produto e a categoria que ele faz parte.