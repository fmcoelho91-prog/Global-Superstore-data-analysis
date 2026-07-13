# Global Superstore - Data Analysis & Business Intelligence


## Executive Summary
Este projeto foca-se na auditoria e análise da rentabilidade da **Global Superstore** (2011-2014). Mais do que reportar o volume de vendas, o objetivo central foi identificar fugas de capital, auditar a integridade dos dados operacionais e encontrar a verdadeira causa raiz das encomendas com margens negativas.

O resultado final traduz-se num Dashboard interativo e num relatório de insights com propostas de melhoria de margem de lucro.

![Dashboard Global Superstore](INSERIR_LINK_DA_IMAGEM_AQUI)

---

## Tech Stack & Metodologia
* **Ferramenta:** Microsoft Excel
* **Técnicas Aplicadas:**
  * **Limpeza e Estruturação de Dados:** Tratamento de valores nulos e estruturação de variáveis.
  * **Data Integrity (Chaves Compostas):** Criação de uma *Primary Key* composta (Order ID + Market) para evitar a duplicação de devoluções, garantindo que o lucro final (Net Profit) reportado é 100% puro.
  * **Cálculo de Métricas (Gross vs Net):** Deduzidas todas as faturas devolvidas para análise de *Net Sales* e *Net Profit* reais.
  * **Fórmulas Avançadas:** IF, ISNA, VLOOKUP, CONCAT, aninhamento de lógica condicional.
  * **Visualização:** Tabelas Dinâmicas (Pivot Tables) interativas e Slicers conectados para Storytelling de dados.


## Key Business Insights

Após a análise detalhada ao lucro líquido total de **$1.43 Milhões**, destacam-se três descobertas críticas de negócio:

### 1. O Mito do Volume vs. Eficiência (APAC vs. US)
Embora a região **APAC (Ásia-Pacífico)** seja o motor de faturação da empresa (+$3.4 Milhões), os **Estados Unidos** são o mercado com a operação mais eficiente. Nos EUA, a empresa atinge a rentabilidade máxima (12.96% de margem). Na prática, para colocar $1 de lucro líquido no bolso, a empresa precisa de vender $8.40 na Ásia, mas apenas $7.70 nos EUA.

### 2. A "Anatomia do Prejuízo"
A auditoria revelou que quase 30% das operações da empresa destroem valor. Isolámos um balde crítico de mais de **15.000 encomendas não-lucrativas**, que geram um buraco financeiro superior a **-$900.000**.

### 3. A Causa Raiz: Política de Descontos no Mobiliário
O cruzamento de dados provou que o prejuízo não é aleatório, derivando de uma agressiva política de descontos usada para forçar o fecho de vendas. 
O impacto é fatal na categoria de **Mobiliário (Furniture)**: devido aos elevados custos logísticos (transporte de volumes pesados), cada encomenda desta categoria que entra no balde negativo custa à empresa, em média, **-$104**.

---

## Recomendação Estratégica
Para estancar esta hemorragia de capital, a principal recomendação técnica é a **implementação de um Teto Máximo de Desconto (Discount Cap)** bloqueado no sistema, com especial urgência para a região da APAC e para a categoria de Mobiliário. Ao isolar ou corrigir apenas as operações com margem negativa, o lucro atual da empresa tem o potencial de quase duplicar no curto prazo.

---
*Projeto desenvolvido como parte do portefólio de Data Analytics.*
