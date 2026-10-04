Você vai construir meu site de portfólio pessoal (Bruna Lopes, programadora backend)
seguindo o design que estou enviando em anexo. Trabalhe no repositório atual do
portfólio, aproveitando o que já existe e mantendo a semântica que já foi corrigida
(títulos em ordem, footer fora do main, lista de contatos).

OBJETIVO
Uma página única, estática, fiel ao design, que abra rápido para um recrutador.

LAYOUT (igual ao design)
- Lateral esquerda: foto de perfil redonda, nome, "Programadora · Backend",
  "Fortaleza, CE" e menu com âncoras (Sobre, Stack, Projetos, Contatos).
- Conteúdo à direita, nesta ordem: Sobre (caixa de destaque), Stack (círculos),
  Projetos (3 cards com imagem, título, descrição e tecnologias), Contatos e redes
  sociais (e-mail, LinkedIn, GitHub com ícones redondos).
- Responsivo: no celular a lateral vai para o topo e as seções empilham.
- Cores base: fundo #0f172a, lateral #0b1120, cartões #1e293b, bordas #334155,
  texto #e2e8f0, texto secundário #94a3b8, destaque #34d399.
- Fontes: IBM Plex Sans (texto) e IBM Plex Mono (rótulos e tecnologias).

STACK PREPARADA PARA CRESCER
- Hoje são 3 itens (Python/FastAPI, Java/Spring Boot, MySQL/Docker), mas vou
  adicionar mais.
- Cada item deve ser um único bloco de HTML repetível (um <li> dentro de uma <ul>).
- Use um grid que se ajusta sozinho (auto-fill com largura mínima), para que
  adicionar um item seja só copiar e colar um bloco, sem mexer em CSS nem em JS.
- Deixe um comentário no HTML mostrando onde e como adicionar um novo item.

BOTÃO DE TEMA
- Adicione um botão acessível (um <button> de verdade, com aria-label) que troca
  a cor de destaque do site entre: verde #34d399, azul #38bdf8, âmbar #fbbf24 e
  rosa #f472b6.
- Implemente com variáveis CSS e um atributo data-theme no <html>, de modo que
  cada tema seja um conjunto de variáveis. Assim dá para criar um tema claro
  depois sem refazer nada.
- Salve a escolha no localStorage (com try/catch) e aplique antes da página
  pintar, para não piscar a cor errada.
- Todas as cores de destaque do site devem vir da variável, nunca fixas.

DEPENDÊNCIAS
- Nenhuma dependência em tempo de execução: sem framework, sem biblioteca de
  ícones, sem jQuery.
- Troque o Tailwind por CDN pelo build com a CLI do Tailwind (dependência de
  desenvolvimento), gerando um único CSS minificado só com as classes usadas.
  Use a versão estável atual e confira a documentação oficial antes de instalar.
- Crie os scripts no package.json: "dev" (watch) e "build" (minificado).
- Mantenha node_modules no .gitignore.
- Ícones: SVG inline. JavaScript: um arquivo pequeno, vanilla, com defer.

DESEMPENHO
- Fontes: carregue só os pesos usados (400, 500, 600, 700 da Sans; 400 e 500 da
  Mono), com font-display: swap e preconnect; se possível, hospede os .woff2 no
  próprio projeto.
- Imagens em WebP, com width e height definidos, loading="lazy" nas capturas dos
  projetos e a foto de perfil em tamanho pequeno (no máximo 300 px).
- Sem animações pesadas e sem scripts de terceiros.
- Meta: nota 95 ou mais em Performance e Acessibilidade no Lighthouse (mobile).

CONTEÚDO
- Use os textos do design. Onde houver [sua foto], [captura de tela] e
  [SEU E-MAIL], mantenha um espaço reservado bem visível e não invente conteúdo.
- LinkedIn: https://linkedin.com/in/bruna-lopes-dev
- GitHub: https://github.com/Brunlps

COMO TRABALHAR
- Sou iniciante em frontend: faça em etapas pequenas e, ao fim de cada uma,
  explique em poucas linhas o que mudou e por quê.
- Antes de começar, liste as etapas que pretende seguir e espere meu ok.
- No final, entregue um relatório com: arquivos criados ou alterados, como rodar
  o projeto, como adicionar um item na Stack, como criar um novo tema e o
  resultado do Lighthouse.