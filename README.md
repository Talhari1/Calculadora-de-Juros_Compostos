# 💰 Calculadora de Juros Compostos em Python

Este projeto é uma **calculadora de juros compostos** feita em Python, desenvolvida como parte de um desafio de programação para iniciantes. A calculadora utiliza a fórmula matemática de juros compostos para calcular o valor total que um cliente deve pagar após realizar um empréstimo bancário com base em uma taxa de juros anual e um período de tempo determinado.

---

## 📘 Sobre o Projeto

A fórmula utilizada para o cálculo é:

\[
\text{Valor Final} = A \times (1 + \frac{p}{100})^n
\]

Onde:
- `A` = valor emprestado (capital inicial)
- `p` = taxa de juros anual (em %)
- `n` = número de anos

O objetivo é ajudar iniciantes em Python a entender conceitos básicos como entrada de dados, operações matemáticas e formatação de saída.

---

## 🛠️ Tecnologias Usadas

- Python 3.x
- [Replit](https://replit.com/) (ambiente de desenvolvimento online)

---

## 🚀 Como Executar (via Replit)

1. Acesse o projeto clicando no link abaixo:  
   👉 [Acessar no Replit](https://replit.com/@vinicius4511/ProjetoPython)

2. Clique em **"Run"** para executar o código no console.

---

## 🧪 Exemplo de Uso

```text
Quanto será emprestado? 10000
Qual a taxa de juros anual do banco? 8
Por quanto tempo? 2

O valor total que o cliente deverá pagar será de R$ 11664.00



---

## 📚 Entendendo o Código

### ✅ Passo a Passo do Desenvolvimento

1. **Entrada de dados**
   - Usamos `input()` para perguntar ao usuário os três valores necessários:
     - Valor emprestado
     - Taxa de juros anual
     - Tempo em anos
   - Convertidos com `float()` ou `int()` para poder fazer cálculos.

2. **Cálculo com a fórmula**
   - Utilizamos a fórmula dos juros compostos:
     \[
     \text{Valor Final} = A \times (1 + \frac{p}{100})^n
     \]
   - `A` é o valor emprestado, `p` é a taxa, e `n` é o tempo.

3. **Saída formatada**
   - Usamos `print()` com `:.2f` para mostrar o valor em reais com duas casas decimais, como `R$ 11664.00`.

---

### 🧠 Por que usei essas coisas?

| Elemento do Código | Por quê? |
|--------------------|----------|
| `float()`          | Para aceitar valores com casas decimais (como 8.5%) |
| `int()`            | Para o tempo em anos, pois são números inteiros |
| `input()`          | Para ler dados do usuário no console |
| `**`               | Operador de potência em Python |
| `:.2f`             | Para formatar como valor em reais com 2 casas decimais |

---

### 🧪 Código Python Comentado

```python
# 1. Solicita o valor emprestado
valor_emprestado = float(input("Quanto será emprestado? "))

# 2. Solicita a taxa de juros anual
taxa_juros = float(input("Qual a taxa de juros anual do banco? "))

# 3. Solicita o número de anos
anos = int(input("Por quanto tempo? "))

# 4. Calcula o valor final com a fórmula de juros compostos
valor_total = valor_emprestado * (1 + taxa_juros / 100) ** anos

# 5. Mostra o resultado formatado
print(f"\nO valor total que o cliente deverá pagar será de R$ {valor_total:.2f}")
