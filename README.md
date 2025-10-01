# Projeto Integrador - LinkedIn Clone (Backend + Bancos Não Relacionais)

Este projeto foi desenvolvido como atividade prática da disciplina de **Engenharia de Software**, com o objetivo de **integrar Backend e Banco de Dados Não Relacionais** em um sistema inspirado no **LinkedIn**.

---

## 🚀 Tecnologias Utilizadas

* **Java 22** + **Spring Boot**
* **MySQL** (dados transacionais)
* **Neo4j** (grafo de relacionamentos)
* **Maven** (gerenciamento de dependências)
* **JWT (JSON Web Token)** para autenticação
* **Postman** (coleção de testes de endpoints)

---

## 📌 Arquitetura do Sistema

O backend está dividido em **dois microsserviços independentes** que se comunicam entre si:

* **[core-service](./core-service/README.md)** → responsável pelos dados transacionais no **MySQL**.
* **[people-graph-service](./people-graph-service/README.md)** → responsável pelos relacionamentos e recomendações no **Neo4j**.

---

## 🛠️ Como Executar o Projeto

### Pré-requisitos

* [Java 22+](https://www.oracle.com/java/technologies/javase/jdk22-archive-downloads.html)
* [Maven](https://maven.apache.org/)
* [MySQL](https://dev.mysql.com/downloads/)
* [Neo4j](https://neo4j.com/download/)

### Passos

1. Clone o repositório principal:

   ```bash
   git clone https://github.com/seu-usuario/linkedin-clone.git
   ```
2. Configure o banco MySQL no **core-service** e o Neo4j no **people-graph-service**.
3. Rode cada microsserviço separadamente:

   ```bash
   cd core-service
   mvn spring-boot:run
   ```

   ```bash
   cd people-graph-service
   mvn spring-boot:run
   ```
4. Teste os endpoints via Postman (coleção disponível no repositório).

---

## 📂 Estrutura do Repositório

```
📦 linkedin-clone
 ┣ 📂 core-service
 ┃ ┗ README.md
 ┣ 📂 people-graph-service
 ┃ ┗ README.md
 ┗ README.md (principal)
```

---

## 👨‍💻 Autor

Vinicius Leal de Melo
Curso: **Análise e Desenvolvimento de Sistemas (ADS)**
Unifacisa - 2025
