### Resumo sobre Funções em C#  

#### 📌 **O que são funções?**  
Funções (ou métodos) são blocos de código reutilizáveis que executam uma tarefa específica.  

#### 📌 **Sintaxe básica:**  
```csharp
TipoRetorno NomeDaFuncao(Tipo parametro1, Tipo parametro2)  
{  
    // Código da função  
    return valor; // Se houver retorno  
}
```

#### 📌 **Principais pontos:**  
✅ **Declaração:** Definem um tipo de retorno, nome e parâmetros opcionais.  
✅ **Parâmetros:** Podem ser obrigatórios, opcionais ou com valores padrão.  
✅ **Retorno:** Pode ser `void` (sem retorno) ou de um tipo específico (`int`, `string`, `bool`, etc.).  
✅ **Modificadores:**  
   - `static` → Pertence à classe, sem precisar de instância.  
   - `public` → Acessível de fora da classe.  
   - `private` → Acessível apenas dentro da classe.  

#### 📌 **Exemplo:**  
```csharp
class Program  
{  
    static void Main()  
    {  
        int resultado = Somar(5, 3);  
        Console.WriteLine(resultado); // Saída: 8  
    }  

    static int Somar(int a, int b)  
    {  
        return a + b;  
    }  
}
```

#### 📌 **Outros conceitos úteis:**  
🔹 **Sobrecarga (Overloading):** Funções com o mesmo nome, mas parâmetros diferentes.  
🔹 **Funções assíncronas:** Usam `async` e `await` para operações assíncronas.  
🔹 **Funções anônimas e expressões lambda:** Para criar funções rápidas e curtas.  

Se precisar de mais detalhes sobre algum ponto, só perguntar! 🚀
