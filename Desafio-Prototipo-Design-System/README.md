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

### 3. Aplicação do Design System
- **Tipografia:** Uso consistente da família Roboto, conforme definido no guia de estilos.
- **Cores Neutras:** Aplicação das cores #0F172A (Neutro Dark) e #FFFFFF (Neutro Light) para garantir alto contraste e legibilidade.

# ⚓ Seção: Footer (Rodapé)
O rodapé foi projetado para oferecer uma visão sistêmica do site, agrupando links por categorias e fornecendo informações legais obrigatórias.

### 1. Estrutura de Navegação em Colunas
Utilizei uma organização em blocos verticais para facilitar o escaneamento visual:

- **Branding:** Espaço dedicado ao Logo da empresa, acompanhado de um texto descritivo de **16px** (#2E2E2E) e ícones sociais para reforço de marca.
- **Colunas de Links** (Sobre e Comunidade):
    - **Títulos:** **20px** na cor #0F172A (Neutro Dark) para garantir destaque.
    - **Links:** Estruturados para direcionar o usuário a páginas institucionais (Parcerias, Blog, Convide um amigo).
- **Social:** Coluna dedicada aos canais oficiais (Instagram, Facebook e LinkedIn) com links diretos.

### 2. Hierarquia Tipográfica e Cores
- **Títulos das Colunas:** 20px Bold/Medium para criar uma separação clara entre as seções.
- **Corpo do Texto:** 16px Regular, garantindo que o rodapé não compita visualmente com o conteúdo principal da página, mas permaneça legível.
- **Paleta:** Uso das cores #0F172A para o texto principal e títulos, mantendo a consistência com o restante do projeto.

### 3. Rodapé Legal (Bottom Bar)
- **Copyright:** Texto de **16px** informando a propriedade intelectual.
- **Informações Legais:** Links para "Política de Privacidade" e "Termos e Condições" em 20px **Regular**, posicionados estrategicamente para fácil acesso conforme as normas de conformidade digital.

# 🔐 Seção: Tela de Login e Autenticação
O design da tela de login foi estruturado para ser limpo e funcional, minimizando distrações para o usuário no momento da autenticação.

### 1. Composição Visual (Split Screen)
- **Layout:** Utilização de uma área de destaque de **704px x 924px** dedicada a uma imagem aspiracional ou ilustrativa, equilibrando o peso visual com o formulário de entrada.
- **Navbar:** Integração da barra de navegação superior para permitir que o usuário retorne à Home ou acesse outras áreas antes de logar.

### 2. Formulário de Acesso (Input Fields)
Os campos de entrada foram desenhados com foco em clareza e affordance:

- **Título:** "Faça seu login" em 24px Bold, estabelecendo a hierarquia imediata.
- **Campos (E-mail e Senha):** Dimensões: 300px x 44px.
    - Identificadores: Uso de ícones (E-mail e Trava) para suporte visual.
    - Placeholder: Texto em **18px** na cor #CACACA, indicando claramente o que deve ser preenchido.
- **Botão Entrar (CTA):** * Dimensões: 200px x 39px com **Border Radius de 8px.**

### 3. Links de Suporte (Acessibilidade e Fluxo)
Para garantir que o usuário não fique "preso", foram adicionados links de recuperação e cadastro:

- **Links:** "Esqueci minha senha" e "Criar conta".
- **Estilização:** **12px Regular**, posicionados estrategicamente abaixo do botão principal para não competir visualmente, mas estarem disponíveis quando necessários.

# 📝 Seção: Tela de Cadastro (Sign Up)
A tela de cadastro foi projetada para capturar dados de forma organizada, utilizando componentes resilientes para garantir uma experiência de preenchimento fluida.

### 1. Arquitetura do Formulário Inteligente
- **Container Principal:** Um frame de **396px x 676px** utilizando **Auto Layout** e configurado como **Componente Master**. Isso garante que qualquer ajuste de espaçamento ou estilo de input seja replicado instantaneamente.
- **Hierarquia de Texto:** Título em **24px Bold** e Subtítulo em **20px Regular**, fornecendo as instruções iniciais de forma clara.

### 2. Campos de Entrada (Inputs)
O formulário conta com 5 campos estratégicos (Nome, Telefone, E-mail, Senha e Confirmação), todos padronizados:

- **Dimensões:** 300px x 44px.
- **Identidade Visual:** Ícones representativos para cada categoria e texto de placeholder na cor #CACACA.
- **Segurança:** Inclusão do campo de "Confirmação de Senha" para reduzir erros de digitação no primeiro acesso.

### 3. Ações e Conversão (CTA)
- **Botão Principal:** "Criar minha conta" com **270px x 39px**, utilizando a cor **Verde** da marca para atrair o clique e reforçar a ação positiva.
- **Legal e Conformidade:** Abaixo do botão, foi inserido o texto de "Políticas de Privacidade" e "Termos de Uso".
    - **Destaque:** Links na cor verde com **underline**, seguindo padrões de acessibilidade para elementos clicáveis.

### 4. Fluxo de Alternância
- **Link de Login:** Texto de suporte para usuários que já possuem conta, facilitando a transição para a tela de Login através de um link destacado em verde, melhorando a navegabilidade.

# 📖 Seção: Tela "Sobre Nós" e Storytelling Visual
Esta tela foi projetada para transmitir autoridade e os valores da marca, utilizando uma composição equilibrada entre grandes ativos visuais e blocos de texto informativos.

### 1. Header e Proposta de Valor
- **Título de Impacto:** Utilização de um Heading robusto de **56px** ("Soluções inteligentes para o seu dia a dia").
- **Apoio Textual:** Texto descritivo em **18px**, seguindo o padrão de legibilidade do Design System para o corpo de texto.
- **Ativo Visual:** Espaço dedicado para imagem de destaque no lado direito (**688px x 503px**), criando um equilíbrio assimétrico moderno.

### 2. Seção "Nossa Jornada"
Focada na narrativa histórica da empresa:

- **Título da Seção:** **48px** na cor #0F172A (Neutro Dark), garantindo hierarquia clara.
- **Composição:** Texto posicionado à direita para uma leitura fluida, seguido por um grande banner visual de **1280px x 738px**, ideal para fotos de equipe ou infraestrutura.

### 3. "O Que Nos Move" e "Nossa Visão"
Estruturação de blocos de conteúdo intercalados (Z-pattern) para manter o engajamento do usuário:

- **Layout:** Em um frame amplo de **1440px x 1024px**, os textos e imagens alternam posições, guiando o olhar através dos pilares da empresa.