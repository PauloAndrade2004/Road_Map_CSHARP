# Operadores Lógicos em C#

Este documento serve como um guia de estudos sobre operadores lógicos em C#.

## O que são operadores lógicos?
Os operadores lógicos são usados para combinar expressões booleanas (true ou false). Eles ajudam a criar condições mais complexas em estruturas de controle, como `if`, `while` e `for`.

## Tipos de Operadores Lógicos em C#

### 1. `&&` (E Lógico)
Retorna `true` **somente** se **ambas** as expressões forem verdadeiras.

```csharp
bool resultado = true && true;  // true
bool resultado2 = true && false; // false
```

**Exemplo prático:**
```csharp
int idade = 20;
bool temCarteira = true;

if (idade >= 18 && temCarteira)
{
    Console.WriteLine("Pode dirigir!");
}
```

### 2. `||` (OU Lógico)
Retorna `true` se **pelo menos uma** das expressões for verdadeira.

```csharp
bool resultado = true || false;  // true
bool resultado2 = false || false; // false
```

**Exemplo prático:**
```csharp
bool temDinheiro = false;
bool temCartao = true;

if (temDinheiro || temCartao)
{
    Console.WriteLine("Pode fazer a compra!");
}
```

### 3. `!` (NÃO Lógico)
Inverte o valor de uma expressão booleana.

```csharp
bool resultado = !true;  // false
bool resultado2 = !false; // true
```

**Exemplo prático:**
```csharp
bool chovendo = false;

if (!chovendo)
{
    Console.WriteLine("Pode sair sem guarda-chuva!");
}
```

## Resumo da Tabela Verdade
| Expressão 1 | Expressão 2 | `&&` (E) | `||` (OU) |
|-------------|-------------|----------|----------|
| true        | true        | true     | true     |
| true        | false       | false    | true     |
| false       | true        | false    | true     |
| false       | false       | false    | false    |

## Conclusão
Os operadores lógicos são fundamentais para o controle de fluxo em C#. Combinando-os, é possível criar condições mais robustas para os programas.

---
### 📌 Dica
Para praticar, tente criar pequenos programas que utilizem esses operadores em `if`, `while` e outras estruturas!

---
**Criado para

