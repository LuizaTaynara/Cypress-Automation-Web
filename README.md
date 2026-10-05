# 🧪 Cypress Web Automation — Automation Exercise

## 📌 Sobre o projeto

Projeto de **automação de testes web com Cypress**, utilizando o [Automation Exercise](https://www.automationexercise.com/) como ambiente de testes.

O projeto foi desenvolvido para praticar a automação de fluxos de usuário, incluindo **login, registro e exclusão de conta**, além do uso de diferentes seletores, campos de formulário e validações.

## 🎯 Objetivos

* Praticar automação de testes web com Cypress.
* Automatizar cenários de login e registro.
* Trabalhar com diferentes elementos de formulário.
* Utilizar seletores para localizar elementos.
* Criar validações com assertions.
* Trabalhar com cenários positivos e negativos.
* Automatizar o fluxo de exclusão de uma conta.

## 🧪 Testes realizados

### 🔐 Login

Foram automatizados cenários de:

* Login com usuário e senha válidos.
* Login com usuário e senha inválidos.
* Login com usuário válido e senha inválida.
* Login com usuário inválido e senha válida.

Para os cenários de login inválido, é validada a mensagem:

```text
Your email or password is incorrect!
```

No login realizado com sucesso, é validada a mensagem:

```text
Logged in as Teste Cypress
```

### 👤 Registro de usuário

Foram automatizados cenários de:

* Registro de um novo usuário.
* Registro utilizando um e-mail já existente.

No cadastro de um novo usuário, são preenchidos dados de conta e endereço, utilizando diferentes tipos de campos, incluindo opções de seleção e checkbox.

Após o cadastro, é validada a mensagem:

```text
Account Created!
```

Também é validado o login automático após a criação da conta.

Quando é utilizado um e-mail já cadastrado, é validada a mensagem:

```text
Email Address already exist!
```

### 🗑️ Exclusão de usuário

Também foi automatizado o fluxo de exclusão de uma conta:

```text
Login
  ↓
Delete Account
  ↓
Account Deleted!
  ↓
Continue
```

Após a exclusão, é validada a mensagem:

```text
Account Deleted!
```

## 🔍 Validações

Durante os testes são utilizadas validações para verificar, entre outros pontos:

* Visibilidade de elementos.
* Mensagens apresentadas pela aplicação.
* Estado de checkbox.
* Valores selecionados em campos `select`.
* Login realizado com sucesso.
* Criação da conta.
* Exclusão da conta.

Exemplo:

```javascript
cy.contains('Account Created!').should('be.visible');
```

## 🛠️ Tecnologias e ferramentas

* Cypress
* JavaScript
* Node.js
* Git / GitHub

## 🚀 Como executar

Instalar as dependências:

```bash
npm install
```

Abrir o Cypress:

```bash
npx cypress open
```

Executar os testes pelo terminal:

```bash
npx cypress run
```

## 📚 Conceitos praticados

* Automação de testes web
* Cypress
* JavaScript
* Seletores
* Navegação
* Formulários
* Checkboxes
* Selects
* Assertions
* Cenários positivos e negativos

---

#### Projeto desenvolvido para praticar **automação de testes web com Cypress**, utilizando o Automation Exercise como ambiente de testes.

## 👩🏻‍💻 Autora

- **Luiza Santos**
- **Projeto:** Practical Manual Testing — SauceDemo
- **Ano:** 2026

## Vamos conectar?
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/luizataynara/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LuizaTaynara)
