**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I*

# Ficha de Exercícios 3 - Estruturas de controlo

>
Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:

- O código apresentado deve ser bem indentado. 
- O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
- `gcc -Wall -Wextra -Wpedantic -Wvla -g exercicio1.c -o exercicio1`
- Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
- Evite o uso de constantes mágicas. 
- Evite duplicação de código. 
- Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.

---

1. Escreva um programa que declara um número real de dupla precisão e o inicializa com a seguinte expressão:
```C
double a = (0.3 * 3) - 0.9;
```
O programa em seguida testa se o número é zero. Execute o programa compilado. O que observa? 


2. [ciclos]	Implemente um programa que calcule o preço a pagar por uma pessoa pela entrada no ZOO de Lisboa, com base na sua idade.
O preço de cada bilhete deve ser calculado usando a seguinte tabela:

   | Idade | Preço |
   | ----- | ----- |
   | 0-16  |  10€  |
   | 17-64 |  17€  |
   | 65    |  10€  |


O utilizador pode comprar vários bilhetes e no final será mostrado o valor total dos bilhetes;

Segue-se um exemplo de uma sessão de uso do programa (à frente do símbolo > aparece o input do utilizador):

   ```bash
   Qual é a idade?
   > 40
   Quer comprar mais algum bilhete?
   > Não
   Preço a pagar: = 17
   ```

3. Implemente um programa que mostre um menu com 5 opções, cada uma etiquetada com uma letra. O programa deve então usar um switch para selecionar uma ação simples baseada na seleção do utilizador. O seu output deve ser semelhante ao seguinte:
   ```bash
   Por favor insira uma das seguintes opcoes: 
   p) piano
   v) violino 
   t) trompete
   c) contrabaixo
   s) sair
   > p
   O pianista toca piano!
   ```
Caso o utilizador introduza uma opção inválida, o programa deverá mostrar a mensagem ```Opcao invalida```.
Numa primeira versão, o programa termina depois de apresentar a resposta. Posteriormente, altere o programa de forma, a após o utilizador inserir uma opção,  seja mostrado novamente o menu. O menu deverá ter uma opção para a saída do programa;

   

4.	Um funcionário irá receber um aumento de acordo com o seu plano de trabalho, de acordo com a tabela abaixo: 

   | Plano | Aumento |
   | ----- | ------- |
   | A     |  10%    |
   | B     |  15%    |
   | C     |  20%    |

Faça um programa que leia o plano de trabalho e o salário atual de um funcionário e calcula e imprime o seu novo salário. Use o comando switch.

5.	[ciclos]	O menu de um snack-bar é o seguinte: 

   | Especificação | Código | Preço |
   | ------------- | ------ | ----- |
   | Cachorro quente |	100  |	1,20 |
   | Crepe simples |	101	| 1,30 |
   | Crepe com chocolate	| 102	| 1,50 |
   | Hambúrguer | 103 | 1,20 |
   | Cheeseburguer | 104 | 1,30 |
   | Refrigerante | 105 | 1,00 |

Implemente um programa que leia o código do item pedido, a quantidade e calcule o valor a ser pago por aquele lanche. Use o comando switch. O utilizador pode comprar vários itens e no final será mostrado o valor total dos itens.

6.	Escrever um programa que solicite um valor numérico correspondente a um mês do ano (1 a 12) e imprima o mês correspondente por extenso. O programa deve avisar se o valor não for válido.

7. [\*]	Escrever um programa que solicite dois números e o símbolo de operação aritmética (+ - * /). O programa deve imprimir o resultado da operação.

8.	Escreva um programa que verificará se o resto de uma divisão de um número digitado pelo utilizador por 5 é 0, 1, 2, 3 ou 4. Se o resto for zero, a seguinte mensagem será exibida: “A divisão é perfeita!”; Escreva também mensagens personalizadas para os valores 1, 2, 3 e 4.

9.	Faça um programa que leia os valores A, B, C e imprima no ecrã se a soma de A + B é menor que C.

10.	Faça um programa que recebe um número qualquer e informa no ecrã se é par ou ímpar.

11.	Faça um programa que encontre o dobro de um número caso ele seja positivo e o seu triplo caso seja negativo, imprimindo o resultado.

12.	Escreva um programa que leia três valores inteiros e diferentes e mostre-os em ordem decrescente.

13.	O IMC – Índice de Massa Corporal é um critério da Organização Mundial de Saúde para dar uma indicação sobre a condição de peso de uma pessoa adulta. A fórmula é

IMC = peso / ( altura )²

Elabore um programa que leia o peso e a altura de um adulto e mostre sua condição de acordo com a tabela abaixo. 

   | **IMC em adultos** | **Condição** |
   | -------------- | -------- |
   | i.	Abaixo de 18,5 | Abaixo do peso | 
   | ii.	Entre 18,5 e 25 | Peso normal |
   | iii.	Entre 25 e 30 | Acima do peso | 
   | iv.	Acima de 30 | obeso |

14. [ciclos] Elabore um programa que apresente o total da soma obtida dos cem primeiros números inteiros.

15. [ciclos] Elabore um programa que efetue a leitura sucessiva de valores numéricos e apresente no final o total do somatório, a média e o total de valores lidos. O programa deve fazer as leituras dos valores enquanto o utilizador estiver a fornecer valores positivos. Ou seja, o programa deve parar quando o utilizador fornecer um valor negativo

16. [ciclos] Elabore um programa que solicite a idade de várias pessoas e imprima: 
   - Total de pessoas com menos de 21 anos. 
   - Total de pessoas com mais de 50 anos. 
   - O programa termina quando idade for =-99.

17. [ciclos] Elabore um programa que solicita um número <n> do tipo unsigned int e em seguida escreve a sequência do jogo buzz. Nesta sequência os números acabados em 7 ou multiplos de 7, ou números com dígitos iguais 11, 22, 33, 333, 55555, 77777 etc,  são substituidos pela palavra buzz enquanto que os restantes números são mostrados na consola. Um número por linha.


