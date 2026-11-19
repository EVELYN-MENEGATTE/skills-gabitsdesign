# web-design

11 skills para tirar a "cara de IA" de interfaces e sites. Cada pasta é a skill completa, copiada do repositório original (SKILL.md + referências, dados e scripts), sem alterações.

| Pasta | Skill | Fonte original | Commit | Licença |
|---|---|---|---|---|
| `anti-ui-slop/` | Anti UI Slop (UIZZE) | [uizze/uizze](https://github.com/uizze/uizze) `skills/anti-ui-slop` | fc401e9 | Apache-2.0 (ver LICENSE/NOTICE) |
| `impeccable/` | Impeccable | [pbakaus/impeccable](https://github.com/pbakaus/impeccable) `.claude/skills/impeccable` | b49177d | Apache-2.0 |
| `taste-skill/` | Taste Skill (`design-taste-frontend`) | [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) `skills/taste-skill` | f6b7657 | MIT |
| `emil-design-eng/` | Emil Design Engineering | [emilkowalski/skills](https://github.com/emilkowalski/skills) `skills/emil-design-eng` | 64eb3de | MIT |
| `web-design-guidelines/` | Vercel Web Design Guidelines | [vercel-labs/agent-skills](https://github.com/vercel-labs/agent-skills) `skills/web-design-guidelines` | 1a2c79d | ver repo original |
| `frontend-design/` | Frontend Design (Anthropic) | [anthropics/skills](https://github.com/anthropics/skills) `skills/frontend-design` | e4bb5d9 | ver LICENSE.txt |
| `hallmark/` | Hallmark | [Nutlope/hallmark](https://github.com/Nutlope/hallmark) `skills/hallmark` | 04977e1 | MIT |
| `make-interfaces-feel-better/` | Make Interfaces Feel Better | [jakubkrehel/make-interfaces-feel-better](https://github.com/jakubkrehel/make-interfaces-feel-better) | 6d9f2f1 | MIT |
| `ui-ux-pro-max/` | UI UX Pro Max | [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) `.claude/skills/ui-ux-pro-max` | 2de1134 | MIT |
| `stageshow/` | Stageshow (Benji Taylor) | [benjitaylor/skills](https://github.com/benjitaylor/skills) `stageshow` | 299140f | ver LICENSE na pasta |
| `tapa-de-ux/` | Tapa de UX (versão PT) | [othiagopinheiro/tapa-de-ux](https://github.com/othiagopinheiro/tapa-de-ux) `plugins/tapa-de-ux/skills/tapa-de-ux` | 555bd87 | CC-BY-4.0 |

## `_loaders/`

Versões "carregadoras" usadas para instalar no Claude (claude.ai): um SKILL.md curto que, ao ser usado, baixa a skill completa do GitHub para `/tmp/skills/<nome>` e segue o SKILL.md original. Assim referências, dados e scripts ficam disponíveis sem precisar subir dezenas de arquivos.

## Como usar em outro agente

- **Claude Code**: copie a pasta da skill para `~/.claude/skills/<nome>/` (ou `.claude/skills/` do projeto).
- **Codex / Cursor / outros**: copie para a pasta de skills do agente (ex.: `.agents/skills/`).

## Atualizar

Rode de novo o clone dos repositórios originais e substitua as pastas; anote o novo commit na tabela e no `LOG.md`.
