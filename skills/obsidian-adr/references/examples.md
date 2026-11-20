# Exemplo de decisão sobre prática

Uma equipe de estúdio considera a revisão por outra pessoa antes de integrar código. Neste exemplo fictício, o motivo da escolha fica em `08-Decisions/00-ADRs/01-Development-and-AI/ADR-NNNN-Review-Code-Before-Merge.md`. O procedimento pertence ao fluxo de engenharia responsável.

```yaml
identificador: ADR-NNNN
titulo: Revisar código antes da integração
tipo_de_decisao: adoção
estado: proposto
temas:
- revisao-de-codigo
- qualidade
tags:
- adrs
```

Na nota real, substituir `ADR-NNNN` pelo próximo identificador disponível e preencher a data e os responsáveis confirmados. O exemplo não aprova uma prática nem estabelece um identificador ou uma data reais.

## Contexto e definição do problema

A equipe quer reduzir problemas que poderiam ser percebidos por outra pessoa antes de integrar mudanças. O contexto deve vir de ocorrências ou objetivos realmente informados.

## Decisão e justificativa

A proposta é adotar revisão por outra pessoa para acrescentar uma avaliação independente da implementação e compartilhar conhecimento. Essas razões precisam ser confirmadas antes de registrar aceitação.

## Consequências

A revisão pode identificar problemas e distribuir conhecimento, mas exige disponibilidade e tempo de outra pessoa. Não há garantia de eliminar falhas.

## Aplicação

Critérios da revisão, responsáveis, comandos, tratamento de comentários e condições de integração ficam no procedimento correspondente. O ADR aponta para esse documento quando existir, sem duplicar suas regras.

Uma escolha de terminal para uso pessoal segue o mesmo esquema e fica em `08-Decisions/00-ADRs/00-Systems-and-Environments/`.
