Tipos complexos ->
vamos utilizar do exemplo da nota sobre POO, usando o método de pagamento ->
Todas as classes que criamos são os tipos complexos.

-----
Propriedades ->
prop -> propriedade com get e set -> acessores, podemos atribuir ou receber valores.
````
private DateTime _DataPagamento { get; set }
````
propFull -> interagir com o método no momento que ele está sendo criado.

------
Métodos -> Posso definir alguma informação a ser recebida em um função com o seguinte formato de sintax -> 
````
Public void Pagar(number Numero, string Nome, bool pagarAposVencimento = false){}
//  com o "= false", nós podemos ler isso como um não obrigatório para a função;
`````

Sobrecargas de métodos -> nomes iguais, mas assinaturas diferentes, por exemplo -> 
````
public void pagar() {}
public void pagar(string Name) {}
// chamando a mesma função duas vezes mas com assinaturas diferentes.
}
`````
podemos ter varias dessas versões que precisamos do mesmo método mas com assinaturas diferentes.

Sobrescrita de método -> usando o virtual, nós podemos mudar como a função se comporta ( ler mais em POO ).

Método construtor -> "cpor" -> 
````
public class Pagamento() : OutraFuncao
{
	public Pagamento() 
	{
		// é um método que é executado sempre que o objeto é iniciado.
		// eles não retornam nada, msa podem receber valores através dos paramêtros.
		// receba um paramêtro que só pode ser acessado no pai, usando a assim ->
	}
	assim ->
	public Pagamento() : base(OutraFuncao)
}
`````

