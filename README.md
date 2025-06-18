# Desafio Controle de Fluxo

Este projeto foi desenvolvido como parte do módulo de Controle de Fluxo do Bootcamp Santander 2025, promovido pela plataforma DIO (Digital Innovation One). O objetivo é exercitar conceitos fundamentais de controle de fluxo em Java, como estruturas condicionais, laços de repetição e tratamento de exceções customizadas.

## Proposta do Projeto

O sistema recebe dois parâmetros inteiros via terminal. Com base nesses valores, ele executa as seguintes regras:

- **Cálculo de Interações:**
  - O programa calcula a diferença entre o segundo e o primeiro número, determinando assim a quantidade de interações de um laço `for`.
  - Para cada iteração, imprime no console a mensagem: `Imprimindo o número X`, onde X é o número da iteração.
  - Exemplo: Se os parâmetros forem 12 e 30, serão impressas 18 mensagens, de 1 a 18.

- **Validação de Parâmetros:**
  - Caso o primeiro parâmetro seja maior que o segundo, o sistema lança uma exceção customizada chamada `ParametrosInvalidosException`.
  - Mensagem da exceção: `O segundo parâmetro deve ser maior que o primeiro`.

## Estrutura do Projeto

```
Desafio-controle-fluxo/
│
├── src/
│   ├── Contador.java                  // Classe principal com a lógica do programa
│   └── ParametrosInvalidosException.java // Exceção customizada para validação de parâmetros
├── bin/                               // Arquivos compilados (.class)
├── README.md                          // Este arquivo
```

## Como Executar

1. **Compile o projeto:**

   Abra o terminal na pasta raiz do projeto e execute:
   ```powershell
   javac -d bin src/*.java
   ```

2. **Execute o programa:**

   Ainda no terminal, execute:
   ```powershell
   java -cp bin Contador <primeiroNumero> <segundoNumero>
   ```
   Substitua `<primeiroNumero>` e `<segundoNumero>` pelos valores desejados.

   **Exemplo:**
   ```powershell
   java -cp bin Contador 12 30
   ```

   Saída esperada:
   ```
   Imprimindo o número 1
   Imprimindo o número 2
   ...
   Imprimindo o número 18
   ```

   Caso o primeiro número seja maior que o segundo:
   ```
   java -cp bin Contador 30 12
   ```
   Saída esperada:
   ```
   O segundo parâmetro deve ser maior que o primeiro
   ```

## Tecnologias necessárias para rodar o projeto
- Java 8 ou superior

## Autor
Desenvolvido para conclusão do módulo de Controle de Fluxo do Bootcamp Santander 2025 na plataforma DIO.
