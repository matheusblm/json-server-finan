# react-atividade-s5-template-JSON-Server

## Base_URL

https://localhost:3001/

## Users

### Cadastro

POST /register

```json
{
  "email": "usuario@email.com",
  "password": "123456",
  "name": "Usuario",
  "age": 41
}
```

### Login

`POST /login`

```json
{
  "email": "usuario@email.com",
  "password": "123456"
}
```

## Receive

### create new receive

`Post /receive`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos",
  "category": "Férias",
  "description": "Bradesco",
  "type": true,
  "date": "08-11-21",
  "userId": 1
}
```

### get receive

`GET /receive/?userId=:id`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "description": "Bradesco",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### get only receive

`GET /receive/:id`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "description": "Bradesco",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### update receive

`PATCH /receive/:id`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos atualizado",
  "category": "Férias",
  "description": "Bradesco",
  "type": false,
  "date": "08-11-21",
  "userId": 1,
  "id": 1
}
```

### delete receive

`DELETE /receive/:id`

header {
Authorization: Bearer token
}

## Spend

### create new spend

`Post /spend`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos",
  "category": "Férias",
  "description": "Bradesco",
  "type": true,
  "date": "08-11-21",
  "userId": 1
}
```

### get spend

`GET /spend/?userId=:id`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "description": "Bradesco",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### get only spend

`GET /spend/:id`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "description": "Bradesco",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### update spend

`PATCH /spend/:id`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos atualizado",
  "category": "Férias",
  "description": "Bradesco",
  "type": false,
  "date": "08-11-21",
  "userId": 1,
  "id": 1
}
```

### delete spend

`DELETE /spend/:id`

header {
Authorization: Bearer token
}

## Wallet

### create new wallet

`Post /wallet`

header {
Authorization: Bearer token
}

```json
{
  "value": 200,
  "bank": "Nubank",
  "userId": 1
}
```

### get wallet

`GET /wallet/?userId=:id`

```json
[
  {
    "value": 200,
    "bank": "Nubank",
    "userId": 1,
    "id": 1
  }
]
```

### get only wallet

`GET /wallet/:id`

```json
[
  {
    "value": 200,
    "bank": "Nubank",
    "userId": 1,
    "id": 1
  }
]
```

### update wallet

`PATCH /wallet/:id`

header {
Authorization: Bearer token
}

```json
{
  "value": 200,
  "bank": "Nubank",
  "userId": 1,
  "id": 1
}
```

### delete wallet

`DELETE /wallet/:id`

header {
Authorization: Bearer token
}
