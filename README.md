# 🎯 Jogo do Número Secreto

Um jogo interativo desenvolvido em JavaScript onde o jogador deve adivinhar um número secreto entre 1 e 10. O jogo inclui recursos de acessibilidade com síntese de voz e feedback dinâmico para o usuário.

## 🎮 Como Jogar

1. O sistema gera aleatoriamente um número secreto entre 1 e 10
2. Digite seu palpite no campo de entrada
3. Clique no botão para verificar seu chute
4. Receba dicas se o número é maior ou menor que seu palpite
5. Continue tentando até acertar o número secreto
6. Após acertar, você pode reiniciar o jogo para uma nova partida

## ✨ Funcionalidades

- **Geração de números aleatórios únicos**: O sistema evita repetir números já sorteados em sequência
- **Contador de tentativas**: Acompanha quantas tentativas você fez para descobrir o número
- **Feedback dinâmico**: Informa se o número secreto é maior ou menor que seu palpite
- **Síntese de voz**: Utiliza a biblioteca ResponsiveVoice para narrar as mensagens em português brasileiro
- **Interface responsiva**: Atualização automática dos textos na tela conforme o progresso do jogo
- **Sistema de reinicialização**: Possibilidade de começar uma nova partida a qualquer momento

## 🛠️ Tecnologias Utilizadas

- **JavaScript ES6+**
- **HTML DOM Manipulation**
- **ResponsiveVoice.js** (para síntese de voz)
- **Math.random()** (para geração de números aleatórios)

## 📋 Estrutura do Código

### Principais Funções

- `exibirTextoNaTela()`: Atualiza elementos HTML e reproduz áudio
- `verificarChute()`: Processa o palpite do jogador e fornece feedback
- `gerarNumeroAleatorio()`: Gera números únicos e gerencia a lista de números já sorteados
- `reiniciarJogo()`: Reseta o estado do jogo para uma nova partida
- `limparCampo()`: Limpa o campo de entrada após cada tentativa

### Variáveis Globais

- `listaDeNumerosSorteados`: Array que armazena números já utilizados
- `quantidadeDeNumerosSecretosMaximo`: Define o limite superior dos números (1-10)
- `numeroSecreto`: Armazena o número atual que deve ser adivinhado
- `tentativas`: Contador de tentativas do jogador

## 🎯 Lógica do Jogo

O jogo implementa um sistema inteligente que:

1. **Evita repetições**: Mantém uma lista de números já sorteados para garantir variedade
2. **Reset automático**: Quando todos os números possíveis foram utilizados, a lista é limpa
3. **Recursividade**: Usa recursão para garantir que números únicos sejam sempre gerados
4. **Feedback contextual**: Ajusta as mensagens baseadas no número de tentativas (singular/plural)

## 🔧 Configuração

Para usar este projeto, você precisará:

1. Um arquivo HTML com os elementos necessários:
   - Um elemento `<h1>` para o título
   - Um elemento `<p>` para as mensagens
   - Um `<input>` para os palpites do jogador
   - Um botão com id "reiniciar"

2. Incluir a biblioteca ResponsiveVoice:
   ```html
   <script src="https://code.responsivevoice.org/responsivevoice.js"></script>
   ```

3. Incluir o arquivo JavaScript com o código do jogo


## 📱 Acessibilidade

O jogo foi desenvolvido com foco na acessibilidade, incluindo:
- Síntese de voz em português brasileiro
- Feedback claro e imediato
- Interface simples e intuitiva
- Suporte para usuários com deficiência visual

---

## 🙋🏻 Autor 

- Desenvolvido por Mauricio Grass de Bronstein


Divirta-se jogando e testando sua intuição para descobrir o número secreto! 🎉
