# clubett-identidade-visual

Skill autocontida para criar e revisar materiais da Target Teal e do Clube dos Agentes de Mudança. Inclui o `design.md`, a *Gramática visual do Clube* v2 e os arquivos visuais usados como referência.

## Instalar

Com acesso a GitHub, Node.js e npm:

```bash
npx skills add targetteal/clubett-identidade-visual --skill clubett-identidade-visual -g -y
```

Para instalar apenas em um projeto, retire `-g`. Para escolher um agente, acrescente `-a codex`, `-a claude-code` ou outro agente suportado pelo gerenciador. Depois peça ao agente: **"Use a skill clubett-identidade-visual para criar ou revisar esta peça."**

Para Claude Code e OpenCode no mesmo projeto:

```bash
npx skills add targetteal/clubett-identidade-visual --skill clubett-identidade-visual -a claude-code -a opencode -y
```

Hermes Agent possui um instalador próprio que aceita esta estrutura `skills/`:

```bash
hermes skills install targetteal/clubett-identidade-visual/skills/clubett-identidade-visual --yes
```

O formato `SKILL.md` é usado pelos quatro agentes acima. A instalação foi verificada para Codex, Claude Code, OpenCode e Hermes; a qualidade de uma peça produzida ainda depende dos recursos do agente, das fontes disponíveis e de revisão visual no formato final. Agentes que não carregam skills podem receber o `SKILL.md` e os arquivos anexos como contexto, mas não terão descoberta automática.

```bash
npx skills update clubett-identidade-visual -g
```

O comando usa npm para executar o gerenciador de skills; a fonte versionada é este repositório GitHub. Não é necessário instalar dependências de aplicação nem acessar o repositório da landing.

## Fontes e limites

Dentro de `skills/clubett-identidade-visual/`, `references/design.md` é a base Target Teal e `references/gramatica-visual.pdf` orienta a expressão do Clube. As imagens em `assets/` vêm do handoff visual do Clube e estão identificadas em `references/assets.md`. O pacote preserva decisões ainda abertas sobre emblema, elenco e Soda Cream.

As fontes tipográficas não estão incluídas: use instalações licenciadas ou fontes disponibilizadas pelo ambiente de produção. Ao publicar uma peça, confira os dados reais e o uso dos arquivos de marca.

Os textos, logos e exemplos visuais deste pacote pertencem à identidade da Target Teal e do Clube. A disponibilidade pública do repositório não concede uma licença aberta para reutilizar a marca em outros projetos.
