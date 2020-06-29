# **O que é Dojo?**

Dojo é um local de treinamento de artes marciais. Se tratando de programação, é um local onde treinamos código de maneira colaborativa.

## **Como funciona na prática?**

Existem 3 papéis:

* **Piloto:** pessoa que ficará no teclado programando
* **Co-piloto:** pessoa que irá orientar quem está no comando
* **Público:** irá observar o que está sendo feito e auxiliar caso o piloto e o co-piloto tenha algum impedimento

**Informações importantes:**

* Cada pessoa fica 5min no computador
* Dojo não é uma competição, seguimos baby steps (pequenos passos para cumprir o objetivo)
* Utilizamos boas práticas e testes (no caso do portugol vamos fazer teste de mesa)

# **Mão na massa: Mega sena**

Escreva um programa que simule o sorteio da Megasena. No final, o seu programa deverá imprimir 6 números distintos separados por espaço. 

Exemplo de sorteio válido:

![Sorteio válido desafio megasena](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image9.png)

## **Dividir para conquistar**

Um dos conceitos bases utilizados na computação é dividir um problema em pequenas partes com o objetivo de facilitar a resolução do problema maior. Vamos seguir a mesma ideia no Dojo.

## **Parte 1: Escrevendo a estrutura base para o programa**

Todo programa precisa começar de alguma base. Algumas linguagens de programação são executadas a partir de um bloco de código conhecido como função principal. E isso não é diferente no Portugol. Vamos criar a nossa estrutura base para o algoritmo da Megasena.

1.1. Crie a função principal do seu programa

1.2. Escreva uma função que retorne um número inteiro entre 1 e 60 (números válidos para a Megasena)

> Dica: Existe uma biblioteca* chamada Util em portugol que possui uma função chamada sorteia onde os parâmetros são dois números inteiros que determinam o intervalo do sorteio. Para usá-la use o comando no início do seu programa: inclua biblioteca Util → apelido. O apelido é opcional, mas facilita quando o nome da biblioteca é grande. Assim, você não precisa ficar chamando a biblioteca pelo seu nome e sim pelo apelido

> *Uma biblioteca em programação é você utilizar um trecho de código já escrito por outro programador, assim você pode se concentrar apenas na tarefa que deve ser feita

1.3. Chame a função sorteio na função principal e exiba o número na tela para o usuário

## **Parte 2: Sorteando 6 números**

Quem acerta os 6 números na Megasena ganha o prêmio máximo, vamos simular o sorteio desses 6 números da sorte.

2.1.  Chame a função sorteio 6 vezes na função principal para simular um sorteio da Megasena

2.2. Salve o resultado do sorteio em alguma estrutura de dados

> Estrutura de dados é a uma maneira de armazenar um ou mais elementos no computador. Considere uma estrutura como uma coleção de dados

## **Parte 3: Tratando números repetidos**

No jogo da Megasena, o sorteio sempre considera números únicos, ou seja, sem repetição. Vamos tratar isso em nosso código.

3.1. Pense e implemente uma maneira de não salvar números repetidos na estrutura que você criou no passo 2.2

> Dica: Lembrem-se que a cada número sorteado você pode compará-los com os números anteriores

3.2. Exiba o resultado do sorteio na tela

## **Desafio extra**

No sorteio da Megasena, é comum que o resultado exibido seja sempre em ordem crescente dos números como na imagem abaixo:

![Sorteio megasena](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image2.png)

Vamos implementar isso em nosso programa.

## **Parte 4: Exibindo o sorteio em ordem crescente**

4.1. Ordene a estrutura com os números sorteados em ordem crescente. Para isso, o primeiro elemento `<` segundo elemento `< … <` último elemento.

Para conseguir fazer uma ordenação, existem vários algoritmos que podem ser utilizados. Aqui, como desafio, iremos fazer o algoritmo de ordenação chamado “Bubble Sort”. Seu funcionamento pode ser visto [nesse vídeo](https://www.youtube.com/watch?v=llX2SpDkQDc&t=4s).

> Dica 1: Lembre-se dos conceitos aprendidos sobre laços de repetição e condicionais. Se esses conceitos não ficaram claros PARE e volte na seção 7 (7. Conceitos Básicos da Lógica de Programação).Se necessário, consulte materiais extras sobre o assunto. Quando tiver compreendido seu funcionamento volte a fazer o desafio.

> Dica 2: Implemente uma função que faça a ordenação e receba como parâmetro a estrutura com os números sorteados feito no passo 3

4.2. Exiba o resultado para o usuário

## **[extra] Parte 5: Testando e exibir o resultado para o usuário**

5.1. Exiba o resultado final para o usuário

5.2. Validar que todos os cenários do algoritmo estão satisfeitos

> Dica: Usar teste de mesa - https://www.youtube.com/watch?v=Atcfaafvs4M. Às vezes utilizado como “Debug”* manual

> Debug é um termo apontado pela analista Grace Hopper que significa tentar encontrar e reduzir os defeitos. O termo surgiu na época em que os computadores ocupavam uma sala e realmente o que estava causando erro na máquina era um inseto (bug), daí o termo “debuggar”
