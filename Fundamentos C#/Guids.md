Identificador global único, sempre que executamos o Guid, ele nos devolve um identificador diferente, ele devolve um id com 32 caracteres, podemos diminuir transformando ele em string com o Tostring() e depois com o Substring(0, 8) -> pegando apenas os primeiros 8 caracteres

Interpolação de Strings -> juntar uma string com outros valores
exemplo -> 
````
var price = 10.2
var text = "O preço do produto é : " + price;
// de uma forma melhor ->
var text = $"O preço do produto é : {price}"
````

string.Format -> como o nome diz, ele formata o valor de dentro do texto que fica especificado no fim do parâmetro 

Comparação de textos -> CompareTo() -> se comparada com um texto igual, retornará 0 e 1 caso não;  Contains -> serve para comparar com um texto completamente igual ou pedaço de um, ele pode por exemplo buscar palavras em textos e retorna true ou false;
AMBAS SÃO CASESENSITIVE -> mas caso queiramos que não seja é só colocarmos no segundo parâmetro o "stringComparasion.OrdinalIgnoreCase"

StartsWith && EndsWith -> começa com e termina com, basicamente serve para compararmos se o texto x começa com tal coisa ou se y termina com x coisa, ambos retornam true e false. AMBAS SÃO CASESENSITIVE

Equals -> (CASESENSITIVE), ele compara para dizer se um é igual ao outro mas apenas para objetos iguais aos que estão sendo comparados, ou seja, não compara string com numbers por exemplo.

Indices -> É o índice de um array( posição do array ) 
IndexOf() -> ela basicamente recebe o que você coloca e procura onde foi chamada, ela é um método que pode ser chamada em listas, e só vai buscar se o que for recebido seja igual a lista que está chamando ela.
LastIndexOf() -> ele procura o que foi passado e retorna o último achado.