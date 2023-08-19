Objetos -> sempre um tipo de referência, composto por propriedades, metodos e eventos.
	Diferença maior entre class e struct é a forma em que eles são armazenados.
	objeto -> Tipo de referência -> os itens criados a partir das classes passam a apontar para o mesmo lugar na memória que as classes, então se o valor das classes é alterado, suas referências também são.
ainda podemos continuar utilizando structs, principalmente para criação de tipos.

-----------------------
**Encapsulamento**

Por exemplo a class de pagamento, o processo de pegar informações, ações, eventos do pagamento e trazer para dentro de uma classe -> é o conceito de Encapsulamento ( agrupar o que faz sentido estar junto ).
Dentro da classe de pagamento podemos ter o método de pagar() -> Variaveis de dentro das classes se tornam as propriedades desse objeto e as funções se tornam os métodos.

----------
Abstração ->
o ato de esconder os detalhes ( public, private ), voltando a classe pagamento, faz sentido termos a propriedade de vencimento publica para que todos possam ver ? sim, mas e o Método de consultar o saldo? não.

----------------
Herança ->

Suponhamos que você criou outra classe -> pagamentoBoleto, é um tipo de pagamento mas diferente da classe que usa o cartão de crédito, você criar tudo novamente? repetir código??? JAMAIS, usamos a herança, fazendo com que essa nova class obtenha as propriedades e métodos da outra classe, como? usando da seguinte maneira -> 
````
class PagamentoBoleto : Pagamento
{
    codigo...
}
````

desta maneira, estamos herdando todas as coisas de dentro de uma e passando para a outra ter acesso, assim reutilisamos o código.

---------------
Polimorfismo -> 
Basicamente você sobrescreve o método, ou seja, usando o exemplo de pagamento novamente, podemos modificar a ação de pagar para a classe de PagamentoBoleto -> usando o tag name "virtual" -> 
````
public virtual void pagar()
{

}
````

então quando formos chamar o método virtual em outra classe usando o "override" =>
````
public override void Pagar()
{
	base.Pagar();
}
````
Virtual no Pai e Override no Filho;
para acessar a chave do pai, temos que usar o "base."

-------
Modificadores de acesso ->
private, protect, internal e public;
private -> é visível apenas dentro da classe que é instanciada. -> se você não colocar nada nas classes, propriedades e etc, por default ela está privada.
protect -> ele é visível para o pai e seus filhos, mas para fora deles continua private;
internal -> ele fica disponível dentro do mesmo namespace. -> Quase não usamos muito no desenvolvimento WEB.

------
