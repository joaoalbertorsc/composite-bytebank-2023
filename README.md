# Projeto Composite ByteBank 2023

## Descrição
Este é um projeto simples de sistema bancário desenvolvido como parte dos estudos de programação orientada a objetos em Java. O projeto implementa funcionalidades básicas de um banco, como criação de contas, clientes, depósitos, saques e transferências.

## Estrutura do Projeto

O projeto é composto por três classes principais:

### Client
Representa um cliente do banco com as seguintes propriedades:
- `name`: Nome do cliente
- `cpf`: CPF do cliente
- `profession`: Profissão do cliente

### Account
Representa uma conta bancária com as seguintes propriedades e métodos:
- Propriedades:
  - `balance`: Saldo da conta
  - `agency`: Número da agência
  - `number`: Número da conta
  - `holder`: Titular da conta (referência a um objeto Client)

- Métodos:
  - `deposit(double value)`: Adiciona um valor ao saldo da conta
  - `withdraw(double value)`: Retira um valor do saldo da conta, se houver saldo suficiente
  - `transfer(double value, Account receiver)`: Transfere um valor para outra conta, se houver saldo suficiente

### BankTest
Classe de teste que demonstra o uso das classes Client e Account:
- Cria um cliente (Paulo Silveira)
- Cria uma conta para o cliente
- Realiza um depósito de 100.0 unidades monetárias
- Imprime informações do titular da conta

## Como Executar

Para executar o projeto, você precisa ter o Java instalado em sua máquina. Em seguida, compile os arquivos Java e execute a classe principal:

```bash
javac composite_bytebank/*.java
java composite_bytebank.BankTest
```

## Funcionalidades

- Criação de clientes com informações pessoais
- Criação de contas bancárias
- Operações bancárias básicas (depósito, saque, transferência)
- Associação entre clientes e contas

## Tecnologias Utilizadas

- Java

## Conceitos Aplicados

- Programação Orientada a Objetos
- Encapsulamento
- Associação entre objetos
- Métodos com retorno de valores booleanos para indicar sucesso/falha

## Possíveis Melhorias Futuras

- Implementação de interfaces gráficas
- Persistência de dados em banco de dados
- Adição de mais tipos de contas (poupança, investimento, etc.)
- Implementação de autenticação e segurança
- Histórico de transações