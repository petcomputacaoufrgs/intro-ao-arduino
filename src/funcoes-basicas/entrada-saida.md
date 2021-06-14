# Funções de Entrada e Saída

## pinMode()
Na função `pinMode()` é feita a configuração de um pino digital como sendo de entrada (INPUT) ou saída (OUTPUT). Ela é normalmente utilizada dentro da função `setup()`. É de extrema importância que todos os pinos utilizados sejam configurados através dessa função.

Para o funcionamento correto da função, deve-se seguir a seguinte sintaxe: `pinMode(pino, modo)`.
Onde `pino` é o número do pino que deseja-se aplicar o `modo`, que pode ser `INPUT` ou `OUTPUT`.


## digitalRead()
A função `digitalRead()`  retorna o valor lido em um pino digital específico, que irá retornar `LOW` (quando não há corrente passando pelo pino) ou `HIGH` (quando há corrente passando pelo pino).

A sintaxe da função é dada por: `digitalRead(pino)`, onde o parâmetro `pino` é dado pelo número do pino que se deseja ler.


## digitalWrite()
Já na função `digitalWrite()` é possível escrever em um pino digital específico, ou seja, serve para definir a voltagem que o pino estará emitindo, 5V ou 3,3V para o valor de `HIGH` ou 0V para `LOW`.

A sintaxe da função é dada por `digitalWrite(pino, valor)`, onde `pino` é o número do pino que deseja-se inscrever o `valor` (`LOW` ou `HIGH`).
