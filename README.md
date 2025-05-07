# API REST de Consulta de Cidades do Brasil

## Descrição

A **API REST de Consulta de Cidades do Brasil** é uma aplicação backend desenvolvida em Java com Spring Boot, que permite consultar informações sobre cidades brasileiras, como listagem por estado e busca por nome. O projeto utiliza Spring Data JPA para persistência em MySQL, aplicando boas práticas de desenvolvimento backend, como validações e filtragem eficiente com Java Streams.

## Funcionalidades

- Listagem de todas as cidades por estado (ex.: cidades de SP).
- Busca de cidades por nome (ex.: "São Paulo").
- Validação de entradas para evitar consultas inválidas.
- Endpoints REST com respostas padronizadas via DTOs.
- Persistência de dados com relacionamentos entre cidades e estados.

## Tecnologias Utilizadas

- **Java**: Linguagem principal.
- **Spring Boot**: Framework para APIs REST.
- **Spring Data JPA/Hibernate**: Persistência com MySQL.
- **MySQL**: Banco de dados relacional.
- **Postman**: Testes de endpoints.
- **Git**: Versionamento.
- **Maven**: Gerenciamento de dependências.

## Pré-requisitos

- Java 17 ou superior
- Maven 3.8+
- MySQL 8.0+
- Postman (para testes)
- Git

## Instalação e Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/bcstaslva/api-cidades-brasil.git
   ```
2. Configure o MySQL:
   - Crie um banco de dados chamado `cidades_brasil`.
   - Atualize as credenciais em `src/main/resources/application.properties`.
3. Navegue até o diretório do projeto:
   ```bash
   cd api-cidades-brasil
   ```
4. Compile e execute com Maven:
   ```bash
   mvn spring-boot:run
   ```
5. Acesse a API em `http://localhost:8080`.
6. Use a coleção do Postman em `/docs/postman-collection.json` para testar.

## Endpoints Principais

- `GET /cidades`: Lista todas as cidades.
- `GET /cidades/estado/{uf}`: Lista cidades por estado (ex.: SP).
- `GET /cidades/nome/{nome}`: Busca cidade por nome.
- `POST /cidades`: Cria nova cidade (para testes).

## Como Contribuir

1. Faça um fork do repositório.
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`).
3. Commit suas alterações (`git commit -m 'Adiciona nova funcionalidade'`).
4. Push para a branch (`git push origin feature/nova-funcionalidade`).
5. Abra um Pull Request.

## Autor

Bruno Costa da Silva  
[GitHub](https://github.com/bcstaslva) | [E-mail](mailto:bcstaslva@gmail.com)
