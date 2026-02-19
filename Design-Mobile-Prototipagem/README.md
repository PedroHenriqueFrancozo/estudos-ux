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