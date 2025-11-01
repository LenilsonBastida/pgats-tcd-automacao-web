# PGATS - Trabalho de Conclusão da Disciplina - Automação Web com Cypress

Este projeto contém a automação de testes do site [Automation Exercise](https://automationexercise.com/), desenvolvido como trabalho de conclusão da disciplina.

## 🎯 Casos de Teste Implementados

✅ TC 1: Register User
✅ TC 2: Login User with correct email and password
✅ TC 3: Login User with incorrect email and password
✅ TC 4: Logout User
✅ TC 5: Register User with existing email
✅ TC 6: Contact Us Form
✅ TC 8: Verify All Products and product detail page
✅ TC 9: Search Product
✅ TC 10: Verify Subscription in home page
✅ TC 15: Place Order: Register before Checkout

## 📁 Estrutura do Projeto

```
cypress/
    ├── e2e/              # Arquivos de teste
    ├── fixtures/         # Dados de teste
    └── support/          # Comandos customizados e configurações
modules/
    ├── cadastro/         # Módulo de cadastro
    ├── carrinho/         # Módulo de carrinho
    ├── contato/          # Módulo de contato
    ├── login/           # Módulo de login
    ├── menu/            # Módulo de menu
    ├── produtos/        # Módulo de produtos
    ├── subscription/    # Módulo de inscrição
    └── testflows/       # Fluxos de teste
```

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/LenilsonBastida/pgats-tcd-automacao-web.git
```

2. Instale as dependências:
```bash
npm install
```

3. Execute os testes:
- Para abrir o Cypress Test Runner:
```bash
npm run cypress:open
```
- Para executar os testes em modo headless:
```bash
npm run cypress:run
```

## 🧩 Modularização

O projeto foi estruturado de forma modular, onde cada funcionalidade principal do sistema possui seu próprio módulo. Esta abordagem permite:

- Melhor organização do código
- Reusabilidade de componentes
- Manutenção simplificada
- Separação clara de responsabilidades

## 📋 Dados Dinâmicos

Para garantir a independência dos testes e evitar problemas com dados estáticos, utilizamos:

- Geração dinâmica de emails
- Dados aleatórios para cadastros
- Fixtures para dados base
- Comandos customizados para geração de dados

## 🚀 Pipeline GitHub Actions

O projeto está configurado com GitHub Actions para execução automatizada dos testes em ambiente de CI/CD. A pipeline inclui:

- Execução dos testes em cada push para a branch main
- Geração de relatórios de teste
- Armazenamento de artefatos (screenshots e vídeos)
- Notificação de resultados

Para visualizar as execuções, acesse a aba "Actions" no repositório do GitHub.