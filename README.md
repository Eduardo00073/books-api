<h1 align="center">📚 Books API</h1>

<p align="center">
API REST em Spring Boot para gerenciamento de livros e categorias, com autenticação via JWT.
</p>

---

## 📖 Sobre o projeto

Backend desenvolvido em **Java + Spring Boot** para um sistema de catálogo de livros. Expõe endpoints REST para autenticação, cadastro e consulta de livros e categorias, seguindo uma arquitetura em camadas (controller, service, repository, model, DTO). Este projeto serve de API para o front-end [`booksFront_End`](https://github.com/Eduardo00073/books-frontend).

## ✨ Funcionalidades

- 🔐 Autenticação e geração de token JWT (`AuthController`)
- 📘 CRUD de livros (`BooksController`)
- 🏷️ CRUD de categorias (`CategoriesController`)
- 📄 Documentação automática da API via Swagger/OpenAPI
- 🔗 Respostas no padrão HATEOAS

## 🗂️ Arquitetura

```
br.com.eduardogabriel.books
├── config/       # Configurações (segurança, JWT, beans)
├── controller/   # Endpoints REST (Auth, Books, Categories)
├── dto/          # Objetos de transferência de dados
├── exceptions/   # Tratamento de exceções da API
├── mapper/       # Conversão entre entidades e DTOs (ModelMapper)
├── model/        # Entidades JPA
├── repository/   # Interfaces Spring Data JPA
└── service/      # Regras de negócio
```

## 🛠️ Tecnologias

<p align="center">
<img src="https://img.shields.io/badge/Java%2017-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white"/>
<img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white"/>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
<img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white"/>
<img src="https://img.shields.io/badge/Swagger-85EA2D?style=for-the-badge&logo=swagger&logoColor=black"/>
<img src="https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white"/>
</p>

## ▶️ Como rodar o projeto

```bash
# Rodar com Maven Wrapper
./mvnw spring-boot:run
```

Pré-requisitos:
- Java 17+
- PostgreSQL configurado (ajustar credenciais em `application.properties`)

A documentação interativa da API fica disponível em `/swagger-ui.html` após iniciar a aplicação.

---

<p align="center"><i>Projeto desenvolvido como parte dos meus estudos em Desenvolvimento Full Stack.</i></p>
