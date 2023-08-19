Classes Estaticas ->
public static void Funcao() {} ->
Ela não consegue ser instanciada -> pois quando rola o start da aplicação, ela já fica disponível para a memória da aplicação.
Geralmente usadas para coisas em que queremos que fique disponíveis para toda a aplicação -> como por exemplo o consumo de uma API ou configurações de coisas reutilizáveis.

-----
Classes Seladas -> Onde queremos selar uma classe, ou seja, não deixar que seja estendida para outras classes ->
public sealed class Pagamento {}

---------
Partial Class -> utilizando o namespace, posso ter a mesma classe em outros arquivos ->
Arquivo 01 -> 
````
namespace Pagamentos
{
	public class Pagamento{}
}
`````
Arquivo 02 ->
````
namespace Pagamentos
{
	public partial class Pagamento{}
}
`````
desta maneira eu consigo separar em diversos pedaços a mesma classe, pois o compilador irá saber o que fazer.

-----
Interfaces -> Como se fosse um contrato, ele determina como uma classe dever ser, exemplo ->
Sempre começamos com a letra i maiúscula no começo do nome da interface.
````
public interface IPagamento {
	DateTime Vencimento { get; set; }
	void Pagar(double Valor); -> // definindo COMO um pagamento TEM QUE SER.
}
`````
Diferença entre classes e interfaces é que interfaces não contém implementações, ou seja, não devemos chamar funções dentro dela ->
As interfaces não define como fazer, ele diz o que precisa ser feito.

----
Classes abstratas -> 
````
public abstract class Pagamento
{} // ela não pode ser instanciada, **só pode ser herdada**, ela seria herdada por exemplo para a classe de pagamento de cartão de crédito e boleto.
`````
Diferenças entre as classes abstratas e as Interfaces -> Interfaces definem o TEM QUE SER FEITO, não possui o COMO tem que FAZER -> já as classes abstratas tem uma implementação base que pode ser executada.