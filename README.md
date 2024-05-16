# Rede Social Simples - API REST

Este projeto é uma aplicação backend desenvolvida durante o curso Java Orientado a Objetos.

Trata-se de uma API REST simples que simula uma rede social básica. Os usuários podem criar postagens e comentar em postagens existentes. Cada post pode receber vários comentários.

A aplicação utiliza o banco de dados MongoDB para armazenar os dados dos usuários, postagens e comentários. A escolha do MongoDB permite uma integração fácil e flexível com a aplicação, proporcionando um armazenamento eficiente e escalável para os dados da rede social simulada.

Desenvolvida com o objetivo de demonstrar conceitos fundamentais de Java, Programação Orientada a Objetos e desenvolvimento de API REST, esta aplicação oferece uma introdução prática ao desenvolvimento de aplicativos backend com tecnologias modernas.

## Funcionalidades

- Cadastro de usuários
- Criação de postagens
- Comentários em postagens
- Listagem de postagens e comentários
- Atualização e exclusão de postagens e comentários
- Autenticação de usuários

## Tecnologias Utilizadas

### Back end

- Java
- Spring Boot
- Spring Data MongoDB
- Maven

## Endpoints

### Usuários

- **GET /users:** Retorna a lista de todos os usuários cadastrados.
- **GET /users/{id}:** Retorna um usuário específico com base no ID fornecido.
- **POST /users:** Cria um novo usuário.
- **DELETE /users/{id}:** Exclui um usuário existente com base no ID fornecido.
- **PUT /users/{id}:** Atualiza os dados de um usuário existente com base no ID fornecido.
- **GET /users/{id}/posts:** Retorna todas as postagens feitas por um usuário específico com base no ID fornecido.

### Postagens

- **GET /posts/{id}:** Retorna uma postagem específica com base no ID fornecido.
- **GET /posts/titlesearch?text={text}:** Retorna todas as postagens que contenham o texto fornecido no título.

## Documentação com Swagger

Você pode acessar a documentação dos endpoints da API utilizando o Swagger. Basta acessar o seguinte link em um navegador web:

[Swagger UI](http://localhost:8080/swagger-ui/index.html#/)

## Execução

Para executar o projeto localmente, siga estas etapas:

1. Certifique-se de ter o MongoDB instalado e em execução na sua máquina.
2. Clone este repositório: `https://github.com/WerleyL/PostView-API.git`
3. Navegue até o diretório do projeto: `cd PostView-API`
4. Execute o comando Maven para compilar e iniciar a aplicação: `mvn spring-boot:run`

A API estará disponível em `http://localhost:8080`.
