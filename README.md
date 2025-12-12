<p align="center">
  <img src="https://svg-banners.vercel.app/api?type=origin&text1=Task%20Manager%20Lite%20✨&text2=Spring%20Boot%20API%20REST" width="100%" alt="Task Manager Lite Banner">
</p>

<h1 align="center">📌 Task Manager Lite – API REST em Java + Spring Boot</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Java-17-007396?logo=java" />
  <img src="https://img.shields.io/badge/Spring%20Boot-3.3.4-6DB33F?logo=springboot" />
  <img src="https://img.shields.io/badge/Status-Online-brightgreen" />
  <img src="https://img.shields.io/badge/License-MIT-blue" />
  <a href="https://github.com/SEU-USUARIO">
    <img src="https://img.shields.io/badge/GitHub-RafaelSV9-000?logo=github" />
  </a>
</p>

---

## 🚀 Sobre o Projeto

O **Task Manager Lite** é uma API REST desenvolvida com **Java 17** e **Spring Boot 3**, projetada para demonstrar boas práticas de backend, arquitetura limpa e uso de tecnologias modernas do ecossistema Spring.

Ideal para:
- Estudos de desenvolvimento backend
- Portfólio profissional
- Entrevistas técnicas
- Prática de CRUD, DTOs, validação e camadas

---

## 🧱 Tecnologias Utilizadas

<p align="left">
  <img src="https://img.shields.io/badge/Java-17-007396?logo=java" />
  <img src="https://img.shields.io/badge/Spring%20Boot-3.3-6DB33F?logo=springboot" />
  <img src="https://img.shields.io/badge/H2-Database-blue?logo=h2" />
  <img src="https://img.shields.io/badge/Maven-Build-orange?logo=apachemaven" />
  <img src="https://img.shields.io/badge/JPA-Hibernate-59666C?logo=hibernate" />
</p>

---

## 📂 Arquitetura do Projeto

task-manager-lite/
├── controller/
├── dto/
├── exception/
├── model/
├── repository/
├── service/
└── TaskManagerApplication.java

markdown
Copiar código

- **Controller:** entrada das requisições REST  
- **Service:** regras de negócio  
- **Repository:** persistência com Spring Data JPA  
- **DTOs:** request e response  
- **Exception Handler:** validações e erros padronizados  

---

## ⚙️ Como Rodar

bash
git clone https://github.com/SEU-USUARIO/task-manager-lite.git
cd task-manager-lite
mvn spring-boot:run
Acesse:

bash
Copiar código
http://localhost:8080/api/tasks
📚 Endpoints
🔹 Listar tarefas
GET /api/tasks

🔹 Buscar tarefa por ID
GET /api/tasks/{id}

🔹 Criar nova tarefa
POST /api/tasks

🔹 Atualizar tarefa
PUT /api/tasks/{id}

🔹 Atualizar apenas status
PATCH /api/tasks/{id}/status

🔹 Deletar tarefa
DELETE /api/tasks/{id}

🗄️ Banco H2
Acesse:

bash
Copiar código
http://localhost:8080/h2-console
Configuração:

JDBC URL → jdbc:h2:mem:tasksdb

User → sa

Password → (vazio)

🔧 Tratamento de Erros
Erros retornam payload estruturado:

json
Copiar código
{
  "timestamp": "2025-01-01T10:00:00",
  "status": 400,
  "errors": {
    "title": "Title is mandatory"
  }
}
🛣️ Roadmap / Melhorias Futuras
 Paginação e filtros

 Autenticação JWT

 Swagger/OpenAPI

 Testes unitários (JUnit + Mockito)

 Deploy em Docker

 Deploy AWS (EC2 / Elastic Beanstalk)

👨‍💻 Autor
Rafael dos Santos Vicente
Desenvolvedor Backend | Java | Spring | Cloud

<a href="https://github.com/SEU-USUARIO"> <img src="https://img.shields.io/badge/GitHub-RafaelSV9-000?logo=github" /> </a>

📜 Licença
Este projeto está sob a licença MIT — uso livre para estudos e portfólio.
