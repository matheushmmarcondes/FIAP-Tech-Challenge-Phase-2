# PAID Backend - Tech Challenge

API REST desenvolvida com **Node.js**, **Express** e **MongoDB** como parte do **Tech Challenge - Fase 2 (FIAP)**.

---

## 🎯 Objetivo

Desenvolver uma API de blogging para permitir que professores publiquem conteúdos educacionais de forma estruturada, incluindo:

- criação de postagens
- listagem de posts
- leitura por ID
- edição
- exclusão
- busca por palavra-chave

---

## 🚀 Tecnologias utilizadas

- Node.js
- Express.js
- MongoDB
- Mongoose
- Docker
- Docker Compose
- Jest
- Supertest
- Swagger (OpenAPI)
- GitHub Actions (CI/CD)

---

## 🧱 Arquitetura do projeto

O projeto foi estruturado utilizando o padrão **MVC (Model-View-Controller)**:

```
src/
├── config/
├── controllers/
├── middlewares/
├── models/
├── routes/
├── app.js
└── server.js
```

---

## ⚙️ Execução local

### 1. Instalar dependências

```bash
npm install
```

### 2. Criar arquivo `.env`

```env
PORT=3000
MONGO_URI=mongodb://localhost:27017/blogdb
```

### 3. Subir o MongoDB com Docker

```bash
docker compose up -d mongo
```

### 4. Rodar a aplicação

```bash
npm run dev
```

---

## 🐳 Execução com Docker (recomendado)

Subir aplicação + banco de dados:

```bash
docker compose up --build
```

Aplicação disponível em:

```
http://localhost:3000
```

---

## 📄 Documentação da API (Swagger)

A documentação interativa está disponível em:

```
http://localhost:3000/api-docs
```

Nela é possível testar todos os endpoints diretamente.

---

## 📡 Endpoints principais

| Método | Endpoint | Descrição |
|--------|----------|----------|
| GET | /api/posts | Lista todos os posts |
| GET | /api/posts/:id | Retorna um post por ID |
| POST | /api/posts | Cria um novo post |
| PUT | /api/posts/:id | Atualiza um post |
| DELETE | /api/posts/:id | Remove um post |
| GET | /api/posts/search?q= | Busca por palavra-chave |

---

## 🧪 Testes automatizados

Executar testes:

```bash
npm test
```

Gerar relatório de cobertura:

```bash
npx jest --coverage
```

✔ O projeto atende ao requisito mínimo de **20% de cobertura de testes**  
✔ Cobertura atual: aproximadamente **80%**

---

## ⚙️ Integração contínua (CI/CD)

O projeto utiliza **GitHub Actions** para executar automaticamente os testes a cada push ou pull request.

---

## 🧠 Boas práticas implementadas

- Estrutura em MVC
- Separação de responsabilidades
- Tratamento global de erros
- Middleware para rotas não encontradas
- Validação de dados de entrada
- Testes automatizados
- Documentação com Swagger
- Containerização com Docker
- Pipeline CI/CD

---

## 📦 Entregáveis do projeto

- Código-fonte versionado no GitHub
- API funcional com endpoints REST
- Containerização com Docker
- Pipeline de CI/CD
- Documentação técnica (README + Swagger)
- Testes automatizados com cobertura

---

## 📚 Experiências e desafios

Durante o desenvolvimento do projeto, alguns desafios foram enfrentados:

- Integração entre Node.js e MongoDB utilizando Mongoose;
- Configuração do ambiente Docker para rodar aplicação e banco de dados simultaneamente;
- Ajustes no pipeline de CI/CD com GitHub Actions, especialmente na configuração de caminhos e dependências;
- Implementação de testes automatizados garantindo cobertura mínima exigida (De longe foi o mais trabalhoso).

Esse desafio me serviu de início no Backend de uma forma mais especialista e aprofundada, no começo confesso que não acreditei que conseguiria, me sinto realizado após a conclusão desse desafio, e me sinto ansioso para explorar mais o que a pós tem a oferecer.

---

## 👨‍💻 Autor

Matheus Henrique Macedo Marcondes  
Tech Challenge - Fase 2 | FIAP
