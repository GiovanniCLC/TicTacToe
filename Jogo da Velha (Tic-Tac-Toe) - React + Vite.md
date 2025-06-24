# Jogo da Velha (Tic-Tac-Toe) - React + Vite

Um jogo da velha interativo e moderno desenvolvido com React e Vite, apresentando uma interface visual atrativa e funcionalidades completas.

## 📋 Objetivo do Projeto

Este projeto implementa um jogo da velha clássico com as seguintes características:

- **Interface moderna e responsiva** com design gradiente e animações suaves
- **Lógica completa do jogo** incluindo detecção de vitória e empate
- **Sistema de histórico** permitindo navegar entre jogadas anteriores
- **Alternância automática de jogadores** (X e O)
- **Feedback visual** claro sobre o estado do jogo

## 🚀 Como Rodar o Projeto

### Pré-requisitos

- Node.js (versão LTS recomendada)
- npm ou yarn

### Instalação e Execução

1. **Clone ou baixe o projeto**
   ```bash
   # Se usando git
   git clone <url-do-repositorio>
   cd jogo-da-velha
   ```

2. **Instale as dependências**
   ```bash
   npm install
   ```

3. **Execute o projeto em modo de desenvolvimento**
   ```bash
   npm run dev
   ```

4. **Acesse o jogo**
   - Abra seu navegador
   - Navegue para `http://localhost:5173`
   - O jogo estará pronto para uso!

### Comandos Disponíveis

- `npm run dev` - Inicia o servidor de desenvolvimento
- `npm run build` - Gera a versão de produção
- `npm run preview` - Visualiza a versão de produção localmente

## 🎮 Como Jogar

### Regras Básicas

1. **Objetivo**: Seja o primeiro a formar uma linha de três símbolos iguais
2. **Jogadores**: Dois jogadores se alternam (X sempre começa)
3. **Vitória**: Forme uma linha horizontal, vertical ou diagonal
4. **Empate**: Quando todas as casas estão preenchidas sem vencedor

### Controles

- **Clique nas células**: Para fazer uma jogada
- **Botões do histórico**: Para voltar a jogadas anteriores
- **"Ir para o início do jogo"**: Reinicia o jogo completamente

### Funcionalidades Especiais

#### Sistema de Histórico
- Cada jogada é salva automaticamente
- Clique em qualquer botão do histórico para voltar àquela jogada
- Continue jogando a partir de qualquer ponto anterior
- O histórico é preservado durante toda a sessão

#### Interface Responsiva
- Funciona perfeitamente em desktop e mobile
- Design adaptativo que se ajusta a diferentes tamanhos de tela
- Animações suaves e feedback visual

#### Detecção Inteligente
- **Vitória**: O jogo detecta automaticamente quando um jogador vence
- **Empate**: Identifica situações de empate
- **Jogadas inválidas**: Impede cliques em células já ocupadas

## 🛠️ Tecnologias Utilizadas

### Frontend
- **React 18** - Biblioteca para construção da interface
- **Vite** - Ferramenta de build rápida e moderna
- **CSS3** - Estilização com gradientes e animações
- **JavaScript ES6+** - Lógica moderna e funcional

### Estrutura do Projeto

```
jogo-da-velha/
├── src/
│   ├── App.jsx          # Componente principal
│   ├── App.css          # Estilos principais
│   ├── Game.jsx         # Lógica principal do jogo
│   ├── Board.jsx        # Componente do tabuleiro
│   ├── Square.jsx       # Componente de cada célula
│   └── main.jsx         # Ponto de entrada
├── public/              # Arquivos estáticos
├── package.json         # Dependências e scripts
└── README.md           # Este arquivo
```

### Componentes

#### Game (Jogo Principal)
- Gerencia o estado global do jogo
- Controla o histórico de jogadas
- Implementa a navegação entre jogadas

#### Board (Tabuleiro)
- Renderiza o tabuleiro 3x3
- Gerencia cliques nas células
- Exibe o status atual do jogo
- Implementa a lógica de vitória

#### Square (Célula)
- Representa cada célula individual
- Exibe X, O ou vazio
- Responde a cliques do usuário

## 🎨 Design e Estilização

### Características Visuais

- **Gradiente de fundo**: Roxo/azul moderno
- **Cartão central**: Fundo branco translúcido com blur
- **Células coloridas**: Bordas em cores diferentes para cada célula
- **Animações**: Hover effects e transições suaves
- **Tipografia**: Fonte moderna e legível

### Responsividade

- **Desktop**: Layout otimizado para telas grandes
- **Tablet**: Ajustes de tamanho e espaçamento
- **Mobile**: Interface compacta e touch-friendly

## 🧪 Testes Realizados

O projeto foi testado extensivamente para garantir funcionamento correto:

### Funcionalidades Testadas

✅ **Alternância de jogadores** - X e O se alternam corretamente  
✅ **Detecção de vitória** - Todas as combinações vencedoras funcionam  
✅ **Detecção de empate** - Identifica quando não há mais jogadas  
✅ **Sistema de histórico** - Navegação entre jogadas funciona perfeitamente  
✅ **Interface responsiva** - Funciona em diferentes tamanhos de tela  
✅ **Validação de jogadas** - Impede jogadas inválidas  

### Cenários de Teste

- Vitória em linhas horizontais (1-2-3, 4-5-6, 7-8-9)
- Vitória em linhas verticais (1-4-7, 2-5-8, 3-6-9)
- Vitória em diagonais (1-5-9, 3-5-7)
- Situações de empate
- Navegação pelo histórico
- Reinício do jogo

## 📱 Compatibilidade

### Navegadores Suportados
- Chrome (recomendado)
- Firefox
- Safari
- Edge

### Dispositivos
- Desktop (Windows, macOS, Linux)
- Tablets (iOS, Android)
- Smartphones (iOS, Android)

## 🔧 Desenvolvimento

### Estrutura de Código

O código segue boas práticas de React:

- **Componentes funcionais** com hooks
- **Estado gerenciado** com useState
- **Props drilling** controlado
- **Separação de responsabilidades** clara

### Lógica de Vitória

```javascript
const lines = [
  [0, 1, 2], [3, 4, 5], [6, 7, 8], // Horizontais
  [0, 3, 6], [1, 4, 7], [2, 5, 8], // Verticais
  [0, 4, 8], [2, 4, 6]             // Diagonais
];
```

### Sistema de Histórico

- Array de estados do tabuleiro
- Índice da jogada atual
- Navegação bidirecional

## 📄 Licença

Este projeto é de código aberto e pode ser usado livremente para fins educacionais e pessoais.

## 👨‍💻 Desenvolvimento

Projeto desenvolvido seguindo as melhores práticas de React e design moderno, implementando todas as funcionalidades solicitadas com foco na experiência do usuário.

---

**Divirta-se jogando! 🎮**

