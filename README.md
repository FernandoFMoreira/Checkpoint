# Checkpoint
Trabalho de programação para dispositivos móveis 2024-2

## Alunos
Fernando Favaro Moreira

## Visão geral
Jogo Checkpoint (inspirado no jogo de desktop Buckshot Roulette):
A visão do cenário é top-down (de cima para baixo / céu para chão).
Você é um oficial num ponto de checagem de um país, e precisa liberar a passagem apenas dos veículos do seu país (azuis) e mandar de volta os veículos do outro país (vermelhos).

 -O máximo de veículos possíveis é 10, sendo que veículos já na fila tem prioridade sobre os enviados pelo checkpoint do outro país*, e os veículos que chegam de fora tem prioridade sobre os que já estão na fila, com a prioridade ficando: Enviados pelo outro checkpoint* < Dentro da fila < Fora do país. (* Referem-se ao modo de multiplayer local, portanto não são consideradas no modo singleplayer)  
 -Cada veículo vermelho que entra é um erro cometido por você.  
 -Para saber qual é a cor do veículo, você precisa usar dos seus auxílios, que recebe X aleatórios a cada rodada.  
 -Ganha quem não cometer erros o bastante para ser demitido*. (Dinâmica de multiplayer local, provavelmente não será implementada nessa primeira entrega) (Em modo singleplayer, existe apenas a mecânica de recorde local)  
### Auxílios (exemplos desse jogo e sua contraparte no jogo que serviu de inspiração):
 -Espelho: Permite que você veja o veículo na frente da fila; (lupa)  
 -Relatório de erros: Corrije até 3 erros que você cometeu, sendo o mais provável: 3 < 2 < 1; (remédio vencido)  
 -Informante: Informa ao jogador a posição e cor de algum veículo na fila; (Telefone)  

## Usuários
Jogador: Decide se o veículo na fila passa pelo ponto de checagem ou volta de onde ele veio, usando de auxílios do seu inventário, auxílios esses que o mesmo recebe em X quantidade a cada início de turno

## Requisitos funcionais
 -Banco de dados (funcional ou não-funcional) para recordes de jogador;  
 -Mecanismo de aleatoriedade de quantidade de veículos e a cor de cada um (azul ou vermelho);  
 -Controle de "vidas" do jogador (chamadas de "erros" dentro do jogo);  
 -Mecanismo de aleatoriedade dos auxílios a serem dados ao jogador a cada início de turno.  
