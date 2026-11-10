#  Análise de Vendas | Power BI

## Dashboard interativo

Confira o painel desenvolvido no Power BI:

[📊 Acessar painel de vendas (arquivo PBIX)](./painel_de_vendas.pbix)



## Sobre o projeto

Este projeto foi desenvolvido durante um desafio prático da Educadados, mediado pelo professor Felipy Morais, com o objetivo de aplicar conhecimentos de modelagem de dados, criação de medidas DAX e construção de dashboards utilizando o Power BI.

A proposta foi explorar os dados de vendas, desenvolver indicadores e identificar comportamentos que pudessem contribuir para a compreensão dos resultados comerciais.

## Objetivos

- Importar e realizar o tratamento dos dados.
- Desenvolver a modelagem dimensional utilizando Star Schema.
- Criar relacionamentos entre tabelas fato e dimensão.
- Construir medidas utilizando DAX.
- Desenvolver indicadores de desempenho.
- Criar segmentações para análises dinâmicas.
- Identificar padrões e oportunidades por meio da análise dos dados.

## 🛠️ Ferramentas e tecnologias

- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Modelagem Dimensional (Star Schema)

## Modelagem de dados

Foi utilizada a modelagem dimensional Star Schema (Esquema Estrela), organizando a estrutura a partir de uma tabela fato central, relacionada às tabelas dimensão.

### Tabela fato
- fVendas

### Tabelas dimensão
- dProduto
- dLoja
- dCalendario

Essa estrutura permite organizar os dados e facilitar a construção das análises e dos indicadores.

## Medidas DAX

Foram desenvolvidas medidas utilizando as funções SUM, COUNTROWS e DIVIDE.

| Indicador | Expressão DAX |
|---|---|
| Faturamento | `SUM(fVendas[valor_liquido])` |
| Pedidos | `COUNTROWS(fVendas)` |
| Ticket médio | `DIVIDE([Faturamento], [Pedidos])` |
| Itens vendidos | `SUM(fVendas[quantidade])` |

## Dashboard

O relatório foi desenvolvido com segmentações e elementos visuais para permitir a exploração dos indicadores e a análise dos resultados por diferentes perspectivas.

<img width="1212" height="880" alt="image_1b03441f" src="https://github.com/user-attachments/assets/7e865fed-325f-418e-a34b-514dd87dfc89" />


## Principais insights identificados

### 1. Crescimento do faturamento

Em 2025, o faturamento alcançou R$ 11.008.216,68, representando um crescimento de R$ 2.145.940,67 em relação a 2023, equivalente a aproximadamente 24,21%.

### 2. Desempenho por categoria e região

Entre 2023 e 2025, a categoria de Informática apresentou destaque no faturamento, especialmente na região Sudeste.

### 3. Comportamento das vendas ao longo do ano

Foi identificado um aumento mais expressivo nas vendas durante os meses de novembro e dezembro, possivelmente relacionado às festividades e campanhas comerciais de fim de ano.

Também foram observados outros períodos de crescimento:

- 2023: entre março e maio.
- 2024: entre janeiro e março e entre junho e agosto.
- 2025: entre fevereiro e março.

Essas variações levantam hipóteses sobre possíveis influências de campanhas promocionais ou outros fatores comerciais, que poderiam ser investigados em análises complementares.

## Aprendizados

O desenvolvimento deste desafio proporcionou a oportunidade de colocar em prática conhecimentos relacionados a:

- Organização e tratamento de dados.
- Modelagem dimensional.
- Relacionamentos entre tabelas.
- Construção de medidas com DAX.
- Desenvolvimento de indicadores.
- Visualização e interpretação de dados.
- Identificação de padrões e elaboração de hipóteses analíticas.


Sigo aprendendo e evoluindo!


Desenvolvido por Victor Tchiya Soares.

Desafio prático: Educadados | Professor Felipy Morais.
