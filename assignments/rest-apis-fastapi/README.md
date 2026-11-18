# 📘 Atividade: Criando APIs REST com FastAPI

## 🎯 Objetivo

Construa uma API REST com FastAPI, praticando rotas, validação de dados com Pydantic e os métodos HTTP `GET`, `POST`, `PUT` e `DELETE`. Ao final, você terá um serviço que cria, lista, atualiza e remove tarefas.

## 📝 Tarefas

### 🛠️ Criar a Primeira Rota

#### Descrição
Crie um arquivo `main.py` com uma aplicação FastAPI e duas rotas `GET`. Antes de começar, instale as dependências com `pip install fastapi uvicorn` e rode o servidor com `uvicorn main:app --reload`. Depois acesse `http://127.0.0.1:8000/docs` para ver a documentação gerada automaticamente.

#### Requisitos
O programa concluído deve:

- Criar uma instância de `FastAPI` chamada `app`.
- Responder a `GET /` com a mensagem `{"mensagem": "API de tarefas no ar!"}`.
- Responder a `GET /saudacao/{nome}` com `{"mensagem": "Olá, <nome>!"}`, substituindo `<nome>` pelo valor recebido na URL.
- Exibir as duas rotas na página `/docs`.

Exemplo de saída:

```text
GET /saudacao/Maria
Resposta: {"mensagem": "Olá, Maria!"}
```

### 🛠️ Criar e Listar Tarefas

#### Descrição
Crie um modelo de dados com Pydantic para representar uma tarefa e implemente as rotas que criam e listam tarefas. Use uma lista em memória para guardar os dados, sem banco de dados.

#### Requisitos
O programa concluído deve:

- Definir uma classe `Tarefa` (herdando de `BaseModel`) com os campos `id` (inteiro), `titulo` (texto) e `concluida` (booleano, com valor padrão `False`).
- Responder a `POST /tarefas` recebendo um JSON com `titulo` e retornando a tarefa criada com um `id` gerado automaticamente.
- Responder a `GET /tarefas` retornando a lista de todas as tarefas cadastradas.
- Responder com status `422` quando o `titulo` não for enviado no `POST`. O FastAPI faz essa validação automaticamente se o modelo estiver correto.

Exemplo de entrada e saída:

```text
POST /tarefas
Entrada: {"titulo": "Estudar FastAPI"}
Saída:   {"id": 1, "titulo": "Estudar FastAPI", "concluida": false}
```

### 🛠️ Buscar, Atualizar e Remover Tarefas

#### Descrição
Complete o CRUD da API. Você deve permitir buscar uma tarefa pelo `id`, atualizá-la e removê-la. Quando a tarefa não existir, a API deve responder com erro `404`.

#### Requisitos
O programa concluído deve:

- Responder a `GET /tarefas/{id}` retornando a tarefa correspondente.
- Responder a `PUT /tarefas/{id}` substituindo `titulo` e `concluida` pelos valores recebidos.
- Responder a `DELETE /tarefas/{id}` removendo a tarefa e retornando uma mensagem de confirmação.
- Retornar status `404` com a mensagem `"Tarefa não encontrada"` quando o `id` não existir, usando `HTTPException`.
- Testar todas as rotas pela página `/docs` e confirmar que as respostas batem com os exemplos acima.

Exemplo de erro:

```text
GET /tarefas/99
Saída: status 404, {"detail": "Tarefa não encontrada"}
```
