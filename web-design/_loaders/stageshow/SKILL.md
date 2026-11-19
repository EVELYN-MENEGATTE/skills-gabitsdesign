---
name: stageshow
description: Cria UI falsa de produto com cara de real, estática ou animada com cursor: janelas de browser e app, dashboards, celulares, notificações, terminais, bento grids. Use para hero ou card de feature com mockup do app, demo de produto ou walkthrough animado. React e CSS.
---

# Stageshow (Benji Taylor)

Esta skill carrega a versão completa de **Stageshow (Benji Taylor)** direto do GitHub (benjitaylor/skills), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/stageshow
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-stageshow && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/benjitaylor/skills /tmp/skills/_src-stageshow \
    && git -C /tmp/skills/_src-stageshow sparse-checkout set --no-cone '/stageshow/**' \
    && ln -sfn /tmp/skills/_src-stageshow/stageshow "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/stageshow` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
