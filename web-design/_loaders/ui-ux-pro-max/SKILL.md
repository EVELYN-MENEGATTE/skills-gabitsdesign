---
name: ui-ux-pro-max
description: Inteligência de UI/UX com base de dados pesquisável de estilos, paletas, pares de fontes, guidelines de UX, ícones, gráficos e stacks. Use ao desenhar, construir, revisar ou corrigir interfaces web, mobile ou desktop e design systems.
---

# UI UX Pro Max

Esta skill carrega a versão completa de **UI UX Pro Max** direto do GitHub (nextlevelbuilder/ui-ux-pro-max-skill), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/ui-ux-pro-max
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-ui-ux-pro-max && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/nextlevelbuilder/ui-ux-pro-max-skill /tmp/skills/_src-ui-ux-pro-max \
    && git -C /tmp/skills/_src-ui-ux-pro-max sparse-checkout set --no-cone '/.claude/skills/ui-ux-pro-max/**' \
    && ln -sfn /tmp/skills/_src-ui-ux-pro-max/.claude/skills/ui-ux-pro-max "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/ui-ux-pro-max` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
