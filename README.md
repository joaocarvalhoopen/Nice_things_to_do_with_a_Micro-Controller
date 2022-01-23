# Nice things to do with a Micro-Controller
Coisas engraçadas e económicas que se podem fazer com um micro-controlador.

## Descrição

Imaginem os componentes e sensores mais simples e os mais baratos, e na perspetiva de se conseguir fazer o máximo possível com o mínimo possível de hardware ... quais são esses sensores e componentes e as suas aplicações: <br>

1. LED

2. Switch

3. Resistência

4. Condensador

5. Indutor

6. Pino capacitivo (Num micro-controlador sem suporte para pino capacitivo nativo)

7. Disco de Piezo (tipo postal de Natal)

8. Pino com um transístor MOS-FET capaz de comutar rapidamente.

9. Pino Emissor de Radio frequência (onda eletromagnética)

10. Pino de entrada de ADC para fazer sampling a ondas eletromagnéticas de rádio (pode ter de levar um andar de amplificação antes e processamento digital do sinal - difícil, mas exequível em alguns micro-controladores mais potentes Cortex M4 com floating point).

11. Play, gravar, processamento, reconhecimento e text-toSpeech de áudio num micro-controlador

12. Com díodos, transistores e OpAmp’s conseguem-se fazer muitos circuitos interessantes analógicas mesmo que sejam coisas simples e consegue-se alta velocidade analógica.

13. Ecrã LCD 16x2 de 4 euros.

14. Microfones de I2S

15. Pino capaz de ligar e desligar 220 V e alta potência num Relé. (Este não queria pois os Relés são normalmente usados com 220 V e eu não gosto da ideia de usar 220 V nos meus mini projetos, eles devem ser brincadeiras e não coisas sérias que exijam alta segurança para não haver risco de eletrocussão ou de incêndio, quer no desenvolvimento, quer na sua futura utilização, 220 V abre uma CAN of Worms!) <br>
<br>

Agora vou tentar listar todas as funções / aplicações de projetos que consigo imaginar ou lembrar-me para cada um dos componentes ou sensores simples atrás descritos. Coisas que sejam engraçadas e simples. <br>


## 1 - LED

1. Usar um LED para dar luz ON / OFF simples (em que o ON está a 100%).

2. Usar um LED com um padrão complexo de ON / OFF (em que o ON está a 100%). Exemplo emitir código Morse, como forma de comunicação ou de interface com o utilizador.

3. Usar dois LED como comunicação por luz, um emissor e outro recetor. Ou um LED com um foto transistor recetor.

4. Usar um LED com um padrão de PWM que permite escolher as diferentes intensidades do LED ao longo do tempo. (imaginem os programas de LED chama, um led que parece que é uma chama, ou de breading LED dos Mac’s).

5. Usar um LED como uma matrix de LED’s com Rows e Colums.

6. Usar um LED com esquemas de Multiplexing, existe um esquema avançado que permite colocar muitos LED’s em poucos pinos. Acho que é Charly Multiplexing ou algo assim.

7. Usar um LED com um transitor FET para que tenha breves picos de muita corrente durante uma fração muito pequena de tempo, só um instante para que ele funcione e dê um flash intenso de luz mas por um breve instante muito acima do seu regime normal, mas sem queimar por ser breve, só um instante de tempo, que podem ser pulsos periódico.

8. Usar um LED RGB e fazer uma cor à escolha de luz de LED.

9. Usar LED’s vermelhos cuja luz consegue atravessar mais os tecidos moles do corpo humano. Led de um lado e foto transistor do outro que depois faz o varrimento manual ou automatico, para tentar detetar a densidade ou obstrução feita pelas estruturas dos ossos em tecidos moles, ou a sua densidade, um pouco como se fossem algo tipo raios X, mas sem o ser, sem os efeitos nefastos e muito bazarouco. Mas acho que funciona.

10. Usar um LED para detetar a pulsação cardíaca pela diferença ou variação da refletividade da hemoglobina à cor vermelha consoante está a transportar sangue oxigenado (mais refletivo) ou desoxigenado (menos refletivo) (oxímetro) e quando as veias dilatam pelo aumento da pressão do batimento cardíaco. É um LED e um foto sensor no dedo.

11. Usar LEDs vermelhos e foto sensores numa espécie de capacete de LED’s espaçados vermelhos com respetivo fototransistor e assim detetar em cada momento a intensidade de sangue que corre em diferentes partes da cabeça / ”cérebro”, depois tentar fazer diferentes atividades cognitivas e de usar um programa de machine learning para detetar os diferentes tipos de atividade. Relação entre o fluxo do sangue detetado nos diferentes LED’s e a atividade.  

12. Usar um LED normal como sensor de LUZ usando um ADC ligado a ele. Que permita medir de forma rápida a intensidade da luz ambiente e variações dessa intensidade ao longo do tempo ou instantanea.

13. Usar um LED como um botão detetando a diferença de temperatura no LED, por alteração da voltagem de Forward Voltage, quando se toda no botão.

14. Usar um LED como detetor de sopro pela diferença de temperatura no LED. (lima-se o LED até ter menos plástico e depois deteta-se a diferença de voltagem de funcionamento do LED causada pela diferença de temperatura).

15. Usar um LED como um díodo.

16. Usar um LED enquanto díodo que tem uma capacidade de junção muito baixa como detetor de ondas de rádio. Por exemplo saber se o telemóvel está a emitir ou o forno micro-ondas.

17. Usar um LED enquanto díodo que tem uma capacidade muito baixa de junção como detetor cabos elétricos  com energia, EMF detector.

18. Usar um LED ou 5 LEDs com movimento (mão em rápido movimento para a um lado e para o outro, ou motor em eixo rotativo) para implementar Persistent of Vision e com isso desenhar no ar uma imagem ou escrever letras ou mensagens no ar.

19. Usar um único LED ou foto transistor como sensor de luz e uma canula (pequeno tudo escuro no LED) e dois pequenos servos motores (fazendo dois eixos de varrimento) e com isso fazer uma pequena camera sem lentes com um único pixel mas que consegue tirar várias imagens. E Se o LED  for na frequência de IR – Infravermelhos ainda consegue também tirar fotografias de infravermelhos.

20. Com LED foto transistor de infravermelhos fazer um recetor de comando de infravermelhos.

21. Com LED de infravermelhos fazer um emissor de comando de infravermelhos.

22. Consegui montar um link de comunicação por infravermelhos com dois LED (LED e fototransistor).

23. Fazer um sensor de distância a um objeto como uma mão, com dois dois LED’s ou com um LED e um fototransistor por intensidade da reflexão. Pode ser com LED’s de cor normais ou brancos, ou pode ser com LED’s de luz infravermelha.

24. Usar um LED e um interruptor para medir os tempos de reação de uma pessoa entre ver a luz do LED e carregar no botão.

25. Usar LED’s em regime de alta potencia por um período muito breve, tipo instantâneo. Mas que pára um determinado movimento no tempo, por ser estroboscopico a uma determinada frequência. Assim por aleasing, ele pára esse movimento ou até o consegue criar a ilusão de por o movimento a andar para trás no tempo. Isto, dependendo da frequência do ON/OFF do LED e do speaker. Imaginem uma mangueira a pingar gotas de água e em que se cola a mangueira ao cone de um speaker e se gera uma determinada frequência baixa no Speaker de ex: 40 Hz e que depois numa sala escura se ilumina estrobostopicamente (com periodicidade fixa e com grande intensidade por flashes de breves instantes), consoante a frequência é menor, igual ou maior do que a frequência do movimento causada pelo speaker. O que se vai ver com os nossos olhos a olhar para a gotas, elas vão cair mais lentamente, até pararem no ar, e depois se se ultrapassar a frequência do speaker vai se ver as gotas a subir em pleno ar pelo tubo e a voltarem a entrar no tudo. Como se o tempo andasse para trás. Num efeito de aleasing do limite de Nyquist. O mesmo pode ser visto usando uma camera e sem usar os leds só variando a frequência do speaker pois a camera já tem o efeito de sampling na sua captação da imagem que provoca o efeito de aleasing que é o que vamos detetar.

26. Fazer um Theremin (Instrumento musical) com dois circuitos que medem a distancia as duas mãos com LED’s e que com isso usam para modelar e controlar o som do Theremin tanto em intensidade como em frequência.


## 2 - Switch

1. Fazer o debouncing de um interruptor ou botão.

2. Usar o facto do tempo entre bounces e o número de vezes do bouncing de um botão ser aleatório em cada pressionar, como seed para algoritmo de geração de números aleatórios.

3. Medidor de tempo de Reação com LED e switch.

4. Com com um pequeno micro switch sensível, detetor de porta aberta ou porta fechada, ou detetor de fim de curso e um movimento ou calibrar até á sua posição inicial.

5. Com dois fios e um pedaço de metal a fechar o contacto de uma porta ou janela.

6. Com um micro-switch e o peso de uma porca a detetar a orientação de uma caixa, se está virada para cima.

7. Coherer – Interruptor detetor de ondas de rádio. <br>
   [https://en.wikipedia.org/wiki/Coherer](https://en.wikipedia.org/wiki/Coherer)

8. Detetor de que uma coisa está em cima do interruptor, usando como sensor de pressão.

9. Com switch e com embolo e mola (tipo seringa) detetor de pressão do ar.

10. Com um switch e um único fio e com um circuito que detete a capacidade (sensível) conseguir detetar que o fio tem mais capacidade pois tem mais metal da parte da ligação final do interruptor por estar na posição ON vs a OFF.

11. DPDT switch – Comutadores de circuitos, ou entre o processamento de duas fontes de sinal diferentes ou duas saídas de potencia diferentes.

12. Interruptor de pressão simples que está ligado a micro-controlador e que consoante o tempo pressionado vai aumentando a luz e depois diminuindo e em que a pessoa larga o botão quando estiver satisfeito com a intensidade do que está a ligar, seja a intensidade da luz de um led, seja o volume de um aparelho de som. 


## 3 - Resistência

1. Limitar a corrente

2. Aquecer algo, aumentar a temperatura, gerindo com termostato ou com controlador por software de PID.

3. Cortar um fio de Nylon que solta algo por aquecimento quando se coloca uma resistência de pouca potência. 

4. Circuito que fica cortado, aberto a partir de altura que se passa uma corrente superior ao rating (valor limite da potencia da resistências ex:1 / 4 W) da resistência. Como se fosse um fusível programado para ser usado uma vez.


## 4 - Condensador

1. Detetor de movimento, alguns condensadores são microfónicos e alteram a sua capacidade quando são comprimidos.

2. Detetor microfónico em alguns condensadores, pode-se inclusive usar como um tosco microfone.

3. Condensadores feitos à mão com placas de folha de alumínio de cozinha entre folhas de plástico e que podem ser fixos ou variáveis.

4. Usados em filtros passa baixo e filtros passa alto simples.

5. Usados em sensor capacitivo ou os sensores capacitivos medem a capacidade em muitas outras coisas.

6. Com díodos, como geradores de alta voltagem através de um circuito doubler.


## 5 - Indutor

1. Circuito RLC para amplificar / selecionar uma única frequência.

2. Forma de gerar picos de altas voltagens (por ligar ou carregar indutores e desligar muito rapidamente a corrente, gera um pico reverso).

3. Geração de campos magnéticos.

4. Bobine muito pequenas feita à mão para emissor de FM, enrolando fio numa caneta, lápis ou parte de trás de uma broca.

5. Speaker DIY simples, feito com prato de plástico ou folha de papel (cartolina) e íman e bobine enrolada.

6. Transferência de energia elétrica sem contacto por efeito de transformador separado no ar, a curta distância, feito somente com dois enrolamentos de fios a altas frequências.

7. Alimentar circuitos de díodos varicap (Variable capacitance) com corrente forward de forma a ajustar a capacidade do díodo e logo sintonizando o circuito e sem afetar as altas frequências.

8. Detetor de metais ou e de tipo de metal com uma bobine e um circuito RLC.


## 6 - Pino capacitivo - Num micro-controlador sem suporte para pinos capacitivo nativo

Um pino capacitivo implementado num micro-controlador por software mede a capacidade existente num pino ou fio, ou pequena parte de metal como uma das placas de um condensador em que a outra placa é a pessoa sem contacto elétrico (distância variável) . Quer seja pelo tempo de carga ou de descarga dessa capacidade. O ESP32 implementa isto em hardware mas pode-se implementar isto em software.

1. Detetor de toque humano, usando num fio ou um pad numa placa de PCB ou bocado de alumínio pequeno como um botão.

2. Usar como um botão, mas como um botão de slide em que por exemplo se pode escolher a intensidade do volume de som ou da luz de um LED, usando vários pinos.

3. Matriz de botões muitos simples feita com contactos por baixo da camada protetora do cobre de um PCB.

4. Usar como detetor de distância de proximidade de uma mão humana ou da cabeça humana ou da postura humana.

5. Com folhas grandes de alumínio em placas de esferovite, detetar a passagem de uma pessoa no corredor de um quarto ao lado dentro de uma casa, através da parede.

6. Joystick no ar a 3D feito com 3 folhas de alumínio de cozinha coladas num canto de uma caixa de papel ligadas a 3 pinos a funcionar como pino capacitivo de micro-controlador e em que se mede a distância a uma determinada placa pela capacidade de cada placa à medida que a mão altera a sua posição dentro do canto da caixa, ex: 30cm x 30cm x 30cm . Para melhorar a precisão pode-se colocar um algoritmo simples de Machine Learning para aprender a correspondência entre os valores de cada capacidade em cada um dos 3 eixos com a posição da mão, no espaço a 3D.  

7. Usar como identificador de uma pessoa numa família, detetando a capacidade diferente ao tocar no circuito de uma pessoa grande vs uma pessoa de estatura média vs uma criança. Pessoas de estaturas diferentes tem capacidades diferentes.

8. Usar como forma de detetar se várias pessoas (até 4) se estão a tocar ou a dar as mãos, pois a capacidade altera quer seja a fechar um circuito ou só pelo aumento da capacidade ao tocar num único fio.

9. Detetar se uma pessoa tem os sapatos colocados ou está de meias no chão de pedra ou tijoleira pelo aumento da capacidade quando toca no fio de um circuito destes que mede a capacidade com o ground, ou seja se tem um ground melhor ou pior. 

10. Detetar os diferentes dedos em contacto ou partes do corpo diferentes à superfície de contacto do metal do pino capacitivo por analise do padrão de intensidade diferentes para frequências que são emitidas (as suas diferenças de voltagens de um circuito RLC) a diferentes frequências de ressonância no corpo humano (diferentes caminhos Paths AC 3.3 V e só de sinal) consoante se tem um dedo a tocar ou dois ou 3 dedos por exemplo numa maçaneta de uma porta (e com  isso introduzir em sequência ou uma combinação secreta na maçaneta de uma porta que abre a porta heheheh), ou num tanque com água. Procurar na net pelo projeto Touché e procurar na net por uma implementação open source do projeto touché que descreve o funcionamento do hardware, existe uma . Pode ter de ser usado ML para conseguir classificar os diferentes tipos de padrões de contacto ou diferentes movimento, mas a ML pode ser muito simples. Isto necessita se não me engano de um circuito RLC. Para ML ver os algoritmos do site Eloquente Arduino.

11. Detetar a altura de um liquido, ex:  2 latas de refrigerante, cortada e colocada dentro de um liquido com duas bocas de crocodilo e isoladas por saco fino de plástico. Consoante se aumenta a altura do liquido assim aumenta ou diminui o dielétrico do condensador e como tal se aumenta ou diminui a capacidade do condensador.

12. Detetor de espessura de um material, pois quando mais espessura mais altera a capacidade do condensador, pois altera a espessura do seu dielétrico.

13. Usando 3 pinos destes de MCU (algo tipo relógio em contacto com a pele) e mutiplexados no tempo para que só um esteja em funcionamento em cada momento. como os 3 pontos de um ângulo retângulo a 2D, determinar a distancia de um toque numa superfície do nosso braço por correlação do sinal e dos seus diferentes capacidades de cada um dos sensores, com isso consegue-se determinar com muita precisão a posição X/Y em se tocou no braço. E fazer do nosso braço um teclado de entrada ou um device de entrada de dados. Existe um paper que implementou um device destes. Eles usam um algoritmo simples de ML para determinar o mapeamento entre a capacidade em cada um dos 3 sensores do braço (relógio em contacto com a pele) e a posição do dedo que está a tocar no braço. Não me recordo se o dedo está ligado ao ground do circuito a pilhas ou se não tem ground. <br>

<br>

Ver detalhes em: <br>
[https://www.lionprecision.com/capacitive-sensor-operation-and-optimization-how-capacitive-sensors-work-and-how-to-use-them-effectively/](https://www.lionprecision.com/capacitive-sensor-operation-and-optimization-how-capacitive-sensors-work-and-how-to-use-them-effectively/)

<br>

Ver detalhes em: <br>
Instructables - Capacitive Sensing for Dummies <br>
[https://www.instructables.com/Capacitive-Sensing-for-Dummies/](https://www.instructables.com/Capacitive-Sensing-for-Dummies/)


## 7 - Disco de Piezo (tipo postal de Natal)

Cuidado com os circuitos de piezo, tem de se proteger contra os picos de voltagem gerados e causados por impactos físicos grandes, se o pico for muito grande pode estragar a porta do pino do micro-controlador, usar um díodo para proteger essa entrada.  <br>

1. Usar um piezo como speaker de tons simples, como tocar as músicas de Natal.

2. Usar um piezo como um speaker de áudio normal mas de baixa qualidade.

3. Usar um piezo como um microfone de baixa qualidade ligado a um ADC, é engraçado que um pequeno altifalante também pode ser usado como microfone.

4. Usar como detetor de movimento. Por exemplo se estiver dentro de uma caixa que se abana ou que se movimenta bruscamente.

5. Usar como detetor de movimentos muito subtis caso se use um comparador sensível discreto ou um ADC de alta resolução de poucos milivolts consegue-se colocar uma caixinha com um piezo dentro colado a caixa e detetar se uma pessoa do outro lado da mesa tocou muito ao de leve com um dedo na mesa, nice! Isto pode ser usado para acordar um micro-controlador de deep sleep e fazer o micro-controlador começar alguma atividade ou para o desligar, exemplo alarme luminoso. Ou fazer outro tipo de interface.

6. Usar essa mesma propriedade do piezo para detetar movimento ou ação, mas com 2 piezos ou 3 piezos, fazer com um ADC sampling aos sinais e classificar o tipo de ação que ocorreu com Machine Learning e assim detectar certas ações. Por exemplo pousou-se um lápis na mesa, ou uma caneca ou uma borracha, ou pousou-se um cabide num varão com um casaco ou foi um cabide vazio, ou está-se a tocar numa determinada parte do da mesa ou de um carro, ou algo assim em que se consegue determinar e classificar corretamente um tipo de ação.
 
7. Usando um único piezo, fazer um detetor de passos num corredor ou numa sala e com isso saber se uma pessoa se está a aproximar ou a afastar pela intensidade dos passos, ver exemplo do livro fantástico de AVR. <br>
   **Make - AVR Programming: Learning to Write Software for Hardware** <br>
   by Elliot Williams

Ver o gráfico da intensidade vs frequência dos discos ou sensores de cristal de piezo. <br>
[https://www.avnet.com/wps/portal/abacus/solutions/technologies/sensors/pressure-sensors/core-technologies/piezoelectric/](https://www.avnet.com/wps/portal/abacus/solutions/technologies/sensors/pressure-sensors/core-technologies/piezoelectric/)

1. Detetor de pulsação cardíaca, ao colocar o dedo em cima do disco de piezo e de detetar a pulsação da pessoa como picos de intensidade de voltagem.

2. Usando 3 discos piezo como os 3 pontos de um ângulo retângulo a 2D, determinar a distância de um toque numa superfície a cada um dos sensores, mesa ou madeira por correlação do sinal e dos seus diferentes tempos de chegada a cada um dos sensores, com isso consegue-se determinar com muita precisão a posição X/Y em se tocou na mesa ou na madeira. O mesmo pode ser feito para um giz num quadro de negro pois está sempre a emitir bribrações e pode-se fazer por correlação ou por deteção de picos.

3.  Radar doppler - Esta não sei se é possível com dois discos de piezo (mas talvez seja possível) mas é possível com um speaker e com um microfone. Envia-se continuamente um tom / som / sinal a uma determinada frequência precisa e depois com o outro piezo ligado a um ADC está a funcionar como microfone que recebe o sinal sonoro diretamente do primeiro piezo e vai receber também um sinal muito mais pequeno (numa frequência diferente adjacente) de uma pessoa a andar para a frente e para trás a aproximar-se ou a afastar-se a velocidades diferentes e com isso consegue detetar a velocidade da pessoa (mais ou menos) e se essa velocidade na direção positiva ou negativa. Para isso gera-se um sinal no piezo A numa frequência fixa, depois faz-se o sample no piezo B com o ADC e depois faz-se uma FFT e determina-se se os buckets ao lado para a direita (componente de frequência mais alta da FFT do que o sinal original) tem intensidade ou se não tem e faz-se o mesmo para os buckets mais baixos, pois a pessoa ao andar para a frente e para trás vai comprimir as ondas ou afastá-las. Gerando um sinal de áudio mais pequeno a uma frequência mais alta ou mais baixa consoante a direção, velocidade do movimento e a área de reflecção da pessoa. Existe um paper da Microsoft sobre isto e como implementar num PC e eu tenho um projeto de PC em Python no meu github que implementa isto. É simples.

**Stimson's Introduction to Airborne Radar, 3rd Ed** <br>
by George W. Stimson, Hugh D. Griffiths, Christopher J. Baker, Dave Adamy <br>


4.  Radar medidor de distâncias, ou espessuras, ou fraturas em sólidos ou no ar medindo o tempo de propagação do impulso entre um sensor de piezo emissor e um recetor de piezo. A velocidade de propagação depende do meio, ou seja do material (ar, versos metal, versos água, versos pedra).

5.  Implementação de um sonar hidrofónico com um único disco de piezo (e um banho de silicone isolador) em que o piezo ora está a emitir um sinal ora está à escuta dos ecos do sonar e mede o seu tempo de propagação.

6.  Implementação de um microfone hidrofónico com um piezo para trabalhar debaixo de água. Ouvir os peixinhos hehehehehe ou os barrulhos no mar, pois a água propaga muito bem o som, a grande velocidade e a grandes distâncias.

7.  Implementar um sensor captador de áudio com um piezo para uma guitarra acústica ou clássica ou outro instrumento não eletrificado. Basicamente deteta a vibração. Isto pode inclusive ser usado para fazer uns pads silenciosos de bateria que depois o micro despoleta um sinal MIDI e que o computador toda um determinado sample de bateria.

8.  Medir a altura de um liquido dentro de um recipiente, por exemplo colocar um sensor na base do recipiente com água e depois enviar um chirp muito curto ou pico e detetar uma de duas coisas, ou o pico do som refletido no cimo da água e que volta outra vez para o sensor de piezo e esse tempo depende da quantidade de água que existe dentro do recipiente, ou então fazer um varrimento de frequências no piezo e detetar a frequência de ressonância do recipiente que se altera consoante a quantidade de liquido que existe dentro dele. Depois é só mapear uma coisa para a outra quer por simples tabela, quer por mapeamento aprendido por um algoritmo de Machine Learning.

9.  Gerar ultrasons com discos de piezo que podem ir até aos 1 MHz mas que são discos ligeiramente diferentes. (nesse campo depois podemos pensar em ver dentro do corpo humano, pois o corpo humano é feito de água e transmite bem o som, podemos pensar em medir distâncias com grande precisão como por exemplo a altura de líquidos).


## 8 - Pino com um transístor MOS-FET capaz de comutar rapidamente.

1. Com isto conseguem-se controlar electro-válvulas, consegue-se ligar ou desligar relés, consegue-se ligar ou desligar motores que rodam numa única direção.

2. Ligado a um pino PWM consegue-se alterar a velocidade de um motor que roda para um só lado, consegue-se fazer a modelação da intensidade de um LED de potência, consegue-se implementar um amplificador de classe D que alimenta um ou mais speakers e que é muito eficiente.

3. Consegue-se controlar todas as fases de um steper motor, um transistor por cada fase.

4. Consegue-se implementar com 4 MOS-FET um ponte em H que permite controlar um motor para  rodar nas duas direções e com variação de velocidade que depois pode inclusive ser controlado por algoritmo de PID - Proporcional, Integrative and Diferential control. Existem chips baratos para fazer pontes H.


## 9 - Pino Emissor de Radio frequência (onda eletromagnética)

1. Um simples pino de um micro-controlador sem mais nada ou ligado a um simples transistor pode ser usado para uma experiência de fazer um pequeno emissor de AM – Amplitude Modelada com pequeno alcance se a antena for só um pequeno fio e o recetor for um rádio de AM comercial. Existem dois modos de funcionamento, ou se enviam musicas em simples mas diferentes tons ou se modela o AM com um som de áudio que se recebe por um jack de 3.5mm e que é capturado no ADC do MCU e modelado e emitido pelo emissor de AM. <br>
   Vejam a descrição fantástica do projeto do livro: <br>
   **Make - AVR Programming: Learning to Write Software for Hardware** <br>
   by Elliot Williams



2. Pode-se fazer um emissor de algo como o Weak Signal Propagation Reporter Network que vai a grandes distâncias e que é simples de construir. A complexidade está toda no recetor, o emissor também pode ser feito com o PWM de um Raspbery PI <br>
   [https://www.wsprnet.org/drupal/](https://www.wsprnet.org/drupal/)

3. Era bom que se conseguisse fazer um Radar com os pinos de um micro-controlador, mas como para ter boa emissão a baixas potências de poucos mW, ou se tem nas baixas frequências que um microcontrolador consegue comutar um pino de 1 a 100 MHz se tem de ter antenas muito grande o que não é praticável. A 1 megahertz estamos a falar de antenas de centenas de metros ou se tem antenas pequenas mas se tem de ir para frequências de giga hertz em que os micro-controladores atuais não conseguem gerar por software essas frequências. Por isso radares diretos em micro-controladores não são fáceis de fazer, mas seria muito giro se se conseguissem fazer. Todas as implementações de radares em pequenos devices usam circuitos de transistores e RLC’s feitos em microstrips de PCB na frequências de giga hertz e isso é Black Magic da eletrónica. Já é preciso saber muito de eletrónica para conseguir fazer isso. E ter equipamento caro. Mas nada é impossível. O primeiro Radar dos Ingleses na segunda guerra mundial funcionava a 1 MHz ou a 10 MHz, mas as antenas eram gigantescas e estava em toda a costa com a França.



## 10 - Pino de entrada de ADC para fazer sampling a ondas eletromagnéticas de rádio 

Pode ter de levar um andar de amplificação antes e processamento digital do sinal, difícil, mas exequível em alguns micro-controladores mais potentes Cortex M4 com floating point. <br>

1. É possível de se usar um micro-controlador nomeadamente o ADC com um OpAmp antes para se fazer diretamente um SDR – Software Defined Radio. Existe código OpenSource online em mais de um projeto e existe um livro muito bom sobre como implementar um SDR do zero. Mas isto é um projeto muito difícil de se fazer pois é muito código DSP avançado e tem de ser código muito otimizado pois todo o processamento tem de ser feito em tempo real a altas frequências. Os MCU’s normalmente tem de ter um clock superior a 100 MHz e tem de ser um ARM Cortex M4 com floating point e instruções de DSP. Mas muitas coisas giras já foram feitas nesta área. <br>
   **Software Receiver Design: Build your Own Digital Communication System in Five Easy Steps** <br>
   by C. Richard Johnson Jr, William A. Sethares, Andrew G. Klein

2. Radar também seria uma opção mas é demasiado difícil fazer-se a frequências baixas, quer da  onda de rádio quer do MCU, quer das antenas muito grande que teria de ter devido à baixa frequência das ondas usadas. 

3. Num ADC é possível fazer o sampling de frequências muito mais elevadas do que o máximo do teorema de Nyquist nos diz para a sampling frequency máxima do ADC. Isto se soubermos que a única frequência que temos no pino está acima da frequência de sampling do ADC, mas abaixo da frequência de limite analógico do ADC. Que normalmente é muito superior ao que o limite do sampling rate máximo. Ou seja, consegue-se obter uma frequência mais alta do que a sample rate por aliasing e se souber-mos qual é a gama de frequência original (em que largura de banda cai), conseguimos reconstruir o sinal original num array no MCU.

4. Pode-se usar técnicas de over-sampling por software, num ADC para aumentar a sua resolução e precisão por averaging.

5. Pode-se usar técnicas de Compressive Sensing para não necessitar de tanto volume de dados ou para se conseguir frequências muito mais altas do que a frequência de sample rate.

6. Técnicas de DSP são muito úteis em todos estes tipos de processamento de sinal.


## 11 - Play, gravar, processamento e reconhecimento de áudio num micro-controlador

1. Play de musicas guardadas na flash de memoria do programa do micro-controlado, comprimidas em ADPCM – Adaptive Differencial Pulse Code Modulation em mono a 8 Khz de Sample Rate. Ver App Note da STM32 que está no site do STM32F103. O áudio do ADPCM pode ser gerado num programa no PC e incluído os bytes num array do código do programa do micro-controlador. A cada sample é gerado temporizadamente um valor com um PWM, ou com um DAC – Digital to Analog Converter ou som dois PWM’s encadeados um fazer de low bit’s e outro de high bit’s para se ter mais resolução no PWM e melhor qualidade de som.

2. Pode-se ter um interface humano de output por voz recebendo o resultado como sons encadeados, exemplo números do resultado de uma calculadora ou pequenas instruções como cima, baixo, esquerda, direita ou saltar. Ou pode-se ter frases mais compridas em que poucos sons são reutilizados muitas vezes.

3. Fazer o play usando um chip de uma memoria flash barata por I2C ou SPI que tem muita capacidade vários Mega Bytes e custa só uns cêntimos. Alguns micro-controladores como o ESP32 e o pico tem flash de programas muito grandes.

4. Gravar áudio - Capturar e fazer o sampling é necessário usar um ADC e fazer o sampling a ex: 8 Khz com um timer a gerar os instantes de sampling do ADC o chamado modo continuo para um buffer que tanto pode ser um Ring Buffer (ocupa menos memoria) como pode ser um esquema de double buffer em que enquanto o ADC está a escrever para o buffer A por DMA – Direct Memory Access, o micro-controlador está a processar o buffer B por exemplo fazendo uma FFT e depois dando o resultado da análise de alguma forma como num LCD de 16x2 ou como a emissão de AM de um pino do micro-controlador, ou como uma amplificação de um amplificador de classe D muito eficiente feito com um micro-controlador e um transistor FET, ou fazendo por exemplos os efeitos de som de uma pedaleira de guitarra.

5. Reconhecimento de comandos simples num micro-controlador isto é mais complexo, mas para comandos simples também é exequível com um pouco de machine learning, ver o site do Eloquente Arduino que tem lá um exemplo disso.

6. Text to speech em micro-controladores também é possível e existe uma empresa que faz isso com mensagens pré codificáveis em fonemas, existe alguma coisa na net sobre isso, mas não é muito fácil de se fazer. Antigamente existiam uns chips que faziam isso.

7. Existem algoritmos de compressão de áudio open source que conseguem descer a 1.2 ou 1.3 Kbytes / segundo mas usam muito poder de calculo para o conseguir fazer e são muito complexos, ver o post do Hackaday sobre os codecs. Para as coisas normais e para ser simples o ADPCM é simples de implementar.

8. O som que sai de uma aplicação de áudio pode sair de muitas formas diferentes:
   - Por um jack de 3.5mm em intensidade padrão de ligações de áudio para ser amplificada externamente. 
   - Pode sair para uma saída de Phones já amplificada com um OpAmp para uns phones.
   - Pode sair por PWM ou DAC para um amplificador LM386 simples externo e ligado a um speaker.
   - Pode sair por um PWM ligado a um MOS-FET que implementa um amplificador de classe D ligado a um speaker pequeno ou grande.
   - Pode sair como dois PWM’s coordenados em que um faz os low bits e o outro faz os high bits para que se tenha mais resolução e qualidade na saída do áudio para qualquer dos tipos de amplificação.
   - Pode sair para um disco de piezo (não tem grande qualidade mas gera áudio e não só tons).
   - Pode sair por BLE ou por WIFI para um telemóvel e ser amplificada pelo sistema de amplificação do telemóvel ou do PC, por exemplo abrindo um porto com sockets.



## 12 – Com díodos, transistores e OpAmp’s

Conseguem-se fazer muitos circuitos interessantes analógicos ou partes de circuitos mesmo que sejam coisas simples e consegue-se alta velocidade analógica. <br>

## Díodos

1. Usar um díodo para medir a temperatura.

2. Usar um díodo Zener para regular a corrente.

3. Usar um díodo como detetor de RF – Radio Frequencies

4. Usar um díodo para proteger a polaridade da alimentação de um circuito, de preferência um de baixa queda de tensão, um schotky.

5. Usar díodos como forma de fazer um condensador com uma capacitância variável, quer seja usando um díodo normal quer seja usando um díodo VeriCap, bom para ser o C de circuitos RLC de resonância.

6. Usar um díodo de uma galena para fazer a desmudelação de uma emissão de RF de AM.

7. Como frequency multipliers em RF.


## Transistores

1. Amplificadores de microfone de electreto que depois são sampled por ADC.

2. Amplificador de phones ou de speakers por transistor FET (pequeno ou grande) , classe D.

3. Amplificador linear de áudio feito com transistores, classe A, classe B, classe AB, Push-Pull.

4. Como switch’s de maior potência.

5. Como amplificadores a diferentes frequências.

6. Como osciladores.

7. Como modeladores.

8. Como detetores.

9. Fast peak detector.

10. Como transistores de avalanche que conseguem fazer pulsos muito rápidos de corrente e quando estão ligados a bobines conseguem criar pulsos na ordem dos picos ou mesmo fento segundos, bons para medir a frequência de resposta de um osciloscópio.


## OpAmps

1. Amplificadores de microfone de electreto que depois são sampled por ADC.

2. Amplificador de phones por um unico OpAmp.

3. Todo o tipo de filtros feitos com OpAmps, passa baixo, passa banda, passa alto, notch e muito mais.

4. Como amplificadores de sinal, quer sinais muito baixos (nano ou micro volts), quer sinais muito rápidos, quer sinais com pouca corrente (fento ou pico amperes).

5. Como voltage follower ou buffers de ganho unitário.

6. Circuitos inversores.

7. Conversores de corrente para voltagem.

8. Como retificadores ativos,

9. Como integradores e diferenciadores

10. Como comparadores de voltagem.


## 13 – Ecrã LCD 16x2 de 4 euros.

1. Estes ecrãs são muito económicos, e são muito úteis para mostrar todos os tipo de mensagem quer estáticas quer em movimento em animação. Eles têm um interface com muitos pinos mas que pode ser usado como interface de 4 bits (menos fios) e de 8 bits’s (mais fios) e pode ser inclusive usado com uma placa de I2C (esta placa custa quase tanto como o LCD) que depois tem uma ligação de menos fios ao MCU. Existem libs para todos os micro-controladores para usarem com estes este tipo de ecrã de LCD standard.

2. Um LCD destes já vem com um número pré-configurado de caracteres diferentes que se podem usar. Mas podem ser criados no momento novos tipos de caracter na memória do LCD e com isso fazer pequenos gráficos ou animações num ecrã como por exemplo um barra de progresso com uma percentagem no final. Isto por exemplo na segunda linha e em que na primeira linha tem uma descrição do que está a fazer. O facto de programar-se os caracteres como gráficos pode inclusive ser usado em jogos para ter um desenho de uma pessoa a andar ou algo assim, ou de uma bola ou de outra coisa qualquer.

## 14 -  Microfones de I2S

1. Existem alguns microfones MENS baratos de telemóvel que vem em placas com interface interno de I2S, nem todos os micro-controladores tem interface I2S, o ESP32 têm, mas o I2S pode ser simulado por software em outros micro-controladores que não o tenham.

2. Com um microfone e com um amplificador de speaker classe D de transistor e com o algoritmo de PSOLA (está no meu github uma implementação) que altera a frequência da voz ou seja o seu timbre fazer uma brincadeira de tornar a voz de uma criança na voz de uma pessoa mais velha ou a voz de uma mulher na de um homem, ou de uma pessoa muito pequena numa voz muito grave de uma pessoa muito grande.


## Have fun!
Best regards, <br>
João Nuno Carvalho <br>


