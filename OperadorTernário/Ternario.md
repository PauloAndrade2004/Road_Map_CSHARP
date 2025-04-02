O operador ternário em C# é uma forma simplificada de escrever um `if-else`, tornando o código mais conciso. Ele segue esta sintaxe:

```csharp
condição ? expressão_se_verdadeiro : expressão_se_falso;
```

### Como funciona?
- **Se a condição for `true`**, retorna o valor da primeira expressão.
- **Se a condição for `false`**, retorna o valor da segunda expressão.

### Exemplo básico:
```csharp
int numero = 10;
string resultado = (numero % 2 == 0) ? "Par" : "Ímpar";
Console.WriteLine(resultado); // Saída: Par
```

### Exemplo com `return` em método:
```csharp
static string VerificarIdade(int idade)
{
    return (idade >= 18) ? "Maior de idade" : "Menor de idade";
}

Console.WriteLine(VerificarIdade(20)); // Saída: Maior de idade
```

### Usando operador ternário aninhado:
```csharp
int nota = 85;
string status = (nota >= 90) ? "Ótimo" : (nota >= 70) ? "Bom" : "Ruim";
Console.WriteLine(status); // Saída: Bom
```
(Nesse caso, se `nota >= 90`, retorna `"Ótimo"`, se não, verifica se `nota >= 70`, retornando `"Bom"`, caso contrário retorna `"Ruim"`).

### Quando usar?
- Quando a condição e as expressões são simples.
- Para tornar o código mais enxuto e legível.

### Quando evitar?
- Quando a lógica é complexa e pode dificultar a leitura.
- Quando várias condições precisam ser verificadas (use `if-else` para maior clareza).
