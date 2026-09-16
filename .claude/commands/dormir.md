---
description: Fecha a sessão deste repo e avisa o Segundo Cérebro (~/Cerebro) — sem a Liv copiar nada
allowed-tools: Read, Write, Edit, Bash(git add*), Bash(git commit*), Bash(git status*), Bash(git log*), Bash(python3 *), Bash(bash *)
---
Encerre a sessão deste repositório gravando em DOIS lugares, nesta ordem:

**1. Aqui no repo (como sempre):** atualize o arquivo de status deste projeto (STATUS.md ou o que o CLAUDE.md indicar) e o bloco de sessão no CLAUDE.md, no formato que este repo já usa. Depois `git add -A && git commit -m "docs: fecha a sessão AAAA-MM-DD — <resumo curto>"`. Se houver arquivos de trabalho sem commit, inclua-os — trabalho sem commit é trabalho sem backup. NUNCA commite `.env`, chaves ou senhas.

**2. No Segundo Cérebro (`~/Cerebro`)** — é a recepção que enxerga todos os projetos:
- Rode `bash ~/Cerebro/scripts/backup.sh dormir-<nome-do-repo>`.
- Em `~/Cerebro/orion/STATUS.md` (ou o andar indicado no CLAUDE.md deste repo): atualize a linha desta sala na tabela "Estado atual" (estado, data, 1 frase) e, se esta sala for a mais urgente, o `proximo_passo` do cabeçalho YAML e a data `atualizado`.
- Em `~/Cerebro/orion/pendencias.md`: marque `[x]` o que foi resolvido nesta sessão e adicione o que ficou pendente no formato `- [ ] AAAA-MM-DD | [Sala] texto` (data = prazo, opcional).
- Se a Liv te corrigiu nesta sessão, adicione a lição em `~/Cerebro/LICOES.md` (`- [data] [orion] lição`).
- Rode `python3 ~/Cerebro/scripts/gerar-indice.py` e `git -C ~/Cerebro add -A && git -C ~/Cerebro commit -m "dormir: <sala> AAAA-MM-DD"`.

**3. Responda** com: 5 tópicos do que foi feito + parágrafo de até 5 linhas "Contexto para o próximo chat".
$ARGUMENTS
