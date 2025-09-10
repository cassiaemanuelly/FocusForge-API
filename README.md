# FocusForge

**API RESTful para gerenciamento de tarefas e produtividade.**

O **FocusForge** é um projeto de back-end desenvolvido para gerenciar listas de tarefas de forma eficiente. A API permite realizar operações de criação, leitura, atualização e exclusão (CRUD) de tarefas, servindo como uma base sólida para qualquer aplicativo de front-end que precise de funcionalidades de produtividade.

## 🚀 Tecnologias Utilizadas
- **Java:** Linguagem de programação principal.
- **Spring Boot:** Framework para desenvolvimento rápido de APIs.
- **Spring Data JPA:** Para a camada de acesso a dados.
- **H2 Database:** Banco de dados em memória, ideal para desenvolvimento e testes.
- **Maven:** Ferramenta de automação de construção e gerenciamento de dependências.
- **Lombok:** Biblioteca para reduzir código repetitivo (getters, setters, etc.).

## ✨ Funcionalidades
- **Criar Tarefa:** Adicione uma nova tarefa com título, descrição e status de conclusão.
- **Listar Tarefas:** Recupere todas as tarefas existentes.
- **Buscar Tarefa por ID:** Consulte os detalhes de uma tarefa específica.
- **Atualizar Tarefa:** Modifique os dados de uma tarefa existente.
- **Deletar Tarefa:** Remova uma tarefa do banco de dados.

## 🛠️ Como Executar o Projeto

### **Pré-requisitos**
- [Java Development Kit (JDK) 17 ou superior](https://www.oracle.com/java/technologies/downloads/)
- [Maven](https://maven.apache.org/download.cgi)
- Uma IDE de sua preferência (IntelliJ IDEA, VS Code, etc.)

### **Passos para Execução**
1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/FocusForge.git](https://github.com/seu-usuario/FocusForge.git)
    ```
2.  **Navegue até o diretório do projeto:**
    ```bash
    cd FocusForge
    ```
3.  **Compile e execute a aplicação (usando Maven):**
    ```bash
    ./mvnw spring-boot:run
    ```
    A aplicação será iniciada na porta padrão `8080`.

## 🧪 Endpoints da API

Você pode testar a API usando ferramentas como **Postman** ou **Swagger**.
A seguir, estão os principais endpoints disponíveis:

### **Tarefas (`/tasks`)**

| Método | URL                  | Descrição                                 |
| :----- | :------------------- | :---------------------------------------- |
| `POST`   | `/tasks`             | Cria uma nova tarefa.                     |
| `GET`    | `/tasks`             | Retorna a lista de todas as tarefas.       |
| `GET`    | `/tasks/{id}`        | Retorna uma tarefa pelo ID.               |
| `PUT`    | `/tasks/{id}`        | Atualiza uma tarefa existente pelo ID.    |
| `DELETE` | `/tasks/{id}`        | Deleta uma tarefa pelo ID.                |

**Exemplo de corpo de requisição (POST/PUT):**
```json
{
  "title": "Configurar o projeto FocusForge",
  "description": "Adicionar o código e o README.md no GitHub.",
  "completed": false
}
