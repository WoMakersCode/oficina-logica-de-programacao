# **Desafio 1. Mega sena**

Escreva um programa que simule o sorteio da Megasena. No final, o seu programa deverá imprimir 6 números distintos 
separados por espaço. 

Exemplo de sorteio válido:

`23 41 46 52 54 59`

## **Dividir para conquistar**

Um dos conceitos bases utilizados na computação é dividir um problema em pequenas partes com o objetivo de facilitar a 
resolução do problema maior. 

## **Parte 1: Escrevendo a estrutura base para o programa**

1.1 Escreva uma função que retorne um número inteiro entre 1 e 60 (números válidos para a Megasena)

> Dica: Existe uma biblioteca* chamada `random` com uma função `randint` em Python que possui uma função chamada sorteia 
> onde os parâmetros são dois números inteiros que determinam o intervalo do sorteio. 

> *Uma biblioteca em programação é você utilizar um trecho de código já escrito por outro programador, 
> assim você pode se concentrar apenas na tarefa que deve ser feita

1.2. Chame a função sorteio e exiba o número na tela para o usuário

## **Parte 2: Sorteando 6 números**

Quem acerta os 6 números na Megasena ganha o prêmio máximo, vamos simular o sorteio desses 6 números da sorte.

2.1.  Chame a função sorteio 6 vezes para simular um sorteio da Megasena

2.2. Salve o resultado do sorteio em alguma estrutura de dados

> Estrutura de dados é a uma maneira de armazenar um ou mais elementos no computador. 
> Considere uma estrutura como uma coleção de dados

## **Parte 3: Tratando números repetidos**

No jogo da Megasena, o sorteio sempre considera números únicos, ou seja, sem repetição. Vamos tratar isso em nosso código.

3.1. Pense e implemente uma maneira de não salvar números repetidos na estrutura que você criou no passo 2.2

> Dica: Lembrem-se que a cada número sorteado você pode compará-los com os números anteriores

3.2. Exiba o resultado do sorteio na tela

No sorteio da Megasena, é comum que o resultado exibido seja sempre em ordem crescente dos números como na imagem abaixo:

![Sorteio megasena](https://github.com/WoMakersCode/oficina-logica-de-programacao/blob/master/images/image2.png)

Vamos implementar isso em nosso programa.

## **Parte 4: Exibindo o sorteio em ordem crescente**

4.1. Ordene a estrutura com os números sorteados em ordem crescente. 
Para isso, o primeiro elemento `<` segundo elemento `< … <` último elemento.

> **Dica:** Veja se existe algum recurso disponível na linguagem que faça a ordenação

4.2. Exiba o resultado para o usuário

## **[extra] Parte 5: Testando e exibir o resultado para o usuário**

5.1. Validar que todos os cenários do algoritmo estão satisfeitos

> Dica: Usar teste de mesa - https://www.youtube.com/watch?v=Atcfaafvs4M. Às vezes utilizado como “Debug”* manual

> Debug é um termo apontado pela analista Grace Hopper que significa tentar encontrar e reduzir os defeitos. 
> O termo surgiu na época em que os computadores ocupavam uma sala e realmente o que estava causando erro na máquina 
> era um inseto (bug), daí o termo “debuggar”
