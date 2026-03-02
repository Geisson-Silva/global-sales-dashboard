# 📊 Análise de Vendas Globais — Google Sheets

## 📌 Visão Geral

Este projeto consiste em uma análise completa de vendas de uma empresa global que comercializa produtos por canais **online** e **offline**.
A análise foi desenvolvida no **Google Sheets**, utilizando técnicas de limpeza de dados, análise exploratória, criação de métricas financeiras, visualizações e análise ABC (Curva de Pareto), com foco em gerar insights de negócio.

O conjunto de dados é composto por três tabelas:

* **Events** — registros de vendas ao longo de vários anos
* **Products** — informações dos produtos e categorias
* **Countries** — países, regiões e sub-regiões

---

## 🎯 Objetivo do Projeto

* Avaliar a qualidade e integridade dos dados.
* Calcular métricas financeiras (receita, custo e lucro).
* Analisar desempenho de vendas por:

  * categorias de produtos
  * países, regiões e sub-regiões
  * canais de venda (online/offline)
  * períodos de tempo (anos, meses e dias da semana)
* Avaliar relação entre tempo de envio e lucro.
* Realizar análise ABC com base no princípio de Pareto.
* Criar um mini dashboard com as principais visualizações.
* Apresentar conclusões sob a ótica de negócio.

---

## 🧹 Tratamento e Qualidade dos Dados

Foi realizada uma análise de integridade dos dados com os seguintes ajustes:

* Padronização das colunas de data para o formato brasileiro.
* Ajuste da localidade da planilha para Brasil.
* Padronização dos valores de canal de venda (Online/Offline).
* Registros com país ausente (#N/A) classificados como **UNK (Unknown)** e agrupados na sub-região **Outros**.
* Correção do separador decimal em campos financeiros.
* Formatação monetária em Real Brasileiro (R$).

---

## 📈 Métricas Criadas

Na tabela **Events** foram adicionadas as colunas:

* **Receita Total** = quantidade × preço unitário
* **Custo Total** = quantidade × custo unitário
* **Lucro Total** = receita total − custo total

Também foram calculadas métricas gerais, como:

* número total de pedidos
* lucro total
* número de países atendidos

---

## 🔎 Principais Análises Realizadas

### Lucro por dia da semana

* Maior volume de lucro ocorre aos domingos.
* Estabilidade entre segunda e terça-feira.
* Queda acentuada na quarta-feira, seguida de recuperação gradual até sábado.

### Análise ABC (Curva de Pareto)

* Forte concentração de resultados:

  * Classe A: ~77%–80% do lucro total (6 categorias).
  * Classe B: 3 categorias.
  * Classe C: 3 categorias.
* Confirmação clara do princípio de Pareto.

### Dinâmica temporal de vendas

* Crescimento entre 2010–2012.
* Queda em 2013.
* Recuperação em 2014.
* Retração em 2015.
* Retomada do crescimento entre 2016–2017.

### Análise geográfica

* Top 10 países majoritariamente europeus.
* País classificado como **UNK** aparece como líder devido a inconsistências nos dados.
* Forte concentração de lucro por sub-região, com queda progressiva entre posições do ranking.

### Canais de venda

* Online e offline apresentam equilíbrio na geração de lucro.
* Não há dependência clara de um único canal.

### Tempo de envio vs lucro

* Não foi identificado padrão consistente.
* Ausência de relação direta entre tempo de envio e lucratividade nesta base.

---

## 📊 Dashboard

Foi criado um mini dashboard no Google Sheets consolidando as principais visualizações:

* desempenho por categorias
* análise geográfica
* evolução temporal
* análise por canal de venda
* resultados da análise ABC

---

## 💼 Principais Insights de Negócio

* Forte concentração de lucro em poucas categorias (efeito Pareto).
* Dependência geográfica relevante, com predominância europeia.
* Necessidade de melhoria na qualidade dos dados geográficos.
* Distribuição equilibrada entre canais online e offline.
* Tempo de envio não demonstrou impacto direto no lucro.

---

## 🛠️ Ferramentas Utilizadas

* Google Sheets
* Funções analíticas (WEEKDAY, agregações, fórmulas financeiras)
* Tabelas dinâmicas
* Visualizações e dashboards

---

## 📄 Observação

Este projeto foi desenvolvido como estudo prático de análise de dados aplicada ao negócio, com foco em tomada de decisão baseada em dados e comunicação de insights.
