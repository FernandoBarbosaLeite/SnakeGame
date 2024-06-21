# 2-Player Snake Game

## Estruturas:
### Tile:

Atributos:
- `int x`: posição X do tile.
- `int y`: posição Y do tile.

### SnakeGame:

Atributos:
- `int boardWidth`: largura do tabuleiro.
- `int boardHeight`: altura do tabuleiro.
- `int tileSize`: tamanho do tile (25 por padrão).
- `Tile snakeHeadOne`: cabeça da Snake One.
- `ArrayList<Tile> snakeBodyOne`: corpo da Snake One.
- `Tile snakeHeadTwo`: cabeça da Snake Two.
- `ArrayList<Tile> snakeBodyTwo`: corpo da Snake Two.
- `Tile food`: posição da comida.
- `Random random`: gerador de posições aleatórias para a comida.
- `Timer gameLoop`: loop do jogo que controla a taxa de atualização.
- `int velocityOneX`: velocidade X da Snake One.
- `int velocityOneY`: velocidade Y da Snake One.
- `int velocityTwoX`: velocidade X da Snake Two.
- `int velocityTwoY`: velocidade Y da Snake Two.
- `boolean snakeOneDies`: indicador de morte da Snake One.
- `boolean snakeTwoDies`: indicador de morte da Snake Two.
- `boolean tie`: indicador de empate.

## Funções:
### App.main(String[] args):

Descrição: Inicializa a aplicação, configurando a janela do jogo e iniciando o SnakeGame.  
Parâmetros: `String[] args` - argumentos de linha de comando.  
Retorno: N/A

### SnakeGame.SnakeGame(int boardWidth, int boardHeight):

Descrição: Construtor da classe SnakeGame, inicializa o tabuleiro, as cobras, a comida e o loop do jogo.  
Parâmetros:
- `int boardWidth` - largura do tabuleiro.
- `int boardHeight` - altura do tabuleiro.  
Retorno: N/A

### SnakeGame.paintComponent(Graphics g):

Descrição: Método de desenho que chama o método draw para renderizar o jogo.  
Parâmetros: `Graphics g` - contexto gráfico.  
Retorno: N/A

### SnakeGame.draw(Graphics g):

Descrição: Desenha o tabuleiro, as cobras, a comida e as mensagens de fim de jogo.  
Parâmetros: `Graphics g` - contexto gráfico.  
Retorno: N/A

### SnakeGame.placeFood():

Descrição: Define uma nova posição aleatória para a comida no tabuleiro.  
Parâmetros: N/A  
Retorno: N/A

### SnakeGame.collision(Tile tile1, Tile tile2):

Descrição: Verifica se dois tiles colidiram (mesma posição).  
Parâmetros:
- `Tile tile1` - primeiro tile.
- `Tile tile2` - segundo tile.  
Retorno: `boolean` - true se os tiles colidiram, caso contrário false.

### SnakeGame.moveOne():

Descrição: Movimenta a Snake One, trata colisões e verifica condições de morte.  
Parâmetros: N/A  
Retorno: N/A

### SnakeGame.moveTwo():

Descrição: Movimenta a Snake Two, trata colisões e verifica condições de morte.  
Parâmetros: N/A  
Retorno: N/A

### SnakeGame.actionPerformed(ActionEvent e):

Descrição: Atualiza o estado do jogo a cada intervalo de tempo do timer.  
Parâmetros:
- `ActionEvent e` - evento de ação do timer.  
Retorno: N/A

### SnakeGame.keyPressed(KeyEvent e):

Descrição: Lida com a entrada do teclado para controlar as cobras.  
Parâmetros:
- `KeyEvent e` - evento de tecla pressionada.  
Retorno: N/A

### SnakeGame.keyTyped(KeyEvent e):

Descrição: Método necessário pela interface KeyListener, mas não utilizado.  
Parâmetros:
- `KeyEvent e` - evento de tecla digitada.  
Retorno: N/A

### SnakeGame.keyReleased(KeyEvent e):

Descrição: Método necessário pela interface KeyListener, mas não utilizado.  
Parâmetros:
- `KeyEvent e` - evento de tecla liberada.  
Retorno: N/A

## Fluxo do Programa:

O programa inicia a aplicação, configurando a janela e inicializando o SnakeGame. O loop do jogo é controlado por um `Timer`, que atualiza o estado do jogo a cada intervalo. Os jogadores controlam as cobras usando o teclado, com as seguintes teclas:

- **Jogador 1 (Snake Verde)**:
  - `W`: mover para cima.
  - `S`: mover para baixo.
  - `A`: mover para a esquerda.
  - `D`: mover para a direita.

- **Jogador 2 (Snake Azul)**:
  - `↑`: mover para cima.
  - `↓`: mover para baixo.
  - `←`: mover para a esquerda.
  - `→`: mover para a direita.

O jogo termina quando uma cobra colide com uma parede, seu próprio corpo ou o corpo da outra cobra. Mensagens de fim de jogo são exibidas indicando o vencedor ou se houve empate.

## Considerações Adicionais:

- **Verificações de entrada**: O jogo garante que os movimentos não causem colisões inválidas.
- **Interface de usuário**: Implementada usando Java Swing, proporcionando uma interação gráfica simples e eficaz.
- **Efeitos sonoros**: Sons são tocados ao comer comida e ao fim do jogo para melhorar a experiência do usuário.

---

Enjoy playing the 2-Player Snake Game! If you encounter any issues or have suggestions, feel free to open an issue on the GitHub repository. Happy gaming!
