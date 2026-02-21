# 📱 Design Mobile: Estruturas e Componentes

### 1. List View vs. Grid View
A escolha entre lista ou grade depende do tipo de conteúdo e do objetivo do usuário:

- List View (Modo Lista):
    - **Foco:** Texto e leitura (Padrão em F).
    - **Vantagem:** Permite escanear informações rapidamente sem distrações visuais. Ótimo para detalhes técnicos, nomes ou mensagens.

- Grid View (Modo Grade):
    - **Foco:** Imagens e exploração visual.
    - **Vantagem:** A atenção é distribuída. É ideal quando o usuário precisa escolher baseado na aparência (ex: e-commerce de roupas ou galeria de fotos).

### 2. Prática no Figma: Construindo a Interface

**Grid Layout e Espaçamento**

- **Configuração:** Uso de 2 colunas com **Margem e Respiro (Gutter)** de 16px.
- **Nota técnica:** 16px é o "padrão de ouro" do mobile, pois garante que os elementos não encostem na borda física do celular.

### O Poder do Auto Layout
o Auto Layout no botão "Conhecer".

- **Padding (Respiro):** 24px (lateral) e 12px (vertical).
- **Vantagem:** O botão se torna "elástico". Se você mudar o texto de "Conhecer" para "Saiba mais agora", o botão cresce sozinho mantendo as margens.

### Ergonomia e Área de Clique

- **Botão Home:** Adicionei um shape invisível para aumentar a área de clique.
- **Dica de UX:** A Apple e o Google recomendam uma área de toque mínima de **44x44px** ou **48x48px**, mesmo que o ícone seja menor. Isso evita que o usuário clique e "nada aconteça".

### Efeitos Visuais

- **Máscaras:** Uso de imagens sobre shapes para controle de bordas.
- **Sombra (Drop Shadow):** Aplicada na barra de navegação para criar **hierarquia visual** (elevação), indicando que a barra está "acima" do conteúdo que rola por baixo.

### Top Bar Inteligente

1. Estrutura da Top Bar
- Dimensões: 393px (largura total do device) por 72px (altura).
- Margens Internas: Uso padrão de 16px nas laterais para alinhar com o restante do conteúdo.
- Elementos: Avatar (Usuário), Título (Nome da tela/App) e Ícone (Menu/Notificações).
- Estilização de Elevação (Drop Shadow):
    - **Y:** 0.5 (deslocamento vertical mínimo para um efeito de linha fina).
    - **Blur (Desfoque):** 2 (suavização leve).
    - **Opacidade:** 16% (sombra discreta e profissional).
    - **Objetivo:** Criar separação visual entre o cabeçalho fixo e o conteúdo rolável da página.

### 2. Construção com Auto Layout (A forma inteligente)
Em vez de posicionar cada item manualmente sobre um retângulo, segui o fluxo:

1. **Seleção dos Itens:** Selecionei o Avatar + Título + Ícone.
2. **Aplicação do Auto Layout (`Shift + A`):** Isso cria um frame que envolve os três.
3. **Distribuição Espacial:** * Defini o alinhamento como Centralizado Verticalmente.
    - Altei o espaçamento entre os itens para **"Auto"** (ou usamos Space Between), fazendo com que o título fique no centro ou o avatar e ícone fiquem nas extremidades.
4. **Padding (Margens):** Adicionei os **16px** de preenchimento horizontal diretamente nas configurações do Auto Layout.
5. **Cor e Estilo:** Apliquei a cor principal diretamente no fundo deste frame.

### 3. Vantagens do Método Inteligente
- **Adaptabilidade:** Se mudar o tamanho da tela, a barra se ajusta automaticamente.
- **Consistência:** A margem de **16px** nunca será "quebrada" por erro humano ao arrastar um objeto.

# Menu de Pesquisa / Filtros Horizontais
A criação de menus roláveis permite que o usuário acesse várias categorias sem ocupar muito espaço vertical na tela.

### 1. Estilização e Hierarquia Visual
O uso de pesos e cores diferentes serve para indicar ao usuário qual item está **Ativo (Selecionado)** e quais estão **Inativos**.

- **Fonte:** Source Sans Pro (uma excelente escolha para legibilidade em telas).
- **Item Ativo:** Cor #2563EB, Peso `Black` (Máximo destaque).
- **Item Inativo:** Cor #BBCFF9, Peso Regular.
- **Espaçamento (Gap):** 4px entre os elementos do grupo.

### 2. Configuração de Scroll Horizontal (Protótipo)
Para que o menu deslize para os lados, é necessário configurar o "estouro" do conteúdo:

- **Frame de Recorte:** O frame pai deve ter a largura da tela (ex: 393px).
- **Clip Content:** Esta opção deve estar marcada para "esconder" os itens que passam da borda da tela.
- **Margem de Segurança:** O ajuste de `-16px` nas bordas garante que o clique do usuário não seja invalidado por estar colado no limite do frame, melhorando a precisão do toque.
- **Aba Prototype:** No campo Overflow Scrolling, define-se como Horizontal Scrolling.

### 3. Componente Master vs. Instância
- **O Componente Master** contém toda a lista esticada com todos os itens.
- A **Instância** dentro da tela do celular é que tem o tamanho reduzido e o scroll ativado. Isso mantém o design organizado e fácil de editar.

# 🎡 Construção de Carrossel de Cards
O carrossel é um elemento de alto impacto visual que combina imagens, informações de destaque e controles de interação.

### 1. Estrutura do Card de Imagem
- **Dimensões do Frame Principal:** 618px x 253px.
- **Técnica de Fundo:** Usei a imagem ocupando a área total.

### 2. O Painel de Informações (Overlay)
Criei um frame interno (335px x 90px) para garantir a legibilidade sobre a imagem:

- **Background:** Cor com 60% de opacidade. Esse efeito de "vidro" (glassmorphism leve) é essencial para que o texto não "suma" na foto de fundo.
- **Conteúdo Interno:** * Título do item.
    - Avaliação (Estrelas).
    - Botão de "Gostei" (Favoritar).
- **Organização:** Usei o Auto Layout aqui para manter o botão no final do frame e as estrelas alinhadas com o título.

# 🎡 Refinamento do Carrossel e Auto Layout Avançado

### 1. Painel de Informações Inteligente (Overlay)
A grande evolução aqui foi tornar o painel dinâmico em vez de estático.

- **Redimensionamento:** Uso do "Hug Contents" (Envolver conteúdo). Isso faz com que, se o título do item for maior ou tiver mais estrelas, o fundo (background) cresça automaticamente para acomodar tudo.
- **Contraste de Cor:** Para evitar que o texto fique transparente, a opacidade deve ser aplicada apenas no Fill (Preenchimento) do frame e não na Layer (Camada) global.
- **Blur (Opcional):** Para um efeito real de vidro, pode-se adicionar o efeito Background Blur nas configurações de Effects.

### 2. Hierarquia de Auto Layout (O segredo do Botão de Like)
Para conseguir o efeito de "espaço entre" os elementos (título de um lado e botão do outro), apliquei a técnica de **Aninhamento**:

- **Grupo A:** Auto Layout entre [Texto do Título + Estrelas de Avaliação].
- **Grupo B:** O Botão de Like.
- **Frame Pai:** Um Auto Layout englobando o **Grupo A** e o **Grupo B**.
- **Distribuição:** Configurado como "**Space Between**" (Espaço entre), o que "empurra" o título para a esquerda e o botão para a direita, independentemente da largura do card.

### 3. Prototipagem de Fluxo
- **Overflow Scrolling:** Configurado como Horizontal na aba Prototype.
- **Clip Content:** Ativado no frame pai (do tamanho da tela do celular) para esconder o restante do carrossel de 618px e permitir o deslize.

# 📑 Figma: Scroll Vertical e Elementos Fixos
A criação de listas verticais extensas requer atenção à hierarquia de camadas para que os elementos de navegação não "sumam" durante a rolagem.

### 1. Estrutura dos Cards Verticais
- **Dimensões:** 172px x 175px (proporção próxima ao quadrado).
- **Direcionamento:** Fluxo configurado para expansão vertical (Y-axis).
- **Componentização:** O card foi transformado em **Componente Master**, permitindo escalabilidade e manutenção rápida do design.

### 2. Painel de Informações (Overlay)
- **Dimensões:** 172px x 70px.
