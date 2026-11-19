---
name: emil-design-eng
description: Filosofia de design engineering do Emil Kowalski: polimento de UI, estados de press e hover, origem de popover, timing de tooltip, transitions vs keyframes, clip-path e detalhes de drag. Use ao construir ou revisar interações e polimento de componentes.
---

# Emil Kowalski Design Engineering

Esta skill carrega a versão completa de **Emil Kowalski Design Engineering** direto do GitHub (emilkowalski/skills), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/emil-design-eng
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-emil-design-eng && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/emilkowalski/skills /tmp/skills/_src-emil-design-eng \
    && git -C /tmp/skills/_src-emil-design-eng sparse-checkout set --no-cone '/skills/emil-design-eng/**' \
    && ln -sfn /tmp/skills/_src-emil-design-eng/skills/emil-design-eng "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/emil-design-eng` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
