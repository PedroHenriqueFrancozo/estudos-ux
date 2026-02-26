# 🎨 Documentação: Design System

### 1. Tipografia (Typography)
A escolha da família tipográfica Roboto foca em uma interface moderna e funcional.

- **Base:** 1 rem = 16px.
- **Pesos utilizados:** Bold, Medium e Regular.
- **Hierarquia Visual:**
    - **Headings:** Escalonados de **H1 (48px)** até **H6 (18px)** para garantir uma clara distinção de seções.
    - **Subtitles:** Variações de 24px e 20px (Regular).
    - **Body:** Tamanhos de 18px e 16px, otimizados para leitura prolongada em diferentes densidades de tela.

# 2. Paleta de Cores (Colors)
O sistema de cores foi dividido em categorias funcionais para garantir consistência em toda a aplicação.

### 🟢 Cor Primária (Primary)
Composta por uma escala de 10 tons (do Darker ao Light), permitindo flexibilidade para estados de botões, fundos e destaques.

- **Main:** #059669 (Normal).
- **Variações:** Inclui tons para estados de hover e active (ex: #03A33F, #047854).

### ⚪ Neutras e Texto (Neutral & Text)

- **Neutrals:** Tons para superfícies e bordas, variando de #0F172A (Dark) até o branco puro #FFFFFF.
- **Text Colors:** Escala de cinzas ( #1A1A1A a #9E9EA6 ) para garantir contraste e acessibilidade na leitura.

# ⚠️ Cores Semânticas (Semantic/Other Colors)
Utilizadas para fornecer feedback visual imediato ao usuário:

- **Danger/Error:** #E60F0F (Vermelho).
- **Success:** #1DC560 (Verde).
- **Warning/Alert:** #FFB800 (Amarelo).
- **Info:** #0F9AE8 (Azul).

![Desing System](/assets/DesingSystemProjeto.png)

# 🏗️ Estrutura do Protótipo de Alta Fidelidade
O layout foi desenvolvido seguindo a metodologia de componentes reutilizáveis e layouts adaptáveis.

### 1. Navegação Principal (Navbar)

- **Estrutura:** Logo, Links de navegação (Home, Sobre nós, Contato) e botões de CTA (Criar conta, Entrar).
- **Técnica:** Componente Master com Auto Layout para garantir o espaçamento fixo entre os links e botões.
- **Visual:** Fundo verde #059669 com 60% de opacidade.

### 2. Seção Hero (Header)
O primeiro contato do usuário com o site foi desenhado para impacto e clareza:

- **Background:** #E6F5F0 (Verde menta muito claro), gerando um contraste suave com a Navbar.
- **Conteúdo:** * Imagem de destaque (618px x 517px).
    - **Hierarquia de Texto:** Título principal em 48px (Cor #0F172A - Azul quase preto) para máxima leitura e Subtítulo em 24px.
- **CTA Principal:** Botão "Saiba mais" (152px x 52px) em fundo branco, destacando-se sobre o fundo colorido da seção.

### 3. Seção de Serviços
Focada em apresentar os benefícios de forma organizada através de **Cards**:

- **Títulos de Seção:** Mantendo o padrão de 48px para o título e 24px para o subtítulo (Cor #2E2E2E para o texto secundário).
- **Cards de Serviço:** * Criados como Componente Master com Auto Layout.
    - **Hierarquia Interna:** Título do card (32px), área de imagem/ícone e descrição (18px Regular).
    - **Vantagem:** A alteração em um card (como o arredondamento das bordas ou cor do texto) é replicada instantaneamente em todos os outros.

# 📍 Seção: Venha nos Conhecer
Esta seção foi desenhada para facilitar a conversão através de duas ações principais: agendamento e localização.

### 1. Elementos de Texto e Hierarquia

- **Título Principal:** "Venha nos Conhecer" com 40px na cor #0F172A.
- **Subtítulo de Apoio:** 20px na cor #1A202C, reforçando a clareza da mensagem.
- **Subtítulos dos Cards:** 24px na cor #0F172A para destacar os tópicos "Agendamento" e "Local".
- **Corpo de Texto:** Tamanho 14px na cor #1A202C, garantindo que informações secundárias não briguem com os destaques.

### 2. Composição e Design Visual

- **Conectividade:** Utilização de uma linha curva entre os frames para guiar o olhar do usuário e simbolizar o fluxo entre o agendamento e a visita ao local.
- **Ícones:** Uso de ícones de calendário (agendamento) e alfinete (local) inseridos em formas arredondadas (shapes) com tons suaves de azul/cinza para manter o equilíbrio visual.
- **Botões (CTAs):** * Ambos os botões possuem fundo branco (#FFFFFF) e altura de 44px.
    - O botão de agendamento tem largura de **167px**, enquanto o do Google Maps tem **224px**, adaptando-se ao tamanho do texto interno.
- **Selo de Confiança:** Adição de um ícone de verificado com a cor de sucesso do sistema para transmitir segurança ao usuário.