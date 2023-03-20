**UNIVERSIDADE LUSÓFONA DE HUMANIDADES E TECNOLOGIAS**

*Linguagens de Programação I*

# Ficha de Exercícios 3 - Estruturas de controlo

> Na resolução destes exercícios deve ser utilizada a Linguagem de Programação C. Para além da correta implementação dos requisitos, tenha em conta os seguintes aspetos:
>* O código apresentado deve ser bem indentado. 
>* O código deve compilar sem erros ou *warnings* utilizando o *gcc* com as seguintes flags:
>* `-Wall -Wextra -Wpedantic -Wvla -g`
>* Tenha em atenção os nomes dados das variáveis, para que sejam indicadores daquilo que as mesmas vão conter.
>* Evite o uso de constantes mágicas. 
>* Evite duplicação de código. 
>* Considere a implementação de funções para melhorar a legibilidade, evitar a duplicação e criar soluções mais genéricas.


## Controlo de fluxo: if, else, switch, operador ternário

1. Escreva um programa que lê um número inteiro e uma letra. Consoante a letra lida, apresenta o número em base Decimal, octal ou hexadecimal:
- `'D'`, `'d'` ou `'i'`: decimal
- `'O'`, `'o'` ou `'0'`: octal
- `'x'`, `'h'`: hexadecimal com dígitos hexadecimais em letra minúscula
- `'X'`, `'H'`: hexadecimal com dígitos hexadecimais em letra maiúscula
Utilize a clausula `switch` para resolver o problema.


2. Escreva um programa que lê três números e apresenta o valor máximo e o valor mínimo. Utilize o operador ternário para encontrar o máximo e o mínimo.


3. Escreva um programa que lê as jogadas de dois jogadores de Papel (P), Pedra (R) ou Tesoura (S) e determina qual o vencedor. Exemplo:

```
Jogador 1 - Introduza a jogada:
>R
Jogador 2 - Introduza a jogada:
>P
Vencedor: Jogador 2
```

4.	Escrever um programa que solicite um valor numérico correspondente a um mês do ano (1 a 12) e imprima o mês correspondente por extenso. O programa deve avisar se o valor não for válido.

5.	Escreva um programa que verificará se o resto de uma divisão de um número digitado pelo utilizador por 5 é 0, 1, 2, 3 ou 4. Se o resto for zero, a seguinte mensagem será exibida: “A divisão é perfeita!”; Escreva também mensagens personalizadas para os valores 1, 2, 3 e 4.

## Estruturas de controlo (ciclos): while, do while, for

1.	O menu de um snack-bar é o seguinte: 
```
   | Especificação | Código | Preço |
   | ------------- | ------ | ----- |
   | Cachorro quente |	100  |	1,20 |
   | Crepe simples |	101	| 1,30 |
   | Crepe com chocolate	| 102	| 1,50 |
   | Hambúrguer | 103 | 1,20 |
   | Cheeseburguer | 104 | 1,30 |
   | Refrigerante | 105 | 1,00 |
```
Implemente um programa que leia o código do item pedido, a quantidade e calcule o valor a ser pago por aquele lanche. Use o comando switch. O utilizador pode comprar vários itens e no final será mostrado o valor total dos itens.

2. Elabore um programa que efetue a leitura sucessiva de valores numéricos e apresente no final o total do somatório, a média e o total de valores lidos. O programa deve fazer as leituras dos valores enquanto o utilizador estiver a fornecer valores positivos. Ou seja, o programa deve parar quando o utilizador fornecer um valor negativo

3. Elabore um programa que solicite a idade de várias pessoas e imprima: 
   - Total de pessoas com menos de 21 anos. 
   - Total de pessoas com mais de 50 anos. 
   - O programa termina quando idade for =-99.

4. Elabore um programa que solicita um número <n> do tipo unsigned int e em seguida escreve a sequência do jogo buzz. Nesta sequência os números acabados em 7 ou multiplos de 7, ou números com dígitos iguais 11, 22, 33, 333, 55555, 77777 etc,  são substituidos pela palavra buzz enquanto que os restantes números são mostrados na consola. Um número por linha.

5. Considere a seguinte função que detecta se um número é primo.
```
int is_prime(unsigned x)
{
   unsigned i;

   if (x <= 1)
      return 0;
                
   for (i = 2 ; i < x ; i++)
      if (x % i == 0)
         return 0;

   return 1;
}
```
   5.1. Faça um programa que leia um número do utilizador e utilize a função `is_prime()` para verificar se o número é primo.
                     
   5.2. Re-escreva a função `is_prime()` de forma a utilizar um ciclo `while`
                     
   5.3. Re-escreva a função `is_prime()` de forma a utilizar um ciclo `do while`
   
> De notar que, neste exercício, a condição do ciclo poderia ser alterada de forma a aumentar bastante a performance do algoritmo. Poderiamos testar apenas os números até a raiz quadrada de `x`, porque quaisquer fatores de `x` que sejam maiores que a raiz quadrada de `x` teriam necessariamente um fator correspondente que é menor que a raiz quadrada de `x`. Por exemplo, suponha que desejamos testar se `x = 49` é primo. Se iterarmos de 2 até `x-1`, verificaríamos os divisores 2, 3, 4, 5, 6, 7 e 8. No entanto, podemos parar na raiz quadrada de `x`, que é 7, porque quaisquer fatores de `x` que sejam maiores que 7 teriam necessariamente um fator correspondente que é menor que 7. Neste caso, já teríamos verificado 7 e saberíamos que 49 não é primo.
> A condição poderia ser então alterada para: `i <= sqrt(x)` ou seja `i * i <= x`.



