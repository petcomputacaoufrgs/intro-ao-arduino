# Funções de Tempo

Existem basicamente dois tipos de funções de tempo: um deles faz uma pausa e o outro retorna o tempo desde que a aplicação está rodando.


## delay() e delayMicrosseconds()
Na função `delay()`, é passado como parâmetro um valor de tempo em milissegundos e ao executar, o programa entrará em modo de espera pelo tempo especificado. Caso seja necessário uma maior precisão, pode-se usar a função `delayMicroseconds()` que como o nome sugere, executará uma pausa no programa de acordo com o valor em microssegundos que foi passado para o programa.

## millis() e micros()
Com a função `millis()` é possível obter o tempo em milissegundos que decorreu desde que a placa Arduino começou a rodar o programa. Também existe a versão em microsegundos, dada pela função `micros()`. 

Há uma diferença no formato do valor passado para as funções, enquanto as que operam sobre milissegundos utilizam no formato `unsigned long`, podendo variar de 0 a 4.294.967.295, enquanto as que opera sobre microssegundos utilizam-se de formatos em `unsigned int`, limitando sua capacidade de 0 a 65.535. Assim, a função  `micros()` pode armazenar um tempo de até aproximadamente 70 minutos enquanto a função  `millis()` armazena aproximadamente 50 dias. Ao atingir o valor máximo, acontece um _overflow_, fazendo com que o valor retorne a 0, recomeçando a contagem.

`1 segundo = 1.000 milissegundos = 1.000.000 microsegundos`