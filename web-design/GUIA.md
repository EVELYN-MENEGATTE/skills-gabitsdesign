# Guia: para que serve cada skill e quando usar

Regra geral: **uma skill principal por etapa**. Várias skills fazem coisas parecidas; carregar muitas ao mesmo tempo faz as regras brigarem (uma pede ousadia, outra pede contenção). Use a principal da etapa e deixe as outras de reserva.

## O fluxo

```
1. Direção  →  2. Criar  →  3. Polir  →  4. Revisar
```

### 1. Direção (antes de qualquer código)

| Skill | Para que serve | Quando usar |
|---|---|---|
| **UI UX Pro Max** | Base de dados pesquisável de estilos, paletas, pares de fontes, guidelines de UX, ícones e gráficos. | No início, para escolher estilo, paleta e fontes pelo ramo do cliente. Trate como consulta, não como regra. |
| **Anti UI Slop** | Obriga a definir o "contrato" da tela (público, tarefa principal, estados) e tem um portão final que barra UI genérica. | Telas de app e produto. Em landing, o Hallmark já cobre esse papel. |

### 2. Criar

| Skill | Para que serve | Quando usar |
|---|---|---|
| **Hallmark** | Páginas novas que parecem desenhadas, não geradas. Vem com lint (`sloplint`) que aponta padrões de IA. | **Principal para site ou landing de cliente.** Em design já existente, só chamando pelo nome: `/hallmark redesign <pasta>` ou `/hallmark audit <pasta>`. |
| **Taste Skill** | Sites de empresa com copy de voz própria, um sistema visual, uma seção por tela. | Site institucional em que a marca e o texto pesam mais que tudo. |
| **Impeccable** | Design, redesign, crítica e polimento de qualquer frontend, incluindo dashboards e design system. | **Principal para app, painel ou dashboard.** Também serve para redesenhar algo existente. |
| **Stageshow** | UI falsa de produto com cara de real, estática ou animada com cursor (janelas, celulares, terminais, bento grids). | Só para o mockup do produto no hero, card de feature ou demo animada. |
| **Frontend Design** (Anthropic) | Direção estética geral para não cair no template. | Reserva. Hallmark e Taste cobrem o mesmo com mais profundidade. |

### 3. Polir

| Skill | Para que serve | Quando usar |
|---|---|---|
| **Make Interfaces Feel Better** | Detalhes que fazem a interface parecer cuidada: sombras, bordas, raio, alinhamento óptico, números tabulares, ícones, animações de entrada e saída. | Depois que a página está montada e "parece estranha" sem saber por quê. |
| **Emil Design Eng** | Interações: press e hover, popovers, tooltips, transições, drag. | Só quando há interação de verdade (menus, modais, arrastar). Em landing estática quase não tem uso. |

### 4. Revisar antes de entregar

| Skill | Para que serve | Quando usar |
|---|---|---|
| **Tapa de UX** | 70 verificações de UX em 10 assuntos, cada uma com fonte. Em português. | **Revisão principal.** Ótima para justificar ajustes ao cliente. Dispara sozinha com "revisa essa tela". |
| **Web Design Guidelines** (Vercel) | Checagem técnica do código contra boas práticas de interface e acessibilidade. | Revisão rápida do código antes de publicar. |

## Resumo de bolso

| Trabalho | Criar | Revisar |
|---|---|---|
| Landing ou site de cliente | Hallmark | Tapa de UX + Make Interfaces Feel Better |
| Site com foco em marca e texto | Taste Skill | Tapa de UX |
| App, painel ou dashboard | Anti UI Slop → Impeccable | Tapa de UX + Web Design Guidelines |
| Componente com animação | Emil Design Eng | Make Interfaces Feel Better |
| Mockup ou demo do produto | Stageshow | — |

## Como chamar

- **Automático:** pedidos como "cria uma landing" ou "revisa essa tela" já puxam a skill certa na maioria das vezes.
- **Garantido:** cite o nome no pedido, por exemplo "usa o hallmark e cria…" ou "roda o tapa de ux nessa tela".
- **Comandos:** algumas aceitam barra, como `/hallmark audit <pasta>` e `/impeccable`.
