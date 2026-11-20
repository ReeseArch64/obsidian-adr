---
name: obsidian-adr
description: Criar, consultar, revisar e organizar registros de decisões arquiteturais (ADRs) em vaults Obsidian. Usar para documentar escolhas de ferramentas e práticas, manter categorias, identificadores e índices, ou registrar substituições.
---

# Registros de decisões arquiteturais

## Finalidade

Um ADR explica a necessidade, a escolha, as razões confirmadas, alternativas realmente consideradas e consequências aceitas. Ele preserva o motivo da decisão; aceitação não comprova implementação nem autoriza uma operação externa.

Procedimentos, permissões, proibições e listas de execução ficam nas práticas, contextos, projetos ou fluxos responsáveis. Referenciar esses documentos sem reproduzir suas instruções no ADR.

## Consultar e classificar

Localizar o índice de ADRs nas regras do vault. Em vaults com a estrutura `08-Decisions/00-ADRs/`, abrir `08-Decisions/00-ADRs/README.md` e seguir o índice da categoria pertinente. Ler os ADRs relacionados e verificar estado e substituições antes de propor um novo registro. Para escrever ou mover um ADR, seguir as [convenções](references/adr-conventions.md) de categoria, identificação e metadados. Consultar o mapa de pastas, como `00-AI/00-Vault/CODEBASE.md`, quando existir. Em outros layouts, seguir os caminhos e as convenções do vault.

## Registrar a intenção

Estabelecer necessidade, ferramenta ou prática escolhida, razões confirmadas e contrapartidas conhecidas. Para substituição, consolidação ou abandono, identificar o arranjo anterior e a função alterada. Perguntar apenas por lacunas materiais ainda não respondidas; não inventar comparações ou motivos de rejeição.

Uma nova decisão aceita exige confirmação da escolha e das razões. A autorização explícita já existente cobre o mesmo escopo; manutenção editorial não reabre decisões estabelecidas.

## Redigir e revisar

Usar o [modelo simples](assets/templates/adr-simple.md) para escolhas diretas e o [modelo comparativo](assets/templates/adr-madr.md) para alternativas efetivamente avaliadas. As [orientações de modelos](references/template-variants.md) e o [exemplo](references/examples.md) ajudam a escolher o nível de detalhe.

Nos vaults que seguem a convenção destes modelos, escrever em português brasileiro e usar nomes de arquivos e pastas em inglês. Preservar identificadores técnicos, nomes próprios e a autoria confirmada.

Revisar pelo [guia de revisão](references/review-checklist.md). Manter a revisão fora do ADR. Verificar referências, metadados, razões e consequências sem declarar testes que não ocorreram.

## Manter o histórico

- Preservar escolha, justificativa, identificador, datas do ciclo de vida, origem e relações de substituição em refatorações editoriais.
- Quando a decisão mudar, registrar a mudança confirmada e vincular os registros anterior e sucessor; não apagar a razão histórica.
- Ao criar, alterar ou mover um ADR, manter a navegação e as referências conforme as [convenções de manutenção](references/adr-conventions.md#manutenção-da-coleção).
- Preservar metadados históricos de implementação como declaração ou evidência qualificada; novos ADRs não exigem rastreamento de execução.
- Se houver material operacional a separar, preservar seu conteúdo e suas limitações no destino autorizado antes de removê-lo do ADR.

## Editar no Obsidian

Usar os modelos Markdown com a CLI do Obsidian quando ela estiver disponível, conforme as regras do vault. Ao gravar, conferir o frontmatter, os links e o índice da categoria afetada.
