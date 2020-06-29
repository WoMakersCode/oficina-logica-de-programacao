# Conceitos básicos de lógica de programação

Agora vamos aprender os conceitos básicos da lógica de programação o/

## **Variável**

Variáveis são espaços situados na memória do computador onde podemos guardar valores ou expressões, ou seja, 
se quisermos que o computador memorize um número para que possamos usá-lo posteriormente em alguma operação, 
“guardamos” esse número na memória utilizando uma variável.

Para compreender melhor o que são variáveis, vamos fazer uma analogia com objetos do nosso cotidiano: 
vamos supor que temos um armário, no qual podemos guardar diversos objetos. E o nosso objetivo é guardar 
uma bola nesse armário.

![Guardar bola no armário](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image7.png)

Só que somos muito organizados em relação ao que guardamos no nosso armário.
Assim, antes de colocarmos um objeto no nosso armário, colocamos uma etiqueta na porta dizendo o 
**identificador** (o nome) desse objeto que está guardado naquela gaveta e de que **tipo** ele é.

No caso da bola, colocaremos o **identificador** BOLA e dizemos que a bola é do **tipo** Brinquedo.

![Variável 2](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image11.png)

Caso quiséssemos colocar um sapato no armário, poderíamos colocar uma etiqueta como:

![Variável 3](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image14.png)

E se quiséssemos guardar o número 2:

![Variável 4](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image10.png)

Nessa analogia, pode-se entender o armário como a memória do computador, onde podemos “guardar” 
valores para serem usados posteriormente, mas esses valores necessitam ser identificados por um nome e por um tipo.

> Em resumo:
* As variáveis são os espaços no armário
* As etiquetas são o identificador (ou nome) que usamos para nos referir a cada espaço vazio
* O tipo corresponde a que objetos (valores) podem ser colocados naquele espaço
* O valor corresponde ao que está guardado naquele espaço do armário

![Variável 5](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image6.png)

[Exemplos retirados dos slides do professor Clayton dos Santos](https://docs.google.com/presentation/d/1GXHp4Y3QpX3nbEcW5j5uRgJmqMYLlXbqyd3MVYRkewQ/edit_)

Veja o exemplo abaixo para armazenar o número 10:

`numero = 10`

Nesse exemplo o **identificador** se chama numero, seu **valor** é o 10 e o seu **tipo** é inteiro*.

> ***Nota:** Em Python não é necessário especificar o tipo de dado para declarar as variáveis, mas em algumas linguagens 
> isso é necessário. O Python tem uma tipagem dinâmica e depende somente do seu conteúdo armazenado.  Pelo fato da 
> variável `numero` estar armazenando o inteiro 10, o Python já tipa dinamicamente essa variável para inteiro.

## **Identificadores**

Toda vez que criamos uma variável precisamos dar um nome a ela. E dando um nome estamos identificando uma variável 
para usarmos novamente em outro momento.

Para nomear uma variável, na maioria das sintaxes do algoritmo precisamos estar atentos a algumas regras:

* O nome deve começar com uma letra;
* Os próximos caracteres do nome podem ser letras ou números;
* Não pode usar símbolos, exceto  _ (underline ou sublinhado). Exemplo: nota_aluno;
* Não pode ter espaços em branco;
* Não pode ter letras acentuadas;
* Não pode ser uma palavra reservada**;

> **São palavras que a linguagem de programação entende como um comando próprio
Exemplos: print, def, if, while

## **Tipos de Dados**

### **Inteiro** 
Consiste dos números inteiros, positivos e negativos, e do resultado das operações de adição, subtração, 
multiplicação, divisão inteira e resto.

Exemplo: 

`idade = 21`

`numero_negativo = -23`

Para verificar o tipo dessa variável vamos usar a função type e exibir o resultado com o comando print conforme abaixo:

`print(type(idade))`

O retorno será um tipo inteiro, que em Python chamamos de int: `<class 'int'>`

### **Real** 
Consiste dos números reais e do resultado das operações de adição, subtração, multiplicação, divisão. 
Na linguagem Portugol, os números reais são caracterizados por possuírem uma parte inteira e uma parte fracionária. 
Por exemplo, as partes inteira e fracionária do número real 3.141596 são 3 e 141596, respectivamente. 
 que um “ponto” e não uma vírgula é usado para separar as partes inteira e fracionária.

> Como sabemos, os números reais incluem os números inteiros. No entanto, para evitar ambiguidades na escrita 
> de algoritmos, assumimos que todo número escrito sem a parte fracionária é do tipo inteiro

Exemplo:

`temperatura = 38.5`

`saldo_bancario = -29.89`

Se usarmos a mesma função `type` que vimos anteriormente, veremos que o retorno será um tipo real ou decimal, que em 
Python chamamos de float: `<class 'float'>`

### **Texto** 
Consiste de um único símbolo, como uma letra do alfabeto, os dígitos numéricos positivos e negativos (0, 1, . . . , 9), 
entre muitos outros símbolos* ou o conjunto (concatenação**) desses símbolos. Para representá-los usamos aspas simples 
ou duplas.

> ** Todos os demais símbolos podem ser consultados [nessa tabela](https://www.matematica.pt/util/resumos/tabela-ascii.php).

> **Concatenação é a operação de unir um ou mais elementos


Exemplo:

`ligado = 's'`

`frase = "Esta e uma frase formada por caracteres”`

`string_vazia = ""` (*)


> (*) Há um elemento especial, “”, que é denominado de palavra vazia, pois não possui nenhum símbolo.


### **Lógico** 
Inclui apenas os valores lógicos falso (em inglês `false`) ou verdadeiro (em inglês `true`).

Exemplo:

`ligado = True`

`esta_frio = False`

## **Operadores Aritméticos**

Os operadores aritméticos são aqueles que permitem realizar as operações básicas da matemática.

### **Soma** 

Permite adicionar valores. Representado pelo símbolo +

Exemplo:

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 + valor2`

### **Subtração** 

Permite subtrair valores. É representado pelo símbolo -

Exemplo:

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 - valor2`

### **Multiplicação** 

Permite multiplicar valores. Representado pelo símbolo *

Exemplo:

`valor1 = 2`

`valor2 = 5`

`resultado = valor1 * valor2`

### **Divisão** 

A divisão é compreendida por duas operações, a divisão e o resto. Ou seja, na programação, é possível obter o resultado 
dessas duas operações, tal como em um cálculo normal. Para realizar a divisão, utilizamos o símbolo / . 
Se a divisão envolve números inteiros, ele retornará o valor inteiro da divisão. Se for número real, 
ele retornará o valor da divisão com as casas decimais. Já para obter o resto (ou módulo), utilizamos o símbolo %. 
Lembrando que o resto sempre se dá em relação a uma divisão inteira.

Exemplo:

`valor1 = 2`

`valor2 = 5`

`divisao = valor2 / valor1`

`resto = valor2 % valor1`

**OBS.:** É necessário observar a prioridade dos operadores. Tal como na matemática tradicional, na programação são respeitadas as mesmas prioridades

Veja os exemplos:

`Exemplo 1: 3 + 7 * 2 => 3 + 14 => 17`

`Exemplo 2: (3 + 7) * 2 => 10 * 2 -> 20`

Ou seja, realizamos sempre o que se está entre parênteses por primeiro. Depois, as multiplicações e divisões. 
E por fim, as somas e subtrações. No caso de mais de uma operação do mesmo tipo, a prioridade é da esquerda para 
direita.

## **Operadores Lógicos**

São operadores que fornecem como resultado um valor lógico (verdadeiro ou falso).
Os operadores E (em inglês `and`) e OU (em inglês `or`) são operadores binários e o NAO (em inglês `not`) é um operador 
unário.

![Operadores lógicos](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/operadores_logicos.png)

### E (and):
Operador que resulta VERDADEIRO somente se seus dois operandos lógicos forem verdadeiros.

`10 < 20 and 20 > 30`

### Ou (or):
Operador que resulta VERDADEIRO quando um dos seus operandos lógicos for verdadeiro.

`10 < 20 or 20 > 30`

### Nao (not):
Operador unário de negação.

`not True`: resultado `False`
`not False`: resultado `True`

Tem a maior precedência entre os operadores lógicos.

### Xou (xor):
Operador que resulta VERDADEIRO se seus dois operandos lógicos forem diferentes, e FALSO se forem iguais.
Também chamado de `ou exclusivo`.

`1 ^ 1`: resultado `0` (Falso)
`0 ^ 1`: resultado `1` (Verdadeiro) 

## **Operadores Relacionais**

São utilizados para comparar valores. Normalmente utilizamos em um bloco condicional

Tipo   | Descrição
--------- | ------
== | Igual
!= | Diferente
\> | Maior
\>= | Maior ou igual
< | Menor
<= | Menor ou igual

> **Nota:** Quando vimos na seção de variáveis vimos que para declarar uma variável bastaria escrever seu identificador
> (nome), colocar o símbolo de atribuição (=) e logo depois o seu valor (conteúdo). Repare que esse símbolo (=) é 
> diferente do símbolo de igual do operador relacional. Em resumo: == (igualdade) e = (atribuição)

## **Escrevendo o primeiro programa**

### Enunciado 
Vamos escrever um algoritmo que tem como objetivo receber um nome e exibir na tela `"Olá <Nome Digitado>!"`

Note que para escrever um programa precisaremos utilizar, além dos conceitos básicos de programação, 
alguns comandos específicos da linguagem Python. Esses comandos fazem parte da sintaxe** da linguagem e é 
importante entender como eles funcionam. Cada linguagem tem seus próprios comandos, com os conceitos básicos bem 
similares, mas escrito de modo diferente (sintaxe).

> **Sintaxe: se refere a construção em si da linguagem, com os seus termos específicos para executar os comandos.

Em Python, para pegar uma informação digitada pelo usuário usamos a função `input()`

## **Desvios Condicionais**

Poderá ser necessário desviar a execução do programa, de acordo com uma ou mais condições.

> Por exemplo, ir à universidade de metrô ou de ônibus?

> Para testar as condições, podemos usar os operadores lógicos e relacionais.

### Desvio condicional simples

```
if condição:
    <instruções>
```

### Desvio condicional composto
```
if condicao:
    <instruções>
else:
    <instruções>
```

> **Nota:** Repare que depois do sinal de dois pontos (:) precisamos dar uma tabulação (espaço) pois em Python 
> trabalharemos com o conceito de blocos através da identação. Nesse caso específico estamos criando um bloco condicional.

Exemplo:

```python
esta_chovendo = True
if esta_chovendo:
   print("Levar guarda-chuva")
```

Exemplo:

Vamos perguntar para o usuário informar sua idade e o nosso programa irá informar se ele é maior ou menor de idade.
Para pedir para o usuário informar um valor, novamente iremos usar a função `input`

```python
idade = int(input("Informe sua idade: "))

if idade < 18: 
    print("Você é menor de idade")
else:
    print("Você é maior de idade")
```

> **Nota:** Você deve estar se perguntando por que precisamos usar esse `int` ao redor da nossa função `input`.
> Dica: experimente ver qual é o valor que está sendo armazenado na variável `idade` se não estivéssemos usando a
> função `int`. Veja como o restante do código irá se comportar.  

### Desvio condicional composto com condição

Aqui conseguimos validar uma primeira condição (em inglês `if`), se ela for falsa, validamos uma 
segunda condição (`elif`, abreviação de `else` + `if`) e assim por diante. No final, podemos colocar 
um senão (em inglês `else`) que significa que se nenhuma das condições anteriores forem satisfeitas, essa
instrução será executada.

```
if condicao:
    <instruções>
elif condicao_2:
    <instruções>
else:
    <instruções>
```

Exemplo:

Vamos perguntar para o usuário informar sua idade e nosso programa irá dizer a se o usuário é criança, adolescente, 
adulto ou idoso

```python
idade = int(input("Informe sua idade: "))

if idade < 13: 
    print("Você é criança")
elif idade >= 13 and idade < 18:
    print("Você é adolescente")
elif idade >= 18 and idade < 60:
    print("Você é adulto")
else:
    print("Você é idoso")
```

## **Programando uma calculadora**
Agora vamos praticar o que aprendemos para criar uma calculadora.
O programa pede ao usuário que informe dois números reais e a operação a ser executada entre estes números (soma, 
subtração, multiplicação ou divisão).
Por fim, será exibido o resultado da operação entre os dois números. 

```python
operando_1 = int(input("Digite o primeiro número: "))
operando_2 = int(input("Digite o segundo número: "))

operador = input("Agora digite uma das operações ( + - * / ): ")
resultado = None

# Verifica qual foi a operação selecionada

if operador == "+":
    resultado = operando_1 + operando_2
elif operador == "-":
    resultado = operando_1 - operando_2
elif operador == "*":
    resultado = operando_1 * operando_2
elif operador == "/":
    resultado = operando_1 / operando_2
else:
    print("Operador inválido")

print("\nResultado:")
print(operando_1, " ", operador, " ", operando_2, " = ", resultado)
```

> **Nota 1:** `None` é um valor que significa vazio. Na variável `resultado`, no primeiro momento, 
> estamos usando um tipo vazio: `<class 'NoneType'>`

> **Nota 2:** Usamos o `\n` para pular uma linha


## **Laços de Repetição**
Para repetir operações e não ser necessário fazer uma por uma, podemos utilizar estruturas chamadas de **laços de repetição**.

### Comando para (for)
Repete as instruções controlado por uma variável numérica que percorre os valores, entre dois limites, utilizando o 
passo definido.
Caso o passo não seja definido, o passo é de mais ou menos uma unidade de forma a poder percorrer o intervalo entre o
valor inicial, e o final de forma crescente, ou decrescente.

Exemplo:

```python
numero = int(input("Informe um número para ver sua tabuada: "))

for contador in range(1, 11): 
    resultado = numero * contador 
    print (numero, " X ", contador, " = ", resultado , "\n")

```

> **Nota:** A função `range` no Python gera uma sequência de números iniciando do primeiro valor passado até o último 
> (exclusivo), ou seja, aqui estamos trabalhando com o intervalo fechado em 1 e aberto em 11: [1, 11)

### Comando enquanto (while)
Repete as instruções enquanto a condição for verdadeira

Exemplo: Dado 5 números informados pelo usuário, vamos exibir sua média

```python
contador = 1
soma = 0

# Laço que verifica se já foram informados 5 valores
while contador <= 5:
    numero = int(input(f"Digite o {contador}º número: "))

    # A variavel soma é o acumulador deste exemplo
    soma = soma + numero
    # Incrementa o contador
    contador = contador + 1
media = soma / 5
print("A média dos números é: ", media, "\n")

```

> A estrutura de repetição **enquanto (while)** permite que sejam feitos testes com mais de uma condição.

Veja o exemplo abaixo:


## **Função**
Função é um trecho de código que busca resolver um problema específico.

Exemplo: função para realizar o cálculo da média de duas notas.

> Vantagens: reutilização, redução de código duplicado, decomposição do problema em pequenas partes, entre outras.

A declaração da função em Python é feita com a palavra reservada **def**, seguida do nome da função, parênteses para
conter os argumentos e por fim os dois pontos para indicar o bloco com o conteúdo da função.  

```python
def minha_funcao():
    pass
```

Exemplo:

Vamos fazer uma função que calcula a média e outra função que exibe um texto na tela formatado.
No final, vamos chamar as funções para exibir o resultado.

```python
def mensagem(texto):
    # Insere uma linha antes do texto da mensagem
    for i in range(50):
      print ("-", end='')

    # Escreve a mensagem
    print("\n", texto)

    # Insere uma linha após o texto da mensagem
    for i in range(50):
      print("-", end='')

def calcula_media(a, b):
    """

    :param a:
    :param b:
    :return: Função que calcula
    """
    resultado = (a+b)/2
    return resultado


print("O resultado do primeiro cálculo é: ", calcula_media(12, 6))
print("O resultado do segundo cálculo é: ", calcula_media(10, 20), "\n")
mensagem("Fim da excução")
```

## **Comentários**

Comentários são linhas que você pode escrever e quando o seu programa for executado a linguagem vai ignorar, não 
tratando como se fosse um comando a ser executado. 
Todas as linhas que começam com # em Python são comentários.

Exemplo:

```python
# Este é um comentário
esta_chovendo = True
if esta_chovendo:
   print("Levar guarda-chuva")
```