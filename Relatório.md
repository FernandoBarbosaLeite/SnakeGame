# **Jogo Snake para 2 jogadores**
**Grupo: 20** *Fernando Barbosa Leite (14570458)*

# Relatório de Produção do Jogo 2-Player Snake

## 1) Requisitos

### 1.1. Funcionalidades do Jogo
- Implementação inicial de um jogo funcional de Snake para um único jogador.
- Adição de uma segunda cobra e ajustes nas interações entre as cobras.
- Integração de recursos estéticos, como mensagens de game over.
- Inclusão de efeitos sonoros para melhorar a experiência do usuário.

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
- Utilização do Eclipse como IDE principal.
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
