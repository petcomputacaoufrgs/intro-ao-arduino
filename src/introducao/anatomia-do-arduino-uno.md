# Anatomia do Arduino UNO

Nesta seção, serão apresentadas algumas partes básicas do arduino que serão referenciadas ao longo do curso. Caso não entenda algum termo aqui, não se preocupe, tudo será explicado detalhadamente nos próximos capítulos. 

 ![Anatomia da placa](./images/anatomia-placa.png)

+ **Botão de Reset:** este botão é muito útil para testar e debugar a placa. Quando pressionado, o código presente na placa será executado desde o ínicio. Especialmente útil para quando estamos tentando descobrir a origem de algum comportamento anormal no projeto. 

+ **Power LED:** Estará aceso enquanto a placa estiver em funcionamento.

+ **Portas Digitais:** O Arduino Uno possui 14 portas de entrada e saída digitais, sendo que 6 delas pode-se usar com a função PWM (pinos com um ‘~’ antes de sua numeração). Também há os pinos 0 e 1, que podem ser utilizados para comunicação serial com outros microcontroladores. Além disso, os pinos 2 e 3 podem ser configurados para gerar uma interrupção externa.

+ **LED (pino 13):** Existe um LED conectado ao pino digital de número 13. Ou seja, se o pino 13 estiver recebendo/emitindo um sinal positivo, o LED acenderá.

+ **Portas Analógicas:** O Arduino possui 6 portas analógicas com resolução de 10 bits. Estas portas são perfeitas para lidar com sensores.

+ **Entrada USB:** Utilizada tanto para alimentação da placa quanto para a comunicação com um computador (Utilizaremos ela para usar a IDE e fazer upload do nosso código para a placa).

+ **Alimentação DC:** Pode-se utilizar como alternativa ao USB, um conector Jack com a tensão entre 7V e 12V.
