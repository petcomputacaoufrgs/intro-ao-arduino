# Buzzer

O buzzer, também conhecido como *piezo* é um componente que utiliza o efeito piezoelétrico, transformando energia elétrica em energia mecânica, e o som nada mais é do que propagação de ondas mecânicas em uma faixa de frequência entre aproximadamente 20Hz e 20KHz . 

Existem dois tipos de buzzer, o ativo e o passivo. O primeiro normalmente possui sua traseira lacrada e possui pinos de diferentes tamanhos, enquanto que no buzzer passivo a placa PCB está à mostra em sua traseira e ambos os pinos tem o mesmo tamanho. Ambos os tipos de buzzer, em sua frente, possuem um sinal de “__+__” indicando qual pino é o terminal positivo.

O buzzer ativo é o mais simples dentre eles, pois basta energizar ele já começa a apitar continuamente. Ele não depende de um circuito externo. Por esse motivo ele não é o mais indicado para criar melodias, mas sim para sinalizações - como alarmes. Sua utilização com o arduino acaba se tornando simples, visto que para ativá-lo basta utilizar a função `digitalWrite()`.

Já com o buzzer passivo, apenas energiza-lo não é o suficiente - ao fazer isso ele apenas emitirá um estalo e ruídos. Para o bom funcionamento dele é necessário utilizar algum circuito para emitir sinais, como se fosse um auto-falante - e isso trás mais precisão na frequência emitida, fazendo com que diversos sons e melodias possam ser gerados. Para se utilizar o buzzer passivo com o arduino, é necessário utilizar a função `tone(pino, frequência, duração)`, onde o parâmetro *pino* é a porta na qual o buzzer está conectado, *frequência* é a frequência do som gerado e o parâmetro *duração* é o tempo em que o buzzer permanecerá emitindo o som.
