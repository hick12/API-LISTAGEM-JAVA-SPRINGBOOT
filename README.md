
---

📌 API de Listagem em Java com Spring Boot

Este projeto é uma API simples de listagem desenvolvida com Java + Spring Boot,
criada para estudos e prática de desenvolvimento de aplicações RESTful.


🚀 Tecnologias Utilizadas
- Java 17+
- Spring Boot
  - Spring Web
  - Spring Test
- Maven (gerenciador de dependências)
- IntelliJ IDEA (IDE utilizada no desenvolvimento)


📂 Estrutura do Projeto
.
├── src
│   ├── main
│   │   ├── java/Varias/apis/demo
│   │   │   ├── Controller/ApiController.java   # Controlador principal
│   │   │   └── ApiDeTarefasApplication.java    # Classe principal (entrypoint)
│   │   └── resources/application.properties    # Configurações da aplicação
│   └── test/java/Varias/apis/demo              # Testes unitários e de integração
├── pom.xml                                     # Dependências Maven
└── README.md                                   # Documentação do projeto

---

## ⚙️ Endpoints Disponíveis

### 🔹 Listar tarefas

```http
GET /task
```

* Retorna todas as tarefas cadastradas.
* Exemplo de resposta:

```json
["Minha tarefa", "Outra tarefa"]
```

### 🔹 Criar uma nova tarefa

```http
POST /task
```

* Adiciona uma nova tarefa enviada no corpo da requisição.
* Corpo da requisição:

```json
"Estudar Spring Boot"
```

### 🔹 Limpar todas as tarefas

```http
DELETE /task
```

* Remove todas as tarefas cadastradas.
* Resposta: `200 OK`

---

## ▶️ Como Executar o Projeto

1. **Clonar o repositório**

   ```bash
   git clone https://github.com/hick12/API-LISTAGEM-JAVA-SPRINGBOOT.git
   cd API-LISTAGEM-JAVA-SPRINGBOOT
   ```

2. **Rodar a aplicação**

   ```bash
   ./mvnw spring-boot:run
   ```

   Ou, no Windows:

   ```bash
   mvnw.cmd spring-boot:run
   ```

3. **Testar no navegador ou via cURL/Postman**

   * [http://localhost:8080/task](http://localhost:8080/task)

---

## 🧪 Testes

O projeto já vem com testes configurados usando **JUnit 5** e **Spring Boot Test**.
Para rodar os testes:

```bash
./mvnw test
```

---

## 📌 Objetivo

Esse projeto tem como objetivo servir de **material de aprendizado**, praticando:

* Estrutura básica de uma API REST em Spring Boot
* Uso de `@GetMapping`, `@PostMapping`, `@DeleteMapping`
* Serialização com `ObjectMapper`
* Boas práticas de versionamento com Git e GitHub

---

## 📄 Licença

Este projeto foi desenvolvido apenas para estudos e **não possui licença comercial**.
Sinta-se à vontade para clonar, modificar e estudar! 🚀


---


