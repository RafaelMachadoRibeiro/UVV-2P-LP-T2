# Descrição do Sistema - Jogo da Velha

O sistema desenvolvido em Python tem como objetivo permitir que um jogador humano jogue o tradicional Jogo da Velha contra um bot. O tabuleiro é representado por uma matriz 3x3, e o sistema implementa as regras básicas para verificar vitórias, empates e alternância de jogadas entre o usuário e o bot. O bot faz movimentos aleatórios, com um nível básico de inteligência, bloqueando jogadas que poderiam levar à vitória do usuário.

## Funcionalidades

### Jogada do Jogador Humano:
- O sistema solicita ao usuário que escolha uma linha e uma coluna no tabuleiro para fazer sua jogada. 
- O sistema valida as entradas, garantindo que o jogador selecione posições válidas e não ocupadas.

### Jogada do Bot:
- O bot faz suas jogadas automaticamente, primeiro verificando se o jogador humano está prestes a vencer e, se necessário, bloqueando essa jogada. 
- Caso contrário, ele faz uma jogada aleatória em uma célula disponível no tabuleiro.

### Verificação de Vitória:
- Após cada jogada, o sistema verifica se algum dos jogadores (humano ou bot) formou uma linha, coluna ou diagonal completa com seu símbolo ('X' ou 'O'), declarando o vencedor se isso ocorrer.

### Verificação de Empate:
- Caso todas as células do tabuleiro estejam preenchidas sem que haja um vencedor, o sistema detecta um empate e encerra a partida.

### Exibição do Tabuleiro:
- Após cada jogada, o tabuleiro é exibido com as posições ocupadas pelos jogadores, permitindo que o usuário acompanhe o progresso da partida.

### Alternância de Turnos:
- O sistema alterna automaticamente entre o jogador humano e o bot, mantendo a ordem correta de jogadas até que haja um vencedor ou um empate.

## Lógica do Bot
O bot implementado possui duas estratégias principais:

- **Defesa**: Caso detecte que o jogador humano pode vencer na próxima jogada, o bot faz o movimento necessário para bloquear essa vitória.
- **Jogada Aleatória**: Se não houver necessidade de defesa, o bot faz uma jogada aleatória em qualquer célula vazia do tabuleiro.

## Exemplo de Execução

Durante a execução do sistema, foram realizadas as seguintes operações:

1. O jogador humano escolheu uma célula, e a jogada foi realizada no tabuleiro.
2. O bot, em seguida, fez uma jogada, bloqueando uma possível vitória do jogador humano ou ocupando uma posição aleatória.
3. Após cada jogada, o sistema verificou se houve vitória ou empate.
4. O jogo continuou até que um vencedor fosse declarado ou que houvesse empate.

Essas operações demonstram que o sistema gerencia corretamente as jogadas, verifica as condições de vitória e empate, e permite que o jogador humano enfrente um bot com comportamento básico de defesa e jogadas aleatórias.
