---
name: design-taste-frontend
description: Taste Skill, skill anti-slop para sites de empresa no nível figma.com/x.ai: copy com voz própria, um sistema, uma seção por tela. Use ao construir landing pages ou sites institucionais novos, ou quando pedirem taste skill.
---

# Taste Skill (tasteskill)

Esta skill carrega a versão completa de **Taste Skill (tasteskill)** direto do GitHub (Leonxlnx/taste-skill), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/design-taste-frontend
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-design-taste-frontend && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/Leonxlnx/taste-skill /tmp/skills/_src-design-taste-frontend \
    && git -C /tmp/skills/_src-design-taste-frontend sparse-checkout set --no-cone '/skills/taste-skill/**' \
    && ln -sfn /tmp/skills/_src-design-taste-frontend/skills/taste-skill "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/taste-skill` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
