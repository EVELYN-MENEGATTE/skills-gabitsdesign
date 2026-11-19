---
name: anti-ui-slop
description: Impede UI genérica de IA: contrato de design específico do produto, estados obrigatórios e um portão final antes de entregar. Use ao criar, redesenhar, revisar ou fazer review pré-entrega de telas web ou iOS, ou quando pedirem anti-ui-slop, stop UI slop ou UI finish gate.
---

# Anti UI Slop (UIZZE)

Esta skill carrega a versão completa de **Anti UI Slop (UIZZE)** direto do GitHub (uizze/uizze), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/anti-ui-slop
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-anti-ui-slop && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/uizze/uizze /tmp/skills/_src-anti-ui-slop \
    && git -C /tmp/skills/_src-anti-ui-slop sparse-checkout set --no-cone '/skills/anti-ui-slop/**' \
    && ln -sfn /tmp/skills/_src-anti-ui-slop/skills/anti-ui-slop "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/anti-ui-slop` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
