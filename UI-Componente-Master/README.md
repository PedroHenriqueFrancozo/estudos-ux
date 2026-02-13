# 💎 Figma: Componentes Master e Instâncias
Os componentes são elementos que podem ser reutilizados em todo o seu design. Eles ajudam a manter a consistência e tornam a atualização do projeto muito mais rápida.

### 1. O que é o Componente Master (Main Component)?
É a "matriz" ou o componente original. Qualquer alteração feita nele (cor, tamanho, fonte) será replicada automaticamente em todas as cópias.

- **Como criar:** Selecione um objeto e clique no ícone de quatro diamantes no menu superior (ou use o atalho `Ctrl + Alt + K` / `Cmd + Option + K`).
- **Identificação:** No painel de camadas, o Master é representado por um ícone de **4 diamantes preenchidos**.

### 2. O que são Instâncias (Instances)?
São as cópias do componente Master. Elas estão "conectadas" ao pai, mas permitem algumas alterações pontuais (chamadas de Overrides).

- **Como criar:** Basta copiar o Master (`Ctrl + C` / `Ctrl + V`) ou arrastar do painel de Assets.
- **Identificação:** No painel de camadas, a instância é representada por um ícone de 1 diamante vazado.

### 3. O conceito de Overrides (Sobreposições)
Você pode alterar algumas propriedades em uma **Instância** sem desconectá-la do Master:

- **O que você PODE mudar:** Texto (conteúdo), Cor de preenchimento, Efeitos (sombra).
- **O que você NÃO DEVE mudar (para não quebrar a lógica):** Posição dos elementos internos ou estrutura básica.
- **Reset:** Se você se arrepender, pode clicar com o botão direito na instância e selecionar "Reset all changes" para ela voltar a ser idêntica ao Master.

### 4. Por que usar Componentes?

- **Eficiência:** Precisa mudar a cor de 50 botões? Mude apenas no Master.
- **Consistência:** Garante que todos os botões, ícones e inputs tenham o mesmo estilo.
- **Organização:** Todos os seus componentes ficam salvos na aba Assets, prontos para serem arrastados para qualquer tela.

# 💡 Dica: "Go to Main Component"
Se estiver editando uma tela e precisar mudar o Master que está escondido em outro lugar, basta selecionar a instância e clicar no ícone de diamante no painel direito (ou botão direito > Go to main component). O Figma te leva direto para a matriz.