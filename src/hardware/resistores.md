# Resistores

Um resistor eletrônico é um dispositivo elétrico capaz de limitar a corrente elétrica em um circuito e transformar energia elétrica em energia térmica (através do efeito joule). A resistência causa a queda de tensão em um circuito elétrico, porém jamais causa queda de corrente elétrica, apesar de limitá-la. Isso significa que a corrente elétrica que entra em um terminal do resistor será exatamente a mesma que sai pelo outro terminal, porém há uma queda de tensão, ou seja, uma diferença de potencial entre os terminais do resistor. Utilizando-se disso, é possível usar os resistores para controlar a corrente elétrica sobre os componentes desejados.

Como visto anteriormente, um LED possui limitação de corrente e tensão. Uma forma de controlar esses valores para evitar que o componente estrague é utilizar um resistor, para que os limites impostos pelo fabricante não sejam ultrapassados.

Qualquer objeto físico pode ser considerado um resistor: plástico, borracha, o corpo humano e até mesmo o vácuo possuem resistência mensuráveis. Essa resistência se dá pela divisão da diferença de potencial pela corrente elétrica, e é medido em ohms (Ω). Metais são materiais que possuem uma baixa resistência, por isso normalmente são utilizados em fios (como o cobre ou até mesmo ouro).
Os resistores utilizados em circuitos elétricos são pequenos componentes cilíndricos, geralmente possuem 4 faixas coloridas (existem os de 5 faixas, também chamados de resistores de precisão). Tais faixas são utilizadas para determinar o valor da resistência. As duas (ou três, no caso de resistores de precisão) primeiras faixas indicam quais os primeiros dígitos do valor da resistência. A próxima faixa corresponde ao fator de multiplicação. Por fim, a última faixa corresponde à porcentagem da tolerância do resistor e se encontra mais distanciada das outras.


Abaixo é possível encontrar uma tabela com as cores e seus valores correspondentes em cada faixa

|    Cor   | 1ª faixa | 2ª faixa | 3ª faixa (mult) | 4ª faixa (tol) |
|:--------:|:--------:|:--------:|:---------------:|:--------------:|
|   Preta  |     -    |     0    |      x 1 Ω      |        -       |
|  Marrom  |     1    |     1    |      x 10 Ω     |       1%       |
| Vermelha |     2    |     2    |     x 100 Ω     |       2%       |
|  Laranja |     3    |     3    |      x 1 KΩ     |       3%       |
|  Amarela |     4    |     4    |     x 10 KΩ     |       4%       |
|   Verde  |     5    |     5    |     x 100 KΩ    |       5%       |
|   Azul   |     6    |     6    |      x 1MΩ      |       25%      |
|  Violeta |     7    |     7    |     x 10 MΩ     |      0.1%      |
|   Cinza  |     8    |     8    |        -        |      0.05%     |
|  Branca  |     9    |     9    |        -        |        -       |
|   Prata  |     -    |     -    |      x 0,01     |       10%      |
|  Dourada |     -    |     -    |      x 0,1      |       5%       |

Tome como exemplo o resistor de quatro faixas abaixo. Suas duas primeiras faixas são amarela e cinza, respectivamente, de onde podemos tirar o número 48. Analisando a terceira faixa, de cor vermelha basta multiplicar o valor anteriormente obtido (48) por 100, obtendo assim 4800 Ω, com uma tolerância de 5% (última faixa dourada). Perceba que a última faixa está mais distanciada das demais, para poder diferenciá-la da primeira faixa.

![Resistor de 4800Ω,](./images/resistor.png)
