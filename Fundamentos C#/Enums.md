São dados especiais que servem para associar conjuntos de constantes a números inteiros.

```csharp
namespace ExemploEnums
{
    enum DiaDaSemana
    {
        Domingo,
        Segunda,
        Terça,
        Quarta,
        Quinta,
        Sexta,
        Sábado
    }

    class Program
    {
        static void Main(string[] args)
        {
            DiaDaSemana hoje = DiaDaSemana.Quarta;

            Console.WriteLine($"Hoje é {hoje}");
        }
    }
```
Anatomia se parece com o Structs, transformamos o 'Enum DiaDaSemana' em um tipo que pode ser usado em partes do código.
Boas práticas -> Usamos o 'E' maiúsculo no começo do nome do enum para facilitação da leitura e entendimento do código, então no exemplo anterior, seria uma ótima ideia modificar para 'EDiaDaSemana'.