# Projeto Base - Cypress

Este é um projeto base para testes automatizados utilizando o **Cypress**.

## 🧩 Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- [Node.js](https://nodejs.org/) (recomenda-se a versão **LTS**)
- [Git](https://git-scm.com/)

## 🚀 Passos para rodar o projeto

### 1. Clonar o repositório

```bash
git clone https://github.com/EBAC-QE/ebac-cypress-samples.git
```

### 2. Entrar na pasta do projeto

```bash
cd ebac-cypress-samples
```

### 3. Instalar as dependências

```bash
npm install
```

### 4. Rodar o Cypress (modo interativo)

```bash
npx cypress open
```

### 5. Rodar os testes (modo headless)

```bash
npx cypress run
```


## ⚙️ Integração Contínua (GitHub Actions)

[![Cypress Tests](https://github.com/oct-gustavo/ebac-cypress-samples/actions/workflows/cypress.yml/badge.svg)](https://github.com/oct-gustavo/ebac-cypress-samples/actions/workflows/cypress.yml)

O pipeline está definido em [`.github/workflows/cypress.yml`](.github/workflows/cypress.yml) e executa automaticamente os testes Cypress (modo headless, no Chrome):

- a cada **push** em qualquer branch;
- a cada **pull request** para a branch `main`;
- manualmente, pela aba **Actions** (`workflow_dispatch`).

Em caso de falha, os screenshots são salvos como artefatos da execução.
