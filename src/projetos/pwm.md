# PWM - Controlando intensidade do LED

A sigla PWM vem do inglês Pulse Width Modulation, e é uma técnica para obter resultados analógicos utilizando sinais digitais. Ondas quadradas são geradas, mudando o nível lógico de *alto* para *baixo*, e o tempo relativo em que a onda passa em cada um desses estados acaba simulando voltagens entre 0V e 5V.

Na prática funciona da seguinte maneira: se a onda tiver uma largura de pulso 0, ou seja, estará sempre no nível *baixo*, ela emitirá 0V. Caso o pulso passe o mesmo período de tempo nos níveis *baixo* e *alto*, a largura da onda será de 50% emitindo assim 2.75V.

[//]: # (Colocar gráficos representando isso)

A placa Arduino UNO possui 6 pinos digitais que suportam o PWM. Eles são representados por um '__~__' ao lado da sua numeração, sendo eles os pinos de números __3__, __5__, __6__, __9__, __10__ e __11__. 

Para controlar os ciclos ativos nas portas, é utilizada a função  `analogWrite(pino, valor)`, onde `pino` deve ser um dos pinos PWM e `valor` deve ser um inteiro entre 0 e 255 (emitindo 0v e 5v, respectivamente). 


Hora de colocar isso em prática. A seguir será demonstrado um programa simples para fazer com que um LED vá aumentando e diminuindo seu brilho, em um efeito pulsante, utilizando as portas digitais com suporte a PWM.

### Hardware
#### Materiais necessários
+ 1 LED 
+ 1 Resistor de 330Ω

#### Esquemático

![Esquemático do projeto](./images/pwm.png)

A montagem do hardware é muito simples, basta conectar o ânodo do LED em um pino digital com suporte à PWM. Neste exemplo é utilizado o `pino 3`, mas sinta-se livre para utilizar qualquer um dos outros pinos, apenas lembre-se de declará-lo corretamente no momento em que for escrever o código! Também é necessário conectar o cátodo do LED ao resistor, que deve ser conectado ao terminal GND. Abaixo uma imagem demonstrando o esquemático para este projeto.


### Software

Primeiramente, é necessário declarar em qual porta o LED está conectado e o brilho inicial, que será 0, (ou seja, o led apagado). Também será necessário um valor que representará a taxa com que o brilho irá se modificar, que aqui será definido como 5. Assim o primeiro bloco de código fica :
 
``` C
int led = 3;		// Pino PWM em que o LED está conectado
int brilho = 0;		// Brilho inicial do LED
int taxa = 5;		// Taxa com que o brilho se modificará a cada iteração
```

Na função `setup()` será necessário apenas declarar o pino como sendo de saída com o seguinte comando `pinMode(led, OUTPUT);`. Já na função `loop()` deve-se enviar para o pino o brilho que o LED deve assumir, incrementar ou decrementar o valor do brilho (bem como checar se ele chegou aos limites de 0 e 255) e por fim, mas não menos importante, acrescentar uma pausa no loop para que seja possível visualizar alguma mudança significativa no LED. 

``` C
analogWrite(led, brilho);   

brilho = brilho + taxa;

if (brilho <= 0 || brilho >= 255) {
  taxa = -taxa;
}

delay(100);
```

Abaixo está o código completo para este programa

``` C
/* Utilizando PWM para controlar a intensidade de um LED */

int led = 3;      // Pino PWM em que o LED está conectado
int brilho = 0;   // Brilho inicial do LED
int taxa = 5;     // Taxa com que o brilho se modificará a cada iteração

void setup() {
  // Declara o pino do LED como sendo de saída
  pinMode(led, OUTPUT);
}

void loop() {
  // Define o brilho do LED
  analogWrite(led, brilho);   

  // Muda o valor do brilho para que na próxima iteração do loop
  // a voltagem no pino possa ser modificada
  brilho = brilho + taxa;

  // Caso estiver nos limites dos valores aceitos pela porta PWM,
  // inverte-se a taxa com que o valor do brilho é modificado
  if (brilho <= 0 || brilho >= 255) {
    taxa = -taxa;
  }
  // Tempo de espera para a proxima iteração, para que seja perceptivel 
  // a mudança no brilho do LED
  delay(100);
}
```

Ao compilar e enviar o código para a placa, você notará que o LED começará desligado e irá aumentar seu brilho até atingir um pico, e depois irá se apagando aos poucos. Caso queira que o pulso seja mais rápido, basta modificar o valor da taxa e/ou o tempo na função `delay()`.

![Projeto em funcionamento](./images/pwm-led.gif)
