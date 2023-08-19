Array é um vector, mas no C# a sintex dele muda um teco -> 
````
static void Main(string[] args)
{
	var myArray = new int[]; -> e ele precisa ter um tamanho -> new int[5];
	int myArray = new int[5]
}
````
se ele possui 5 indicies/posições -> ele possui 4 elementos dentro dele ( arrays começam sempre por 0 ).
Podemos atribuir valor as posições dos arrays como faziamos nos objetos do JS ->
myArray[0] = 12; -> primeiro valor do array  terá o valor de 12.
Se quisermos definir na hora da criação do array ->
````
var myArray = new int[5] { 1, 2, 3, 4, 5};
````
