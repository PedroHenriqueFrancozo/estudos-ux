# 📋 Design System

### 📝 O que é?

É **um conjunto de padrões de componentes de design**, que visa a consistência visual e funcional de um ecossistema.

Pense no Design System como uma biblioteca de "peças de LEGO" padronizadas. Isso evita que, a cada nova página ou frame, você tenha que recriar componentes do zero, garantindo agilidade, padrão e organização ao projeto.

   - **O Design System é um organismo vivo:** Ele é definido no início do projeto, mas evolui e sofre modificações conforme as necessidades do produto e dos usuários mudam.

### 🔄️ Consistência do design

A consistência não é apenas na parte gráfica(visual). Ela se estende para:

- **Comportamento:** Animações e micro-interações.
- **Funcionalidade:** Ações que o usuário executa e como o sistema responde.

### 🏗️ Composição 

Um Design System robusto inclui:

- **Elementos Básicos:** Cores, tipografia (fontes), ícones e espaçamentos.
- **Componentes:** Botões, inputs, calendários, tabelas e gráficos.
- **Assets:** Imagens, ilustrações e animações (motions).

### 📖 Guia de Estilo (Guideline)

É um conjunto de diretrizes da marca. Ele detalha o esquema de cores, as propriedades das fontes e as regras de aplicação de cada elemento para auxiliar na execução e garantir a identidade visual. que pode incluir elementos de interface do usuário. Esquema de cores, fontes  e suas propriedades para auxiliar na execução e uso.

### ⚡ Estados dos Componentes

Para garantir uma boa usabilidade, os componentes devem comunicar visualmente seu estado atual:
- **Padrão (Default):** O estado inicial do componente.
- **Hover (Ao passar o mouse):** Indica que o elemento é interativo.
- **Ativo/Pressionado (Active):** O momento do clique ou toque.
- **Selecionado (Selected):** Quando o item foi escolhido (ex: uma aba ou checkbox).
- **Inativo (Disabled):** Quando a ação não está disponível no momento.
- **Foco (Focused):** Essencial para acessibilidade (navegação via teclado).

Estados de Feedback (Comunicação):
- **Alerta/Erro:** Indica que algo precisa de atenção ou deu errado.
- **Confirmação/Sucesso:** Indica que a ação foi concluída com êxito.
- **Notificação:** Um aviso visual de que há uma nova informação.

### ⚠️ Dica

**Design System não é um projeto (com início e fim); é um produto que serve outros produtos.**

---

# 🧩 Atomic Design for Streanloan

![Metodologia Atomic Design](/assets/atomic.png)

---

# 🖼️ Exemplo de um Design System

### 🖋️ Tipogradia
Define pesos, tamanhos e famílias de fontes para cada nível de informação (H1, H2, Body, etc).
![Escala tipográfica com definições de tamanhos e pesos de fontes](/assets/ex_Typography.png)

### 🎨 Paleta de Cores
Cores primárias, secundárias e neutras, com seus respectivos códigos HEX/RGB.
![Tabela de cores primárias, secundárias e neutras com códigos Hexadecimal](/assets/ex_Colors.png)

### 🔔 Notificações e Feedbacks
Padronização de avisos de erro, sucesso e alertas do sistema.
![Modelos de componentes para mensagens de erro, sucesso e alerta](/assets/ex_notification.png)

---

# ⚛️ Atomic Design

A **Atomic design** é uma metodologia criada por `Brad Frost em 2013`, para a criação de um Design System. Ela apresenta um paralelo entre a química e componentizção de elementos de interface.

Partindo do príncípio de que toda matéria é composta de átomos, e que essas unidades atômicas se organizam para formar estruturas mais complexas.

O Atomic Design é dividido em cinco níveis.

### Os Cinco Níveis do Design System

![Imagem sobre os cinco níveis do Design System](/assets/DesignSystem.png)

# Átomos

Em uma interface os menores elementos visuais seriam, por exemplo, label, field, button. Átomos também representam elementos mais abstratos, que podem ser chamados de tokens, como a paletas de cores, fontes, tamanho, espaçamento e etc.

Os Átomos são bons como referência no contexto de uma biblioteca de padrões, pois você pode ver todos os seus estilos rapidamente