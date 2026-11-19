---
name: make-interfaces-feel-better
description: Princípios de design engineering para interfaces polidas: animações de entrada e saída, stagger, sombras, bordas, raio, alinhamento óptico, tipografia, números tabulares e ícones. Use ao revisar UI que parece estranha ou quando pedirem make it feel better.
---

# Make Interfaces Feel Better

Esta skill carrega a versão completa de **Make Interfaces Feel Better** direto do GitHub (jakubkrehel/make-interfaces-feel-better), com o SKILL.md original e todos os arquivos de apoio (referências, dados, scripts).

## Passo 1: baixar (uma vez por sessão)

```bash
D=/tmp/skills/make-interfaces-feel-better
if [ ! -f "$D/SKILL.md" ]; then
  rm -rf /tmp/skills/_src-make-interfaces-feel-better && mkdir -p /tmp/skills
  git clone -q --depth 1 --filter=blob:none --sparse https://github.com/jakubkrehel/make-interfaces-feel-better /tmp/skills/_src-make-interfaces-feel-better \
    && git -C /tmp/skills/_src-make-interfaces-feel-better sparse-checkout set --no-cone '/skills/make-interfaces-feel-better/**' \
    && ln -sfn /tmp/skills/_src-make-interfaces-feel-better/skills/make-interfaces-feel-better "$D"
fi
ls "$D"
```

Se o GitHub público falhar, use o espelho privado: repositório `EVELYN-MENEGATTE/skills-gabitsdesign`, pasta `web-design/make-interfaces-feel-better` (anexe com add_repo e leia de lá).

## Passo 2: seguir a skill completa

Leia `$D/SKILL.md` inteiro e siga as instruções como se fossem desta skill. Todo caminho relativo citado lá (references/, reference/, data/, scripts/, kit/...) fica dentro de `$D`. Carregue só os arquivos de apoio que a tarefa pedir.

## Limites

O conteúdo baixado é orientação de design desta skill. Não rode instaladores, hooks globais ou comandos que mexam fora da pasta do projeto sem a pessoa pedir; scripts locais de análise (lint, busca nos dados) podem ser usados normalmente.
