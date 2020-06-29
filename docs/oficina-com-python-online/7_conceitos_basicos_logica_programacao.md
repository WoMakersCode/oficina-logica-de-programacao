Agora vamos aprender os conceitos básicos da lógica de programação o/

## **Variável**

Variáveis são espaços situados na memória do computador onde podemos guardar valores ou expressões. Ou seja, se quisermos que o computador memorize um número para que possamos usá-lo posteriormente em alguma operação, “guardamos” esse número na memória utilizando uma variável.

Para compreender melhor o que são variáveis, vamos fazer uma analogia com objetos do nosso cotidiano: vamos supor que temos um armário, no qual podemos guardar diversos objetos. E o nosso objetivo é guardar uma bola nesse armário.

![Guardar bola no armário](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image7.png)

Só que somos muito organizados em relação ao que guardamos no nosso armário.
Assim, antes de colocarmos um objeto no nosso armário, colocamos uma etiqueta na porta dizendo o **identificador** (o nome) desse objeto que está guardado naquela gaveta e de que **tipo** ele é.

No caso da bola, colocaremos o **identificador** BOLA e dizemos que a bola é do **tipo** Brinquedo.

![Variável 2](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image11.png)

Caso quiséssemos colocar um sapato no armário, poderíamos colocar uma etiqueta como:

![Variável 3](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image14.png)

E se quiséssemos guardar o número 2:

![Variável 4](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image10.png)

Nessa analogia, pode-se entender o armário como a memória do computador, onde podemos “guardar” valores para serem usados posteriormente, mas esses valores necessitam ser identificados por um nome e por um tipo.

> Em resumo:
* As variáveis são os espaços no armário
* As etiquetas são o identificador (ou nome) que usamos para nos referir a cada espaço vazio
* O tipo corresponde a que objetos (valores) podem ser colocados naquele espaço
* O valor corresponde ao que está guardado naquele espaço do armário

![Variável 5](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image6.png)

_Exemplos retirados dos slides do professor Clayton dos Santos: https://docs.google.com/presentation/d/1GXHp4Y3QpX3nbEcW5j5uRgJmqMYLlXbqyd3MVYRkewQ/edit_

Veja o exemplo abaixo para armazenar o número 10:

`inteiro numero = 10`

Nesse exemplo o **identificador** se chama numero, seu **valor** é o 10 e o seu **tipo** é inteiro.

## **Identificadores**

Toda vez que criamos uma variável precisamos dar um nome a ela. E dando um nome estamos identificando uma variável para usarmos novamente em outro momento.

Para nomear uma variável, na maioria das sintaxes do algoritmo precisamos estar atentos a algumas regras:

* O nome deve começar com uma letra;
* Os próximos caracteres do nome podem ser letras ou números;
* Não pode usar símbolos, exceto  _ (underline ou sublinhado). Exemplo: nota_aluno;
* Não pode ter espaços em branco;
* Não pode ter letras acentuadas;
* Não pode ser uma palavra reservada**;

> **São palavras que a linguagem de programação entende como um comando próprio
Exemplos: funcao, escreva, se, programa

## **Tipos de Dados**

### **Inteiro** 
Consiste dos números inteiros, positivos e negativos, e do resultado das operações de adição, subtração, multiplicação, divisão inteira e resto.

Exemplo: 

`inteiro idade = 21`

`inteiro numero_negativo = -23`

### **Real** 
Consiste dos números reais e do resultado das operações de adição, subtração, multiplicação, divisão. Na linguagem Portugol, os números reais são caracterizados por possuírem uma parte inteira e uma parte fracionária. Por exemplo, as partes inteira e fracionária do número real 3.141596 são 3 e 141596, respectivamente. Note que um “ponto” e não uma vírgula é usado para separar as partes inteira e fracionária.

> Como sabemos, os números reais incluem os números inteiros. No entanto, para evitar ambiguidades na escrita de algoritmos, assumimos que todo número escrito sem a parte fracionária é do tipo inteiro

Exemplo:

`real temperatura = 38`

`real saldo_bancario = -29.89`

### **Caractere** 
Consiste de um único símbolo, como uma letra do alfabeto, os dígitos numéricos positivos e negativos (0, 1, . . . , 9), entre muitos outros símbolos**. Os elementos do conjunto de valores do tipo caractere devem ser escritos, nos algoritmos do Portugol, entre aspas simples.

Exemplo:

`caracter ligado = 's'`

> Todos os demais símbolos podem ser consultados [nessa tabela](https://www.matematica.pt/util/resumos/tabela-ascii.php).

### **Cadeia** 
Consiste de uma concatenação** de símbolos (cadeia de caracteres). Os elementos do conjunto de valores do tipo cadeia devem ser escritos, nos algoritmos do Portugol, entre aspas duplas.


Exemplo:

`cadeia frase = "Esta e uma frase formada por caracteres”`

`cadeia vazia = ""` (*)


> **concatenação: é a operação de unir um ou mais elementos

> (*) Há um elemento especial, “”, que é denominado de palavra vazia, pois não possui nenhum símbolo.


### **Lógico** 
Inclui apenas os valores lógicos falso ou verdadeiro.

Exemplo:

`logico ligado = verdadeiro`

`logico esta_frio = falso`

## **Operadores Aritméticos**

Os operadores aritméticos são aqueles que permitem realizar as operações básicas da matemática.

### **Soma** 

Permite adicionar valores. Representado pelo símbolo +

Exemplo:

`inteiro valor1, valor2`

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 + valor2`

### **Subtração** 

Permite subtrair valores. É representado pelo símbolo -

Exemplo:

`inteiro valor1, valor2`

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 - valor2`

### **Multiplicação** 

Permite multiplicar valores. Representado pelo símbolo *

Exemplo:

`inteiro valor1, valor2`

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 * valor2`

### **Divisão** 

A divisão é compreendida por duas operações, a divisão e o resto. Ou seja, na programação, é possível obter o resultado dessas duas operações, tal como em um cálculo normal. Para realizar a divisão, utilizamos o símbolo / . Se a divisão envolve números inteiros, ele retornará o valor inteiro da divisão. Se for número real, ele retornará o valor da divisão com as casas decimais. Já para obter o resto (ou módulo), utilizamos o símbolo %. Lembrando que o resto sempre se dá em relação a uma divisão inteira.

Exemplo:

`inteiro valor1, valor2`

`valor1 = 2`

`valor2 = 5`

`divisao = valor2 / valor1`

`resto = valor2 % valor1`

**OBS.:** É necessário observar a prioridade dos operadores. Tal como na matemática tradicional, na programação são respeitadas as mesmas prioridades

Veja os exemplos:

`Exemplo 1: 3 + 7 * 2 => 3 + 14 => 17`

`Exemplo 2: (3 + 7) * 2 => 10 * 2 -> 20`

Ou seja, realizamos sempre o que se está entre parênteses por primeiro. Depois, as multiplicações e divisões. E por fim, as somas e subtrações. No caso de mais de uma operação do mesmo tipo, a prioridade é da esquerda para direita.

## **Operadores Lógicos**

São operadores que fornecem como resultado um valor lógico (verdadeiro ou falso).
Os operadores E e OU são operadores binários e o NAO é um operador unário.

![Operadores lógicos](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/operadores_logicos.png)

### E:
Operador que resulta VERDADEIRO somente se seus dois operandos lógicos forem verdadeiros.

### Ou:
Operador que resulta VERDADEIRO quando um dos seus operandos lógicos for verdadeiro.

### Nao:
Operador unário de negação.

> nao VERDADEIRO = FALSO

> nao FALSO = VERDADEIRO

Tem a maior precedência entre os operadores lógicos.

### Xou:
Operador que resulta VERDADEIRO se seus dois operandos lógicos forem diferentes, e FALSO se forem iguais.

## **Operadores Relacionais**
Tipo   | Descrição
--------- | ------
= | Igual
=/= | Diferente
\> | Maior
\>= | Maior ou igual
< | Menor
<= | Menor ou igual

## **Escrevendo o primeiro programa**

### Enunciado 
Vamos escrever um algoritmo que tem como objetivo receber um nome e exibir na tela `"Olá <Nome Digitado>!"`

Note que para escrever um programa precisaremos utilizar, além dos conceitos básicos de programação, alguns comandos específicos da linguagem Portugol. Esses comandos fazem parte da sintaxe** da linguagem e é importante entender como eles funcionam. Cada linguagem tem seus próprios comandos, com os conceitos básicos bem similares, mas escrito de modo diferente (sintaxe).

> **sintaxe: se refere a construção em si da linguagem, com os seus termos específicos para executar os comandos.

## **Desvios Condicionais**

Poderá ser necessário desviar a execução do programa, de acordo com uma ou mais condições.

> Por exemplo, ir à universidade de metrô ou de ônibus?

> Para testar as condições, podemos usar os operadores lógicos e relacionais.

### Desvio condicional simples

```
se (condição) {
    <instruções>
}
```

### Desvio condicional composto
```
se (condição) {
    <instruções>
senao
    <instruções>
}
```

Exemplo:

```
logico esta_chovendo = verdadeiro
se esta_chovendo {
   escreval("Levar guarda-chuva")
}
```

Exemplo:

```
programa
{ 
	funcao inicio ()
	{ 	
		inteiro menor, idade
		
		escreva("Informe sua idade: ")
		leia(idade)
	
		se (idade < 18) 
		{
			escreva("Você é menor de idade")
		} 
		senao
		{
			escreva("Você é maior de idade")
		}

		escreva("\n")
	} 
}
```

## **Programando uma calculadora**
Agora vamos praticar o que aprendemos para criar uma calculadora.
O programa pede ao usuário que informe dois números reais e a operação a ser executada entre estes números (soma, subtração, multiplicação ou divisão).
Por fim, será exibido o resultado da operação entre os dois números. 

```
programa
{
	funcao inicio()
	{
		caracter operador
		
		real resultado = 0.0, operando1, operando2

		escreva("Digite o primeiro número: ")
		leia(operando1)

		escreva("Digite o segundo número: ")
		leia(operando2)

		escreva("\n")
		
		escreva("Agora digite uma das operações ( + - * / ): ")
		leia(operador)

		/* Verifica qual foi a operação selecionada */
		
		se (operador == '+')
		{
			resultado = operando1 + operando2
		}
		senao  se(operador == '-')
		{
			resultado = operando1 - operando2
		}
		senao se(operador == '/')
		{
			resultado = operando1 / operando2
		}
		senao se(operador == '*')
		{
			resultado = operando1 * operando2
		}	

		limpa()
		
		escreva("Resultado:\n\n")
		escreva(operando1, " ", operador, " ", operando2, " = ", resultado)
		
		escreva("\n")
	}
}
```

> Podemos utilizar também o comando EscolheCaso para o programa da calculadora.

No momento de selecionar a operação, poderíamos fazer da seguinte forma:
```
escolha (operador)
	caso ('+')
	{
		resultado = operando1 + operando2	
	}
	caso('-')
	{
		resultado = operando1 - operando2
	}
	caso('/')
	{
		resultado = operando1 / operando2	
	}
	caso('*')
	{
		resultado = operando1 * operando2
	}	
```

## **Laços de Repetição**
Para repetir operações e não ser necessário fazer uma por uma, podemos utilizar estruturas chamadas de **laços de repetição**.

### Comando para (for)
Repete as instruções controlado por uma variável numérica que percorre os valores, entre dois limites, utilizando o passo definido.
Caso o passo não seja definido, o passo é de mais ou menos uma unidade de forma a poder percorrer o intervalo entre o valor inicial, e o final de forma crescente, ou decrescente.

```
programa
{
	funcao inicio()
	{
		inteiro numero, resultado, contador
		
		escreva("Informe um número para ver sua tabuada: ")
		leia(numero)

		limpa()
		
		para (contador = 1; contador <= 10; contador++) 
		{
			resultado = numero * contador 
			escreva (numero, " X ", contador, " = ", resultado , "\n")
		}
	}
}
```

### Comando enquanto (while)
Repete as instruções enquanto a condição for verdadeira

```
programa
{
	funcao inicio() 
	{
		inteiro contador = 1
		
		real numero, media, soma = 0.0

		// Laço que verifica se já foram informados 10 valores
		enquanto(contador <= 10) 
		{
			limpa()
			escreva("Digite o ", contador, "º número: ")
			leia(numero)

			// A variavel soma é o acumulador deste exemplo
			soma = soma + numero
			// Incrementa o contador
			contador = contador + 1 
		}
		media = soma / 10
		limpa()
		escreva("A média dos números é: ", media, "\n")
	}
}
```

> A estrutura de repetição **enquanto** permite que sejam feitos testes com mais de uma condição.

Veja o exemplo abaixo:


## **Função**
Função é um trecho de código que busca resolver um problema específico.

Exemplo: função para realizar o cálculo da média de duas notas.

> Vantagens: reutilização, redução de código duplicado, decomposição do problema em pequenas partes, entre outras.

A declaração da função no Portugol Studio é feita com a palavra reservada **funcao**, seguida do tipo de retorno. Quando não colocamos o tipo de retorno, o Portugol assume que é vazio.

```
programa
{
	funcao inicio()
	{
		// Chama o procedimento
		mensagem("Bem Vindo")

		// Chama a função no escreva
		escreva("O resultado do primeiro cálculo é: ", calcula (3.0, 4.0))	
		escreva("\nO resultado do segundo cálculo é: ", calcula (7.0, 2.0), "\n")
		mensagem("Tchau")
	}

	funcao mensagem (cadeia texto)
	{
		inteiro i
		// Insere uma linha antes do texto da mensagem		
		para(i = 0; i < 50; i++)
		{
		  escreva ("-")
		}

		// escreve a mensagem
		escreva ("\n", texto, "\n")
		// Insere uma linha após o texto da mensagem
		para(i = 0; i < 50; i++)
		{
		  escreva ("-")
		}
		escreva("\n")
	}

	// Função que realiza um cálculo e retorna o resultado
	funcao real calcula (real a, real b)
	{
		real resultado
		resultado = a * a + b * b
		retorne resultado
	}
}
```

## **Comentários**

Comentários são linhas que você pode escrever e quando o seu programa for executado a linguagem vai ignorar, não tratando como se fosse um comando a ser executado. 
Todas as linhas que começam com // no Portugol são comentários.

Exemplo:

```
// Este é um comentário
logico esta_chovendo = verdadeiro
se esta_chovendo {
   escreval("Levar guarda-chuva")
}
```