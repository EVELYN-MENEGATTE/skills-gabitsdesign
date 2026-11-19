---
name: hallmark
description: Skill de design para sites e páginas novas que parecem desenhados, não gerados. Use ao construir algo novo ou quando citarem Hallmark; em design existente só com /hallmark redesign <path> ou /hallmark audit <path>.
---

# Hallmark

Esta skill carrega a versão completa de **Hallmark** direto do GitHub (Nutlope/hallmark), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/hallmark
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-hallmark && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/Nutlope/hallmark /tmp/skills/_src-hallmark \
    && git -C /tmp/skills/_src-hallmark sparse-checkout set --no-cone '/skills/hallmark/**' \
    && ln -sfn /tmp/skills/_src-hallmark/skills/hallmark "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/hallmark` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
