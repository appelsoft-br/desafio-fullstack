# Desafio Técnico - Mini Sistema de Controle Financeiro (Full-stack)

## Objetivo
Desenvolver um mini sistema de controle financeiro para gerenciar contas de entrada e saída, utilizando **Angular** no front-end e **Laravel** no back-end. O candidato deve demonstrar habilidades em desenvolvimento full-stack, boas práticas de codificação, e integração entre front-end e back-end por meio de uma API REST.

## Requisitos do Projeto:

### 1. Cadastro de Transações (Front-end e Back-end)
- Deve ser possível cadastrar transações financeiras com as seguintes informações:
  - Tipo de transação: Entrada ou Saída
  - Descrição da transação
  - Valor
  - Data
- As transações devem ser armazenadas em um banco de dados via API REST desenvolvida com **Laravel**.

### 2. Listagem de Transações (Front-end e Back-end)
- Exibir uma lista de todas as transações cadastradas, com as seguintes colunas:
  - Tipo (Entrada ou Saída)
  - Descrição
  - Valor
  - Data
- A listagem de transações deve ser consumida da API Laravel.

### 3. Resumo Financeiro (Front-end e Back-end)
- Mostrar o saldo total atual (diferença entre entradas e saídas).
- Exibir o total de entradas e o total de saídas separadamente.
- O cálculo do saldo e dos totais deve ser feito no back-end e retornado pela API.

### 4. Funcionalidades Extras
- Filtro por tipo de transação (Entrada ou Saída).
- Ordenação das transações por data ou valor.

## Requisitos Técnicos (Front-end):
- **Framework**: Utilizar **Angular** (versão 11 ou superior).
- **Roteamento**: Implementar uma estrutura de rotas para navegação, por exemplo:
  - Página de Cadastro de Transações
  - Página de Listagem de Transações
  - Página de Resumo Financeiro
- **Estilização**: Utilizar **CSS** ou **Sass** (preferencialmente com **Angular Material** ou **Bootstrap** para estilização de componentes).
- **Validação de Formulário**: Implementar validações nos formulários utilizando os recursos do **Reactive Forms** do Angular.
- **Responsividade**: A interface deve ser responsiva, adaptando-se a diferentes tamanhos de tela.

## Requisitos Técnicos (Back-end):
- **Framework**: Utilizar **Laravel** (versão 10 ou superior) para construir a API REST.
- **API**: Implementar os seguintes endpoints:
  - `GET /api/transacoes`: Listar todas as transações.
  - `POST /api/transacoes`: Criar uma nova transação.
  - `GET /api/transacoes/{id}`: Obter uma transação específica.
  - `PUT /api/transacoes/{id}`: Atualizar uma transação.
  - `DELETE /api/transacoes/{id}`: Excluir uma transação.
  - `GET /api/resumo`: Obter o resumo financeiro (total de entradas, saídas e saldo).
- **Banco de Dados**: Utilizar **MySQL** para armazenar as transações.
- **Validações**: Implementar validações no back-end para garantir que os campos obrigatórios sejam preenchidos e os valores sejam válidos.
- **Autenticação**: Utilizar **JWT** para autenticar as requisições da API (não obrigatório, mas um diferencial).

## Critérios de Avaliação:
- **Full-stack**: Integração correta entre front-end e back-end por meio de requisições HTTP.
- **Qualidade do código**: Organização, boas práticas, clareza e estrutura do código tanto no front-end quanto no back-end.
- **Usabilidade da interface**: Simplicidade, clareza e facilidade de uso.
- **Validações de dados e tratamento de erros**: Validações de formulários no Angular e validações no back-end com Laravel.
- **Utilização de componentes e serviços reutilizáveis no front-end**.
- **Estrutura de rotas organizada no Angular e na API**.
- **Documentação**: README explicando como rodar o projeto localmente e as rotas da API.

## Diferenciais (não obrigatórios):
- Uso de **TypeScript** avançado no Angular (Interfaces, Enums, Generics).
- Implementação de autenticação com **JWT** no Laravel e integração com o front-end.

## Entrega:
O candidato deve disponibilizar o código em um repositório público no GitHub e incluir instruções de como rodar o projeto localmente, tanto o front-end quanto o back-end.

## Estrutura sugerida de pastas:
```bash
mini-sistema-financeiro/
├── backend/         # Diretório Laravel
│   └── ...
└── frontend/        # Diretório Angular
    └── ...
