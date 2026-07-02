# CLAUDE.md — Landing Page da Orion Voss

## Escopo deste projeto (LEIA PRIMEIRO)
- Este projeto é **somente uma landing page estática** da marca "Orion Voss".
- Trabalhe **apenas dentro desta pasta**. NÃO leia, modifique ou referencie nenhum outro
  projeto/pasta do computador (existe outro projeto "Rei" que NÃO pode ser tocado).
- NÃO crie backend, banco, API ou integração de servidor. A página é 100% estática.
- Entregável: um único `index.html` com CSS (e JS, se preciso) embutidos. Sem build,
  sem frameworks, sem dependências de servidor — para hospedar no EasyPanel.

## A marca: Orion Voss
Orion Voss é uma **psico-astróloga terapêutica que atende por WhatsApp**. A persona é uma
mulher (o rosto da marca) — as fotos dela estão na pasta `assets/` deste projeto.
Objetivo da página: **converter visitantes do Instagram em conversas no WhatsApp.**

## IDENTIDADE VISUAL (siga à risca)
Existe um mockup-referência. Reproduza essa estética premium e mística, NÃO uma versão genérica.

**Paleta:**
- Fundo escuro: azul-meia-noite / índigo profundo (aprox. `#0A0E24` a `#0B1026`).
- Acento principal: dourado/champagne (aprox. `#C9A35C` / `#D9BE84`).
- Seções claras: creme/marfim (aprox. `#F4ECDD`) com texto em azul-marinho escuro.
- Alterne o ritmo: seções escuras e seções claras se intercalando (igual ao mockup).

**Tipografia (Google Fonts):**
- Títulos: serifada elegante e fina — use **Cormorant Garamond** (ou Playfair Display).
- Corpo: sans-serif limpa — use **Montserrat** (ou Inter).
- Rótulos/botões: caixa-alta com bastante espaçamento entre letras (letter-spacing).

**Detalhes decorativos:**
- Linhas finas douradas de constelação, estrelas pequenas e lua crescente como ornamentos sutis (SVG inline, sem imagens externas).
- Muito espaço de respiro. Elegante, calmo, nada poluído.

## ASSETS (use os arquivos locais da pasta `assets/`)
Use as imagens reais da marca. Deixe um comentário claro no código em cada uso indicando
o nome do arquivo, pra eu trocar fácil. Nomes esperados (ajuste se os meus forem diferentes):
- `assets/logo-orion.png` — logo (dourado sobre transparente/escuro) — vai no topo (header).
- `assets/orion-hero.jpg` — foto principal da persona — vai no hero (lado direito/fundo).
- `assets/orion-sobre.jpg` — foto da persona — vai na seção "Sobre a Orion".
Se algum arquivo não existir, deixe um placeholder com fundo índigo e um comentário dizendo qual imagem colocar ali.

## ESTRUTURA DA PÁGINA (siga a ordem do mockup)
1. **Header** fixo/simples: logo "Orion" (lua + nome) no topo à esquerda.
2. **Hero** (escuro): título "ORION" grande em serifada dourada + "psico-astróloga" abaixo;
   a tagline; o parágrafo de apresentação; botão CTA grande "Começar minha jornada 🌙";
   selo "As primeiras conversas são por minha conta. 🌙"; foto da persona à direita.
3. **"O que é psico-astrologia"** (escuro): 2-3 frases — "É unir psicologia e astrologia de
   forma profunda e humana. A psique vem primeiro. O mapa mostra tendências, arquétipos e
   padrões que influenciam suas escolhas. Você continua escrevendo sua história." + um
   ornamento de lua/feminino.
4. **"Como funciona"** (escuro): 3 passos com ícone cada —
   (1) Você envia uma mensagem.
   (2) A Orion escuta sua história e parte da sua base: Sol · Lua · Ascendente.
   (3) Vocês caminham juntas, no seu tempo, com memória. Sem começar do zero.
5. **Faixa clara (creme)**: selo grande "As primeiras conversas são por minha conta. 🌙"
   + botão "Quero conhecer a Orion".
6. **"Sobre a Orion"** (escuro): foto + texto — "Quem conversa com você primeiro é a
   terapeuta. A astrologia é a linguagem que ajuda a psique a se compreender." + lista:
   • Formação em Psicologia
   • Aprofundamento em psicologia analítica, trauma, vínculos e desenvolvimento humano
   • Estudos em astrologia humanista
   • Acompanhamento contínuo, no ritmo e na realidade da sua vida
   Fecho: "Aqui, o céu não dita o futuro. Ele ajuda você a entender quem você é."
7. **"Diferenciais do acompanhamento"** (faixa): linha de ícones com legenda —
   Memória permanente · Conversa pelo WhatsApp · Processo contínuo · Base psicológica ·
   Astrologia humanista · No seu ritmo.
8. **"O que dizem sobre a Orion"** (claro): 3 depoimentos em cartões, cada um com texto,
   nome, cidade/UF e 5 estrelas. (Use depoimentos de exemplo, marcados como placeholder.)
9. **CTA final** (escuro): "Sua história merece mais do que uma leitura." + subtítulo
   "Merece presença, escuta e profundidade." + botão "Começar minha jornada 🌙".
10. **Rodapé**: "Orion · Método Animas" + links Instagram, WhatsApp, Política de Privacidade.

## TEXTOS OFICIAIS (use exatamente)
- **Tagline (hero):** "Seu mapa não prevê o futuro — ele mostra a base de quem você veio ser. O resto, a gente caminha junto."
- **Apresentação (hero):** "Converse com a Orion: uma psico-astróloga que escuta você antes de falar do céu. Ela parte da sua base — Sol, Lua, Ascendente — pra te ajudar a enxergar seus padrões e quem você está se tornando. Acompanhamento de verdade, no seu WhatsApp, no seu ritmo."
- **Selo:** "As primeiras conversas são por minha conta. 🌙"

## CALL TO ACTION
- Todos os botões apontam para o WhatsApp. Deixe um comentário claro no código onde trocar o número:
  `https://wa.me/55SEUNUMERO?text=Oi%20Orion%2C%20quero%20come%C3%A7ar%20minha%20jornada%20%F0%9F%8C%99`
- Texto do botão principal: **"Começar minha jornada 🌙"**

## MOBILE-FIRST
A maioria vem do Instagram no celular. Priorize o layout mobile (igual ao "preview mobile"
do mockup) e depois adapte pro desktop. Bom contraste e acessibilidade.

## MARKETING (preparar, não inventar)
- No `<head>`, deixe um espaço **comentado e sinalizado** para eu colar depois o Meta Pixel
  (Facebook). Só o placeholder com instrução — não invente um ID.

Quando terminar, me explique como abrir o `index.html` no navegador pra ver o resultado.
