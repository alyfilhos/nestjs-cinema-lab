# API de Gerenciamento de Usuários com NestJS, Prisma e SQLite

API REST desenvolvida com **NestJS**, **Prisma ORM** e **SQLite** para gerenciamento de usuários, perfis e endereços.

## Tecnologias utilizadas

- **Node.js**
- **NestJS**
- **Prisma ORM**
- **SQLite**
- **TypeScript**
- **Swagger**
- **Class Validator**

---

## Funcionalidades

A API permite:

- cadastrar perfis;
- cadastrar usuários;
- cadastrar endereços;
- listar registros;
- buscar registros por ID;
- atualizar registros;
- remover registros.

### Relacionamentos

- Um **Profile** pode estar associado a vários **User**;
- Um **User** pertence a um único **Profile**;
- Um **User** pode possuir um único **Address**;
- Um **Address** pertence a um único **User**.

---

## Estrutura das entidades

### Profile
- `id`
- `name`
- `createdAt`
- `updatedAt`

### User
- `id`
- `email`
- `password`
- `name`
- `profileId`
- `createdAt`
- `updatedAt`

### Address
- `id`
- `street`
- `number`
- `city`
- `state`
- `zipCode`
- `userId`
- `createdAt`
- `updatedAt`

---

## Pré-requisitos

Antes de executar o projeto, é necessário ter instalado:

- **Node.js**
- **npm**

---

## Instalação

Clone o repositório:

```bash
git clone https://github.com/alyfilhos/nestjs-cinema-lab.git
cd nestjs-user-management-api
