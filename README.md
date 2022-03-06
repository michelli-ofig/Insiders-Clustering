# Insiders Clustering
![capa linkedin](https://user-images.githubusercontent.com/77075354/156940134-007ec87d-e28f-466e-9096-f71e03f0cbc1.jpeg)

O Insiders Clustering trata-se de um programa de fidelidade da empresa All In On Place destinado a um pequeno número de clientes que possuí um alto número de volume de compras ou então compram produtos de alto valor o que acaba gerando um valor representativo para o faturamento da empresa. São clientes de alto valor e por isso precisam ser fidelizados.

### Objetivo do Projeto

Identificar mensalmente quais são os clientes elegíveis para o programa de fidelização, bem como, criar novas estratégias de marketing para inserir 
potenciais clientes no grupo Insiders Clustering.

### Hipóteses de Negócios

 **Quem são as pessoas elegíveis para do programa de fidelidade?**
 
Clientes com alto ticket médio, alto LTV, baixa recência, alto basket size, baixa probabilidade de churn, alta propensão de compra?

-**Qual é a porcentagem de faturamento por ano vinda do cluster Insider?**

Com esses dados é possível planejar qual é o custo para manter o cliente Insider.

**Expectativa de faturamento:** 

Com isso é possível planejar quais ações devem ser feitas para manter o cliente Insider.

-**Quais ações tomar para fazer clientes com o perfil próximo ao Insider tornar-se um.**

Antes de aplicar o modelo de Machine Learning é necessário identificar padrões do cliente Insider através da matriz RFM:

**Recência:** 

- Tempo desde a última compra

- Tempo de resposta do cliente

**Frequência:**

- Tempo médio entre as transações, quantos produtos o cliente compra em determinado período

**Monetário:**

Quanto o cliente traz de faturamento?

Cliente possui um alto LTV?

## Estratégia de Solução

**Data Description:** Rename columuns, Data dimensions, Data types, Replace NA.

**Feature Engineering:** Foram criadas novas features através de features originais: Gross Revenue, Monetary, Recency, Frequency, Avg Ticket.

**Exploratory Data Analysis:** Foram criada novas features para validação das hipóteses de negócio, são elas:  qtde_invoices, qtde_items, qtde_products,avg_ticket, avg_recency_days, frequency, qtde_returns, avg_basket_size, avg_unique_basket_size.

**Cluster Analysis:** Estudo do Espaço: PCA, t-SNE, Tree-Based Embedding, Decision Tree.



![Tree Based Embedding](https://user-images.githubusercontent.com/77075354/156940453-4dc1037d-6a90-4811-8232-995e7a277897.PNG)

## Top 3 Data Insights

**H1. Os clientes do cluster insiders possuem um volume (produtos) de compras acima de 10% do total de compras**

**Verdade:** O cluster insider possui um volume de compra de produtos de 51%.

**H2. Os clientes do cluster insiders possuem um volume (faturamento) de compras acima de 10% do total de compras**

**Verdadeiro:** O cluster insider possui um volume de GMV de 50%.

**H5. A GMV dos clientes insiders esta concentrados no 3 quartil**

**Falso:** O faturamento do cluster insiders está concentrado no primeiro quartil.


![Violin Plot](https://user-images.githubusercontent.com/77075354/156940598-654c24ee-be46-46db-b3be-e1d6ee126d3c.PNG)

## Aplicação do Modelo de Machine Learning
Foram testados e validados com o cross validation os modelos KMeans, GMN e HClustering, obtendo os seguintes resultados:




![Resultados do modelos de ML](https://user-images.githubusercontent.com/77075354/156940608-45418c43-ebd0-4bba-95f8-67a73f15af37.PNG)


**Para a solução do problema de negócio foi utilizado o KMeans:**




![KMeans](https://user-images.githubusercontent.com/77075354/156940643-f3de94b5-568d-49ab-a000-89b7cca1c840.PNG)

## Performance do Modelo de Machine Learning
![Cluster Validation](https://user-images.githubusercontent.com/77075354/156940689-63ec7c48-fe34-41a5-a551-fa509f0867e3.PNG)

## Resultado de Negócio

![Clusters](https://user-images.githubusercontent.com/77075354/156941508-52322463-6560-4eac-9096-959959d6e843.PNG)

## Conclusão

Composição do Cluster Insider: 
- Número de clientes: 412 (14% dos clientes)
- Faturamento médio: $ 9757,00
- Recência média: 20 dias
- Média de Produtos comprados: 451 produtos
- Frequência de Produtos comprados: 0.10 produtos/dia
- Receita em média: $9757,00 dólares



