# Revisão de ADRs

A revisão verifica se o leitor consegue compreender por que a escolha foi feita. Não inserir esta lista no ADR.

## Justificativa

- A necessidade e a função escolhida estão explícitas e sustentadas pelo contexto?
- As razões são atribuídas aos responsáveis, distinguindo expectativa de observação?
- As alternativas e os motivos de rejeição foram realmente informados?
- Benefícios, custos, dependências e riscos ajudam a compreender as contrapartidas?

## Limites do documento

- O ADR explica uma adoção, abandono, substituição ou consolidação?
- Procedimentos, regras operacionais e listas de execução estão em práticas, contextos, projetos ou fluxos adequados?
- A aceitação continua distinta de implementação verificada?
- Se a escolha é um método, existe referência à sua aplicação quando disponível, sem inventar um procedimento aprovado?

## Integridade

- O registro está em uma única subpasta de `08-Decisions/00-ADRs/` pelo assunto principal e os assuntos transversais estão em `temas`?
- `tipo_de_decisao`, `estado`, `temas`, identificador e responsáveis estão coerentes?
- Identificadores históricos, datas, origem e escopo de substituição foram preservados?
- O identificador é único na coleção e coincide com o início do nome do arquivo e com o título?
- O `README.md` da categoria aponta para o ADR e os links afetados resolvem para os caminhos atuais?
- Uma refatoração preservou a justificativa e as contrapartidas, sem transformar escolha histórica em decisão nova?

Corrigir questões editoriais sustentadas pelo material existente. Perguntar por fatos materiais ausentes, sem inventá-los. Relatar a revisão fora do ADR.
