# Protoboard

[//]: # (Talvez não seja o melhor lugar para se colocar essa sessão e esse conteúdo, vamos ver ao decorrer do curso se há a necessidade de uma página separada para isso ou se é melhor mesclar o conteúdo daqui com outras páginas  -    falar de componentes como led, resistor)

Também conhecida como “placa de ensaio”, “matriz de contato” ou até mesmo “breadboard”, a Protoboard,  como é comumente chamada no meio do Arduino, é uma placa com furos que possuem linhas de contatos entre eles, utilizada na montagem de protótipos. Essa placa se encaixa perfeitamente no contexto desse curso, pois testes e modificações são partes quase que intrínsecas de um projeto em Arduino, ainda mais quando se está no processo de aprendizagem. 

Protoboards consistem basicamente dois grupos de faixas, são eles:

+ Faixa de terminais: faixa de contatos onde são instalados os componentes eletrônicos. São trilhas dispostas na vertical, geralmente em grupos de cinco conectores e um entalhe, demarcando a linha central da placa (que normalmente é espelhada) e para melhor acomodar circuitos integrados e outros componentes que possam vir a ser instalados.
+ Faixa de barramentos: usada para o fornecimento de tensão ao circuito, é constituída de duas faixas horizontais na extremidade, uma reservada para o condutor negativo (terra, marcado em preta ou azul) e outra para o positivo, marcado em vermelho. 

É possível imaginar essas faixas como se fossem um único fio (e, de fato há uma pequena faixa metálica que as conecta). Assim, ao plugar um componente em um terminal, é como conecta-lo a todos outros componentes em toda a faixa. É possível ver o alinhamento dos terminais na imagem abaixo.

 ![Protoboard](./images/protoboard-1.png)

A possibilidade de modificar posições de peças facilmente, rearranjar cabos e adicionar novos componentes faz com que o projeto seja facilmente modificado para corrigir possíveis erros ou implementar melhorias no projeto. Contudo, existem lados negativos em seu uso: pode haver “mau-contato” entre os terminais e resistência entre os contatos da placa e os componentes encaixados além de que um elevado número de “jumpers” pode causar interferência em outros componentes. Por essa razão, recomenda-se o uso de “jumpers” curtos e que não se faça muitos cruzamentos entre eles.
