## 📘 Contador com Exceção Personalizada em Java

Este projeto é um exemplo simples em Java que demonstra o uso de:

* Entrada de dados pelo terminal com `Scanner`
* Criação de **exceção personalizada** (`ParametrosInvalidosException`)
* Lançamento de exceções com `throw`
* Tratamento de erros com `try-catch`
* Laço de repetição `for` para contagem simples

---

### 🧠 Objetivo

Receber dois números do usuário e imprimir uma contagem do primeiro até o segundo número.
Se o primeiro número for **maior** que o segundo, o programa **lança uma exceção personalizada** com a mensagem:

> "O segundo parâmetro deve ser maior que o primeiro"

---

### 🛠️ Como funciona o código

1. O programa solicita dois números via `Scanner`:

   ```java
   int parametroUm = terminal.nextInt();
   int parametroDois = terminal.nextInt();
   ```

2. A função `contar(int, int)` é chamada:

   * Se `parametroUm > parametroDois`, uma **exceção personalizada** (`ParametrosInvalidosException`) é lançada.
   * Caso contrário, o programa realiza uma contagem do número 1 até a diferença entre os dois números, imprimindo:

     ```
     Imprimindo o número 1
     Imprimindo o número 2
     ...
     ```

3. O `try-catch` captura a exceção e imprime a mensagem amigável para o usuário.

---

### 🧪 Exemplo de execução

**Entrada do usuário:**

```
Digite o primeiro parâmetro
3
Digite o segundo parâmetro
7
```

**Saída:**

```
Imprimindo o número 1
Imprimindo o número 2
Imprimindo o número 3
Imprimindo o número 4
```

**Se o primeiro for maior:**

```
Digite o primeiro parâmetro
10
Digite o segundo parâmetro
5
```

**Saída:**

```
O segundo parâmetro deve ser maior que o primeiro
```

---

### 📄 Estrutura do projeto

```
Contador.java                 <- Classe principal com lógica de entrada e contagem
ParametrosInvalidosException <- Exceção personalizada (classe interna ou externa)
```

---

### ✅ Conceitos aplicados

* Programação Orientada a Objetos (POO)
* Boas práticas de tratamento de erros
* Encapsulamento de lógica em métodos
* Leitura de dados com `Scanner`

---
