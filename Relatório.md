# **Jogo Snake para 2 jogadores**
**Grupo: 20** *Fernando Barbosa Leite (14570458)*

# Relatório de Produção do Jogo 2-Player Snake

Objetivo: Desenvolver uma versão multiplayer do clássico jogo da Cobrinha. Este projeto permitirá que os estudantes combinem suas habilidades de programação em Java com técnicas de desenvolvimento de jogos para criar um ambiente de jogo interativo e competitivo.

## 1) Descrição da Tarefa:
Configuração do Projeto:
Criar um projeto que tenha como alvo plataformas desktop para facilitar a configuração e os testes.

Mecânicas do Jogo:
Implementar a jogabilidade clássica da Cobrinha, onde o jogador controla uma cobra que se move em uma grade, comendo comida para crescer.
Cada pedaço de comida comido aumenta o comprimento da cobra e a velocidade do jogo ligeiramente.
Incluir limites ou fazer com que as paredes não colidam, permitindo que a cobra passe por uma parede e saia pelo lado oposto.

Recursos Multiplayer:

Permitir que dois jogadores compitam na mesma tela, cada um controlando uma cobra com entradas do teclado.
Implementar a detecção de colisão entre as cobras, onde o jogo termina se uma cobra colidir consigo mesma ou com a outra cobra.
Rastrear e exibir a pontuação de cada jogador com base em quantos alimentos suas cobras consumiram.

Interface Gráfica:
Usar uma GUI para projetar uma interface dinâmica e visualmente atraente.

Melhorias e Som:
Adicionar efeitos sonoros para comer comida, colisão e outros eventos do jogo usando as capacidades de áudio do LibGDX.

Documentação e Testes:
Documentar as decisões de design, regras do jogo e processo de desenvolvimento.
Testar o jogo minuciosamente para garantir que as mecânicas sejam sólidas e que o jogo esteja livre de bugs.

Resultados Esperados:
Mecânicas de jogo em tempo real: Aprender sobre o gerenciamento de interações em tempo real e colisões em um jogo.


## 2) Descrição do Projeto

### Sistema de Jogo 2-Player Snake
O projeto foi desenvolvido em etapas progressivas para transformar um jogo tradicional de Snake em um jogo multiplayer com aprimoramentos estéticos e sonoros. Começamos com a implementação básica de uma cobra controlável, adicionamos uma segunda cobra com interações entre elas, incorporamos mensagens de game over para feedback visual, e finalmente, introduzimos efeitos sonoros para aumentar a imersão do jogador.

## 3) Comentários sobre o Código

### Estrutura do Projeto
O código está estruturado em diferentes pacotes:
- **GUI:** Contém classes para interface gráfica, como MainFrame, SnakePanel, GameOverDialog.
- **Model:** Inclui classes que representam as entidades do jogo, como Snake e GameBoard.
- **Utils:** Classes utilitárias para funções adicionais, como SoundPlayer e InputHandler.

### Principais Classes e Funcionalidades
- **MainFrame:** Janela principal que hospeda o jogo e gerencia os eventos principais.
- **SnakePanel:** Painel de jogo que exibe as cobras e os elementos do tabuleiro.
- **GameOverDialog:** Janela pop-up exibida ao final do jogo, mostrando o vencedor ou se houve empate.
- **SoundPlayer:** Classe responsável pela reprodução dos efeitos sonoros durante o jogo.
- **InputHandler:** Gerencia as entradas do teclado para movimentar as cobras.

### Melhorias Futuras
- Divisão da lógica de jogo em mais classes para melhorar a manutenibilidade.
- Implementação de níveis de dificuldade e opções de personalização para os jogadores.
- Integração com serviços online para rankings e competições multiplayer.

## 4) Plano e Resultados de Testes

### Procedimentos de Teste
- **Execução do Jogo:** Testar movimentação das cobras, colisões, crescimento e game over.
- **Testes de Interface:** Verificar interações com botões e eventos de teclado.
- **Testes de Som:** Assegurar que os efeitos sonoros estão sincronizados com as ações do jogo.

### Teste de Erros
- Simulação de colisões inesperadas entre cobras.
- Teste de limites de movimentação no tabuleiro.
- Validação de inputs inválidos e comportamentos de erro.

## 5) Procedimentos de Construção

### Compilação e Execução
- **Compilação via Terminal:**
  ```bash
  cd path/do/projeto
  javac -d bin src/*.java

### Execução via Terminal:
```
cd path/do/projeto/bin
java Main
```

### Ambiente de Desenvolvimento
- Utilização do IntelliJ como IDE principal.
- Instalação do plugin WindowBuilder para criação da interface gráfica.
- Gerenciamento de dependências com bibliotecas externas para efeitos sonoros e outras funcionalidades.

## 6) Problemas

### Desafios Encontrados
- Aprendizado inicial da lógica de jogo e da programação de interfaces gráficas.
- Gerenciamento de múltiplas interações de usuário em tempo real.
- Sincronização adequada dos elementos visuais e sonoros do jogo.

## 7) Comentários

### Conclusões e Considerações Finais
- O projeto proporcionou uma valiosa experiência de desenvolvimento de jogos e integração de elementos multimídia.
- A estrutura modular permitiu uma evolução gradual do jogo, facilitando a depuração e a adição de novos recursos.
- Recomenda-se a continuação do desenvolvimento com a inclusão de funcionalidades avançadas e otimizações de desempenho.
