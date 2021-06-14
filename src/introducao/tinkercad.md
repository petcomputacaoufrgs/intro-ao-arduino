# Plataforma Tinkercad

O Tinkercad é uma plataforma online e gratuita que apresenta recursos para o aprendizado, proporcionando a possibilidade de criação e simulação de modelos 3D e circuitos, incluindo o Arduíno. Para utilizar a plataforma, basta criar uma conta no [site oficial](https://www.tinkercad.com/) e em seguida, com um simples clique é possível criar um novo projeto de circuitos. 

 ![Página de projetos de circuitos](./images/tinkercad-1.png)

O Tinkercad oferece uma vasta gama de componentes eletrônicos para você utilizar, que aparecem no painel à direita. Existem várias categorias de componentes, desde os básicos (leds, botões, sensores e baterias), circuitos integrados, transistores, chips de lógica, instrumentos de medida (multímetro, osciloscópio) e microcontroladores (incluindo o Arduíno Uno R3). É um laboratório completo onde o limite é a imaginação do usuário. Por ter uma interface drag-and-drop, basta arrastar os componentes para a posição desejada. Tente arrastar uma placa Arduino para a área de projeto, como na imagem abaixo. Caso não consiga encontrar a placa, basta digitar seu nome na barra de busca acima da lista de componentes.

 ![Espaço de trabalho](./images/tinkercad-2.png)

Você notará que na barra superior existe um botão de código. Ao clicar nele a aba de programação é aberta.  O Tinkercad possibilita dois tipos de programação: uma utilizando código, da mesma forma que se programa em uma IDE, e outra em forma de blocos, baseada na linguagem Scratch.

 ![Códigos de blocos](./images/tinkercad-3.png)

É possível notar que no exemplo padrão, o LED incorporado à placa (ver [Anatomia do Arduíno](./anatomia-do-arduino-uno.md)) irá piscar com intervalos de 1 segundo. Ao clicar em `Iniciar simulação`, na barra superior, é possível ver esse comportamento na placa. 
Não só é possível programar em blocos, mas também ver o equivalente em código, assim. Dessa forma, a ferramenta acaba se tornando poderosíssima no aprendizado, visto que traduz algo em uma linguagem simples e visual em código para o arduino. Para habilitar essa visualização, basta mudar do modo `Blocos` para `Blocos + texto`. Para este exemplo inicial de piscar o led temos exatamente o mesmo código de exemplo que foi utilizado para testar a IDE. Note que não é possível editar o texto, para fazer isso é necessário mudar para o modo `Texto`

__CUIDADO:__ Ao mudar para o modo `Texto` uma mensagem de aviso é mostrada na tela. Esteja ciente que ao clicar em Continuar, todos os blocos serão perdidos. O código gerado por eles permanecem, mas o processo inverso NÃO É POSSÍVEL. Ou seja, uma vez mudado para o modo onde o texto do código é editável, não é possível retornar ao modo de edição em blocos, e qualquer tentativa de fazer isso fará com que seu código vire o exemplo padrão (LED embutido piscando a cada 1 segundo).
