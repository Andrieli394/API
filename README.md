# Roteiro QA - Introdução à API

### Introdução à API

Bem-vindo à API de Exemplo.
Essa API permite integração simples com os principais recursos do sistema, oferecendo endpoints para consulta, cadastro e atualização de dados.

### Autenticação

A autenticação é realizada via token enviado no header das requisições:

```json
Authorization: Bearer {seu_token_aqui}

```
### Formato de Resposta

Todas as respostas são retornadas em **JSON** no seguinte formato:

```json
{
  "success": true,
  "data": { ... },
  "message": "Operação realizada com sucesso"
}

```

## Endpoints Principais

### Listar Registros
```json
GET /api/v1/registros

```

### Criar Registro

```json
POST /api/v1/registros
Body: {
  "nome": "Exemplo",
  "descricao": "Registro de teste"
}

```
### Atualizar Registro

```json
PUT /api/v1/registros/{id}

```

### Excluir Registro

```json
DELETE /api/v1/registros/{id}

```

