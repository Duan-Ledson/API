# API de Gerenciamento de Tarefas

## Introdução
Esta API foi desenvolvida utilizando **Spring Boot** e fornece um conjunto de endpoints para gerenciar uma lista simples de tarefas (**tasks**). A API permite listar, adicionar e limpar todas as tarefas armazenadas em memória.

## Tecnologias Utilizadas
- **Java** (JDK 11 ou superior)
- **Spring Boot**
- **Jackson** (para manipulação de JSON)
- **Maven** (para gerenciamento de dependências)

## Instalação e Execução
### 1. Clonar o repositório:
```bash
 git clone https://github.com/seu-usuario/seu-repositorio.git
```

### 2. Acesse o diretório do projeto:
```bash
 cd seu-repositorio
```

### 3. Construir o projeto com Maven:
```bash
 mvn clean install
```

### 4. Executar a aplicação:
```bash
 mvn spring-boot:run
```

A API será iniciada e estará disponível em `http://localhost:8080`.

## Endpoints Disponíveis

### 1. Listar todas as tarefas
**Endpoint:** `GET /tasks`

**Descrição:** Retorna a lista de todas as tarefas armazenadas.

**Exemplo de Resposta:**
```json
["Comprar café", "Finalizar relatório"]
```

---
### 2. Criar uma nova tarefa
**Endpoint:** `POST /tasks`

**Descrição:** Adiciona uma nova tarefa à lista.

**Body (Exemplo):**
```json
"Estudar Spring Boot"
```

**Resposta:**
- `200 OK` caso a tarefa seja adicionada com sucesso.

---
### 3. Excluir todas as tarefas
**Endpoint:** `DELETE /tasks`

**Descrição:** Remove todas as tarefas da lista.

**Resposta:**
- `200 OK` caso a lista seja esvaziada com sucesso.

## Considerações Finais
Este é um exemplo simples de uma API REST utilizando Spring Boot. Como as tarefas são armazenadas em memória, elas serão perdidas ao reiniciar a aplicação. Para persistência de dados, pode-se utilizar um banco de dados relacional como MySQL ou PostgreSQL.

