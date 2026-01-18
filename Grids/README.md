# 📐 Grids (Grelhas)

A Grid é um sistema de linhas horizontais e verticais que serve como esqueleto para organizar o conteúdo de forma consistente e estruturada em uma interface.

# 🧩 Anatomia de uma Grid

- **Colunas (Columns):** As seções verticais que dividem a tela. No desktop, o padrão comum é usar 12 colunas.
- **Calhas (Gutters):** Os espaços vazios entre as colunas. Elas impedem que o conteúdo de uma coluna "encoste" na outra.
- **Margens (Margins):** O espaço entre as bordas da tela e o conteúdo.
- **Módulos:** Os blocos individuais criados pelo cruzamento de linhas e colunas.

# 📱 Grid Responsiva

A grid permite que o layout se adapte a diferentes tamanhos de tela:

- **Desktop:** Geralmente 12 colunas.
- **Tablet:** Geralmente 8 colunas.
- **Mobile:** Geralmente 4 colunas.

# 💡 Por que usar?

- **1. Consistência:** Garante que todos os elementos sigam a mesma regra de alinhamento.
- **2. Velocidade:** Facilita a tomada de decisão sobre onde colocar um botão ou imagem.
- **3. Colaboração:** Ajuda o desenvolvedor a entender o espaçamento exato na hora de codar.

# 🌊 Grid Fixa vs. Grid Fluida (Líquida)
Existem duas formas principais de como as colunas se comportam ao redimensionar a tela:

- 1. Grid Fixa (Fixed)

As colunas possuem uma largura exata em pixels (ex: 80px).

- **Como funciona:** Quando a tela aumenta, as colunas continuam do mesmo tamanho, e o que sobra vira "espaço em branco" nas margens.
- **Uso:** Comum em sites que querem manter um controle rígido sobre o tamanho das imagens e blocos.

- 2. Grid Fluida ou Líquida (Fluid)

As colunas são definidas por porcentagens (%) em vez de pixels.

- **Como funciona:** As colunas esticam ou encolhem para preencher o espaço disponível da tela. Se a tela aumenta, a coluna aumenta junto.
- **Uso:** Essencial para o design moderno e responsivo, garantindo que o site ocupe bem todo o espaço de qualquer monitor.

# 📏 O Sistema de 8pt

A maioria dos Designers de Interface utiliza o Sistema de 8 pontos. Isso significa que todos os espaçamentos (paddings, margins, alturas de botões) devem ser múltiplos de 8 (8, 16, 24, 32, 40...).

  - Por que 8? Porque a maioria das telas modernas tem resoluções que são divisíveis por 8, evitando que os elementos fiquem com "meio pixel" e pareçam borrados.