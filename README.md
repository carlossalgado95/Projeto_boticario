# Projeto_boticario
# Análise Exploratória Final para Previsão de Vendas

Este repositório contém o notebook de análise exploratória final do projeto de previsão de vendas. O objetivo desta análise é compreender a variabilidade das vendas e identificar padrões significativos que podem orientar estratégias de marketing e otimização de recursos.

## Resumo da Análise

### 1. **Preparação dos Dados**

- **Tratamento de Dados Faltantes:** Foi identificada uma grande proporção de valores nulos na variável `VL_RECEITA_BRUTA`, o que impacta a modelagem e a previsão de vendas.
- **Formato de Data:** A coluna de data possui um formato inadequado (`YYYYWW`), dificultando a análise temporal e a previsão de vendas. A conversão dessa data para um formato padrão de `datetime` é essencial para uma análise precisa.

### 2. **Análise Descritiva**

- **Distribuição das Variáveis:**
  - **`FLG_DATA`:** Indicador binário de data comemorativa, com cerca de 29% das observações associadas a datas especiais.
  - **`COD_CANAL`:** Dois canais distintos de vendas, que possibilitam a comparação entre vendas online e físicas.
  - **`DES_CATEGORIA_MATERIAL`:** Seis categorias de materiais, permitindo a análise de desempenho por tipo de produto.
  - **`COD_REGIAO`:** Duas regiões de venda, facilitando a comparação de desempenho regional.
  - **`COD_MATERIAL`:** 2252 materiais distintos, representando a diversidade de produtos.
  - **`VL_PRECO`:** Dois valores de preço, indicando uma estrutura de preços simples.

### 3. **Visualização e Análise**

- **Correlação entre Variáveis:** 
  - **`FLG_CAMPANHA_MKT_B`** tem uma correlação significativa (0.91) com **`QT_VENDA_BRUTO`**.
  - **`QT_VENDA_BRUTO`** apresenta uma forte correlação (0.91) com **`VL_RECEITA_LIQUIDA`**.
  - **`FLG_CAMPANHA_MKT_A`** e **`FLG_CAMPANHA_MKT_C`** têm uma correlação significativa (0.69).
  - **`FLG_CAMPANHA_MKT_A`** mostra uma correlação perfeita (1.00) com **`VL_RECEITA_LIQUIDA`**.

### 4. **Insights e Recomendações**

- **Alta Variabilidade:** Alguns grupos, como **`COD_CANAL = 0`** e **`COD_REGIAO = 0`**, mostram alta variabilidade na receita bruta, o que pode indicar grandes transações ou clientes de alto valor.
- **Diferença de Receita Média:** O grupo **`COD_CANAL = 0`** e **`COD_REGIAO = 0`** tem a maior média de receita bruta, sugerindo que essas áreas podem ser mais lucrativas.
- **Valores Máximos Altos:** Certos grupos têm valores máximos elevados, indicando grandes transações que impactam a receita total.
- **Desvio Padrão Elevado:** Altos desvios padrões indicam variações significativas na receita bruta, refletindo diferentes padrões de transação entre canais e regiões.

### 5. **Conclusão e Ações Recomendadas**

- **Investigue Grandes Transações:** Analisar transações de alto valor pode revelar oportunidades para replicar ou expandir essas receitas.
- **Ajuste Estratégias:** Personalize estratégias de marketing e vendas com base nas diferenças de receita média entre canais e regiões.
- **Gerencie Variabilidade:** Monitorar e entender a alta variabilidade pode ajudar a otimizar a gestão de receitas e melhorar previsões.

## Objetivo

O objetivo desta análise é fornecer uma visão abrangente dos dados de vendas, identificar padrões e tendências significativas e oferecer recomendações para melhorar o planejamento de demanda e a eficácia das campanhas de marketing.

## Nota

A análise explora a variabilidade e o impacto dos dados de vendas em diferentes categorias e regiões, fornecendo insights para estratégias de vendas mais eficazes.

