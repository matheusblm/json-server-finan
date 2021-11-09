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

## Account

### create new account

`Post /account`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos",
  "category": "Férias",
  "type": true,
  "date": "08-11-21",
  "userId": 1
}
```

### get account

`GET /account`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### get only account

`GET /account/:id`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
    "type": true,
    "date": "08-11-21",
    "userId": 1,
    "id": 1
  }
]
```

### update account

`PATCH /account/:id`

header {
Authorization: Bearer token
}

```json
{
  "value": 20.0,
  "account": "Empréstimos atualisado",
  "category": "Férias",
  "type": false,
  "date": "08-11-21",
  "userId": 1,
  "id": 1
}
```

### delete account

`DELETE /account/:id`

header {
Authorization: Bearer token
}

## receive

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
  "type": true,
  "date": "08-11-21",
  "userId": 1
}
```

### get receive

`GET /receive`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
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
  "value": 20.00,
    "account": "Empréstimos atualisado",
    "category": "Férias",
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

## spend

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
  "type": true,
  "date": "08-11-21",
  "userId": 1
}
```

### get spend

`GET /spend`

```json
[
  {
    "value": 20.0,
    "account": "Empréstimos",
    "category": "Férias",
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
  "value": 20.00,
    "account": "Empréstimos atualisado",
    "category": "Férias",
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