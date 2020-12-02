# Curso MVC





## Projeto ASP .NET

### O que é Entity Framework?

- Entity framework - ORM permite que os desenvolvedores de .NET trabalhem com banco de dados usando objetos .NET

- Utiliza 3 Linhas Principais de Utilização:

  - <b>Database First</b> - utilizado quando o banco de dados é criado antes.

  - <b>Model First</b> - primeiro o modelo é gerado e depois o banco de dados.

  - <b>Code First</b> - primeiro é criado as classes e a responsabilidade do banco fica com o entity framework

    

- Neste Projeto utilizamos o método Code First para criação de uma aplicação ASP.NET
- Middlewares - São componentes que são executados em todas as solicitações
- Foram instalados 2 pacotes:
  - Entity Framework utilizandoSQL-SERVER
  - Ferramentas do Entity Framework para utilizar o Migrations(**recurso que oferece uma maneira de atualizar de forma incremental o esquema de banco de dados para manter em sincronia com o modelo de classe do seu projeto preservando dados existentes no banco de dados. pode faze downgrade com histórico de modificações.**)

- Utilizamos o método OnConfiguring para configurar o  Entity Framework e dentro dele informamos qual o Banco de Dados será utilizado.

- Utilizamos o recurso Scafold  que  gera uma controller com as telas e as operações crud(para isso é necessário possuir model e context).

  

- A aplicação do projeto se trata de um menu onde é possível cadastra uma categoria que será atribuída a um tipo de produto, onde este produto terá a quantidade, tipo do produto e a categoria que ele faz parte.



### Projeto para Estudo Utilizando API

- API - interface de programação de aplicações

- Rest - conjunto de princípios que quando aplicados de maneira correta em uma aplicação, a beneficia com a arquitetura e padrões da própria web.

- swagger - projeto composto por algumas ferramentas para auxiliar o desenvolvedor de API em algumas tarefas como por exemplo a documentação da API.

- Para o uso do swagger para .NET CORE é necessário utilizar uma extensão chamada: **Swashbuckle.AspNetCore**

- É necessário realizar 2 alterações

  - Para ativar a documentação com XML: clicar com botão direito em cima do nome do projeto> Propriedades > Compilar > marcar a CheckBox: Arquivo de documentação XML.

  - Para iniciar o swagger no navegador: Repetir o processo do XML > Deputar > marcar a CheckBox: Iniciar Navegador e alterar para swagger.

    

- Na Startup.CS Habilitamos o Swagger injetando as dependências e habilitamos o middleware.
- Neste projeto foi reaproveitado o projeto MVC usando referência. 
- através do swagger também é possível testar a API.

