# Convenções de ADRs

## Localização e assunto

No layout `08-Decisions/00-ADRs/`, guardar cada ADR em uma única subpasta conforme o assunto principal da escolha. Consultar `08-Decisions/00-ADRs/README.md` para localizar os índices das categorias.

| Assunto | Subpasta de `08-Decisions/00-ADRs/` |
| --- | --- |
| Sistemas operacionais, interfaces gráficas e ferramentas de terminal | `00-Systems-and-Environments/` |
| Desenvolvimento de software, agentes e aprendizado profissional | `01-Development-and-AI/` |
| Hospedagem, redes, contêineres, monitoramento e bancos de dados | `02-Infrastructure-and-Data/` |
| Conhecimento, comunicação, navegação, credenciais, arquivos e conteúdo pessoal | `03-Productivity-and-Communication/` |
| Bancos, crédito, contratos, transporte e serviços de consumo | `04-Finance-and-Services/` |

Usar `temas` para assuntos secundários e links para referenciar o mesmo ADR em projetos, práticas e outros contextos. A justificativa de um método fica na categoria do assunto a que ele se aplica. A aplicação fica no documento operacional responsável. Quando existir, consultar o índice de padrões técnicos do vault, como `11-Notes/05-Technical-Standards/Practice Index.md`.

## Metadados

| Propriedade | Conteúdo |
| --- | --- |
| `identificador` | Identidade estável do ADR |
| `titulo` | Escolha descrita em português |
| `tipo_de_decisao` | `adoção`, `abandono`, `substituição` ou `consolidação` |
| `estado` | Situação da decisão, sem confundir com execução |
| `data` | Data do registro ou da decisão, conforme sua origem; não inventar |
| `atualizado` | Data de revisão editorial quando registrada; não substitui datas históricas |
| `responsaveis_pela_decisao` | Lista dos responsáveis confirmados |
| `temas` | Lista de assuntos transversais, como terminal, privacidade ou contratos |
| `tags` | Tags existentes pertinentes; incluir `adrs` |

Preservar propriedades herdadas, como `data_original`, `implementacao`, `substitui`, `substituido_por` e os campos de substituição parcial. Não transformar uma substituição parcial em revogação integral.

## Tipo de decisão

- `adoção`: introdução de uma ferramenta ou prática.
- `abandono`: interrupção do uso sem sucessor para a função.
- `substituição`: troca de um arranjo por outro.
- `consolidação`: reunião de vários arranjos em uma solução comum.

A categoria acompanha o assunto principal e `tipo_de_decisao` registra a natureza da mudança. Preservar tipo, estado e identidade durante uma reorganização editorial.

## Identificadores e nomes

Preservar integralmente identificadores históricos como `ADR-adopt-0001`, `ADR-replace-0002` e `ADR-replacement-0014`, mesmo com palavras em inglês ou números coincidentes em séries diferentes.

Para um novo registro, consultar os valores de `identificador` em todas as subpastas de `08-Decisions/00-ADRs/`, incluindo séries históricas. Somar um ao maior sufixo numérico encontrado, preencher com zeros à esquerda até quatro dígitos e usar o formato `ADR-NNNN`. Conferir se o identificador e o caminho estão disponíveis antes de gravar.

Usar o identificador no título principal, nos metadados e no início do nome do arquivo. Nomear o arquivo `<identificador>-<Short-English-Title>.md`, com nomes próprios e siglas preservados. Manter o título e o conteúdo da nota em português.

## Ciclo de vida

Usar `proposto`, `aceito`, `rejeitado`, `descontinuado` ou `substituído por ADR-...`, preservando estados históricos. Proposta não é aceitação; aceitação não comprova instalação, migração ou execução.

Ao registrar substituição confirmada, manter as referências entre os registros anterior e sucessor, com escopo explícito quando parcial. Não modificar datas de aceitação por causa de uma reorganização documental.

## Manutenção da coleção

- No `README.md` da categoria, manter um wikilink para o ADR na seção **Registros**, com identificador e título como rótulo. Se a entrada exibir estado ou resumo, atualizar esses dados quando o ADR mudar.
- Ao mover um ADR, retirar a entrada da categoria anterior, incluí-la na nova e conferir os links de entrada e saída. Verificar também mapas e consultas que referenciem o caminho. Preservar o identificador, os metadados históricos e o vínculo com os ADRs relacionados.
- Quando uma alteração autorizada modificar as categorias, atualizar `08-Decisions/00-ADRs/README.md` e o mapa de pastas do vault, como `00-AI/00-Vault/CODEBASE.md`. Usar o próximo prefixo disponível na coleção para uma nova subpasta e dar a ela um `README.md` com finalidade e registros.

## Conteúdo

Contexto, decisão e justificativa, consequências e alternativas conhecidas formam o núcleo. Histórico e razões de reconsideração entram quando úteis. Instruções operacionais ficam em seus documentos próprios. Em outros repositórios, seguir as convenções do projeto.
