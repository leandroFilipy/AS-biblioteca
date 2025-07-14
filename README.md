# 📚 Sistema de Gerenciamento de Biblioteca

Este projeto descreve o **modelo de dados** e a **estrutura do sistema** de uma biblioteca digital, com foco no gerenciamento de livros, usuários, empréstimos e devoluções.

---

## 🧩 Diagrama de Entidade-Relacionamento (ER)

O sistema foi modelado utilizando um **diagrama ER** criado no Draw.io, contendo as principais entidades e seus relacionamentos.

---

## 🗂️ Entidades Principais

### 📘 LIVRO
- `ID_LIVRO` (PK)
- `TÍTULO`
- `AUTOR`
- `EDITORA`
- `ANO_PUBLICAÇÃO`
- `CATEGORIA`
- `EXEMPLARES_DISPONÍVEIS`

### 👤 USUÁRIO
- `ID_USUARIO` (PK)
- `NOME`
- `CPF`
- `EMAIL`
- `TELEFONE`

### 📄 EMPRÉSTIMO
- `ID_EMPRESTIMO` (PK)
- `ID_USUARIO` (FK)
- `ID_LIVRO` (FK)
- `DATA_EMPRESTIMO`
- `DATA_DEVOLUÇÃO`
- `STATUS` (ativo/devolvido)

### 🕘 RESERVA
- `ID_RESERVA` (PK)
- `ID_USUARIO` (FK)
- `ID_LIVRO` (FK)
- `DATA_RESERVA`

---

## 🔗 Relacionamentos

- Um **usuário** pode realizar vários **empréstimos** e **reservas**.
- Um **livro** pode estar associado a múltiplos **empréstimos** e **reservas**.
- **Chaves estrangeiras** garantem a integridade dos vínculos entre entidades.

---

## 💡 Funcionalidades Esperadas do Sistema

- Cadastro e consulta de livros e usuários
- Registro e controle de empréstimos
- Sistema de reservas com prioridade por ordem de solicitação
- Histórico de empréstimos por usuário
- Relatórios de disponibilidade e atraso

---

## 🛠️ Tecnologias Sugeridas

- **Banco de Dados:** MySQL ou PostgreSQL
- **Backend:** Java, Python (Django/Flask) ou Node.js
- **Frontend (opcional):** HTML + CSS + JavaScript (ou React)

---

## 📄 Licença

Este projeto é de uso educacional. Sem fins comerciais. Licenciado sob a [MIT License](LICENSE).

---

## ✍️ Autor

Modelo desenhado por **Leandro** no Draw.io

---



---
