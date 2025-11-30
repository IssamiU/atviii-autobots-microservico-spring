# AutoManager 

## Tecnologias

- **Java 17**
- **Spring Boot 2.7.x**
- **Spring Data JPA**
- **Spring HATEOAS**
- **MySQL 8.0**
- **Lombok**
- **Maven**

---

## Requisitos

Antes de executar o projeto, certifique-se de ter instalado:

- [Java JDK 17+](https://www.oracle.com/java/technologies/downloads/)
- [MySQL 8.0+](https://dev.mysql.com/downloads/mysql/)
- [Maven](https://maven.apache.org/download.cgi) (ou use o wrapper incluído)

---

## Como Executar

### 1️Configurar o Banco de Dados

Crie um banco de dados MySQL:

```sql
CREATE DATABASE automanager;
```

### 2️⃣ Configurar application.properties

Edite o arquivo `src/main/resources/application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/automanager
spring.datasource.username=root
spring.datasource.password=SUA_SENHA_AQUI

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
```

### Executar o Projeto

Execute a classe `AutomanagerApplication.java`

### Acessar a Aplicação

A aplicação estará disponível em:
```
http://localhost:8080
```

---

## Rotas da API

## Empresas

| Método | Rota                                      | Descrição                       |
|--------|-------------------------------------------|---------------------------------|
| GET    | `/empresa/empresas`                      | Lista todas as empresas         |
| GET    | `/empresa/{id}`                          | Busca empresa por ID            |
| POST   | `/empresa/cadastrar`                | Cadastra nova empresa           |
| PUT    | `/empresa/atualizar/{id}`                | Atualiza empresa existente      |
| DELETE | `/empresa/excluir/{id}`                  | Exclui empresa                  |
| POST   | `/empresa/{empresaId}/usuario/{usuarioId}` | Associa usuário à empresa     |
| DELETE | `/empresa/{empresaId}/usuario/{usuarioId}` | Remove usuário da empresa      |
| GET    | `/empresa/{empresaId}/usuarios`          | Lista usuários da empresa       |

---

## Usuários

| Método | Rota                       | Descrição                  |
|--------|----------------------------|----------------------------|
| GET    | `/usuario/usuarios`        | Lista todos os usuários    |
| GET    | `/usuario/{id}`            | Busca usuário por ID       |
| POST   | `/usuario/cadastrar`       | Cadastra novo usuário      |
| PUT    | `/usuario/atualizar`       | Atualiza usuário existente |
| DELETE | `/usuario/excluir`         | Exclui usuário             |

---

## Mercadorias

| Método | Rota                       | Descrição                      |
|--------|----------------------------|--------------------------------|
| GET    | `/mercadoria/mercadorias`  | Lista todas as mercadorias     |
| GET    | `/mercadoria/{id}`         | Busca mercadoria por ID        |
| POST   | `/mercadoria/cadastro`     | Cadastra nova mercadoria       |
| PUT    | `/mercadoria/atualizar`    | Atualiza mercadoria existente  |
| DELETE | `/mercadoria/excluir`      | Exclui mercadoria              |

---

## Serviços

| Método | Rota                       | Descrição                  |
|--------|----------------------------|----------------------------|
| GET    | `/servico/servicos`        | Lista todos os serviços    |
| GET    | `/servico/{id}`            | Busca serviço por ID       |
| POST   | `/servico/cadastro`        | Cadastra novo serviço      |
| PUT    | `/servico/atualizar`       | Atualiza serviço existente |
| DELETE | `/servico/excluir`         | Exclui serviço             |

---

## Veículos

| Método | Rota                       | Descrição                  |
|--------|----------------------------|----------------------------|
| GET    | `/veiculo/veiculos`        | Lista todos os veículos    |
| GET    | `/veiculo/{id}`            | Busca veículo por ID       |
| POST   | `/veiculo/cadastrar`       | Cadastra novo veículo      |
| PUT    | `/veiculo/atualizar`       | Atualiza veículo existente |
| DELETE | `/veiculo/excluir`         | Exclui veículo             |

---

## Vendas

| Método | Rota                       | Descrição                  |
|--------|----------------------------|----------------------------|
| GET    | `/venda/vendas`            | Lista todas as vendas      |
| GET    | `/venda/{id}`              | Busca venda por ID         |
| POST   | `/venda/cadastro`          | Cadastra nova venda        |
| PUT    | `/venda/atualizar`         | Atualiza venda existente   |
| DELETE | `/venda/excluir`           | Exclui venda               |

---

## Credenciais

| Método | Rota                       | Descrição                  |
|--------|----------------------------|----------------------------|
| GET    | `/credencial/credenciais`  | Lista todas as credenciais |
| GET    | `/credencial/{id}`         | Busca credencial por ID    |