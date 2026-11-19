# LOG

## 2026-11-19 10:30 (America/Sao_Paulo) — criação do repo e da pasta web-design

**O que foi feito**
- Criado o repositório `skills-gabitsdesign` com a pasta `web-design/`.
- Baixadas as 10 skills da lista "10 skills that kill AI slop" a partir dos repositórios oficiais (clone raso do branch padrão) e copiadas sem alterações:
  - `anti-ui-slop` ← uizze/uizze @ fc401e9 (uizze.com redireciona em loop; a skill oficial fica no GitHub da UIZZE)
  - `impeccable` ← pbakaus/impeccable @ b49177d (versão `.claude/skills/impeccable`, v4.10.0)
  - `taste-skill` ← Leonxlnx/taste-skill @ f6b7657 (tasteskill 2.5.1, nome interno `design-taste-frontend`)
  - `emil-design-eng` ← emilkowalski/skills @ 64eb3de (só a skill principal; o repo tem outras 19 de animação)
  - `web-design-guidelines` ← vercel-labs/agent-skills @ 1a2c79d
  - `frontend-design` ← anthropics/skills @ e4bb5d9
  - `hallmark` ← Nutlope/hallmark @ 04977e1 (v2.0.0)
  - `make-interfaces-feel-better` ← jakubkrehel/make-interfaces-feel-better @ 6d9f2f1
  - `ui-ux-pro-max` ← nextlevelbuilder/ui-ux-pro-max-skill @ 2de1134
  - `stageshow` ← benjitaylor/skills @ 299140f (v1.1.1)
- Onde a pasta da skill não trazia licença, copiada a licença do repo original como `LICENSE.upstream`.
- Criada `web-design/_loaders/` com 7 SKILL.md carregadores (anti-ui-slop, design-taste-frontend, emil-design-eng, hallmark, make-interfaces-feel-better, ui-ux-pro-max, stageshow). Cada um baixa a skill completa do GitHub para `/tmp/skills/<nome>` e segue o original. Testados: os 7 baixaram com sucesso.
- Instalação no Claude (claude.ai): propostas as 7 skills que ainda não existiam na conta. Já instaladas antes e não duplicadas: impeccable, frontend-design, web-design-guidelines.

**Arquivos criados**
- `README.md`, `LOG.md`
- `web-design/README.md` (tabela com fonte, commit e licença)
- `web-design/<10 pastas de skill>/**` (2.365 arquivos no total, ~57 MB; maior pasta: taste-skill, 40 MB)
- `web-design/_loaders/<7 pastas>/SKILL.md`

## 2026-11-19 10:22 (America/Sao_Paulo) — adicionada a skill tapa-de-ux

**O que foi feito**
- Adicionada `web-design/tapa-de-ux/` ← othiagopinheiro/tapa-de-ux @ 555bd87, versão em português (`plugins/tapa-de-ux/skills/tapa-de-ux`). 70 verificações de UX em 10 assuntos, cada uma com fonte. Licença CC-BY-4.0 (atribuição a Thiago Pinheiro).
- Não incluída a versão em inglês (`tapa-de-ux-en`): o próprio autor recomenda instalar uma língua só, para a revisão não aparecer duplicada.
- Instalação no Claude: enviado o ZIP oficial do autor (`dist/tapa-de-ux.zip`) para upload direto em Customize → Skills, com todas as regras embutidas (sem precisar baixar do GitHub na hora do uso).

**Arquivos alterados**
- Criados: `web-design/tapa-de-ux/SKILL.md`, `web-design/tapa-de-ux/LICENSE.txt`, `web-design/tapa-de-ux/regras/*.md` (10 arquivos)
- Editados: `web-design/README.md` (nova linha na tabela, contagem 10 → 11), `README.md` (contagem), `LOG.md`

## 2026-11-19 10:24 (America/Sao_Paulo) — publicação no GitHub

**O que foi feito**
- Enviado o repositório local para `github.com/EVELYN-MENEGATTE/skills-gabitsdesign` (branch `main`, privado), com os commits 116478b e 196a597.
- A partir de agora, os loaders do Claude usam este repo como espelho quando o GitHub original falhar.

**Arquivos alterados**
- Editado: `LOG.md` (esta entrada)
