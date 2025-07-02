# Relatorio_vendas
Este repositório apresenta um projeto de análise de dados focado em vendas, demonstrando a transformação de dados brutos em insights acionáveis através de consultas SQL e uma visualização interativa. O objetivo é ilustrar um fluxo de trabalho completo, desde a manipulação de dados no banco de dados até a apresentação de métricas de performance.
Introdução para o GitHub
Olá! Este repositório apresenta um projeto de análise de dados focado em vendas, demonstrando a transformação de dados brutos em insights acionáveis através de consultas SQL e uma visualização interativa. O objetivo é ilustrar um fluxo de trabalho completo, desde a manipulação de dados no banco de dados até a apresentação de métricas de performance e tendências de crescimento em um formato de infográfico.

Arquivo README.md
# Análise de Vendas: Transformando Dados em Insights

Este projeto demonstra um pipeline de análise de dados de vendas, desde a extração e transformação de dados brutos usando SQL até a visualização interativa de métricas de performance e tendências de crescimento. O objetivo é fornecer um exemplo prático de como a inteligência de negócios pode ser gerada a partir de dados transacionais.

## Visão Geral do Projeto

O cerne deste projeto reside em duas consultas SQL principais que processam dados de vendas para gerar duas tabelas analíticas:

1.  **`tabela_vendas_produtos`**: Agrega informações de pedidos e produtos para calcular receita, custo e lucro por transação.
2.  **`tabela_vendas_mom`**: Utiliza os dados da primeira tabela para calcular o crescimento Mês a Mês (Month-over-Month - MoM) da receita total, fornecendo uma visão clara das tendências de vendas ao longo do tempo.

## Principais Features

* **Modelagem de Dados SQL**: Criação de tabelas analíticas (`tabela_vendas_produtos`, `tabela_vendas_mom`) a partir de dados transacionais.
* **Cálculo de Métricas Essenciais**: Determinação de receita, custo, lucro e crescimento MoM.
* **Análise de Tendências**: Utilização de funções de janela (`LAG`) para análise temporal.
## Tecnologias Utilizadas

* **SQL**: Para manipulação e agregação de dados.
* **BIGQUERY**: Para inserção e importação das bases de dados
* **LOOKER**: Para criação de graficos e obtenção de insights
## Como Visualizar

## Estrutura de Dados (Conceitual)

As consultas SQL operam sobre as seguintes estruturas de tabela conceituais:

* **`orders_items`**:
    * `order_id` (ID do Pedido)
    * `status` (Status do Pedido)
    * `created_at` (Data de Criação do Pedido)
    * `shipped_at` (Data de Envio)
    * `delivered_at` (Data de Entrega)
    * `sale_price` (Preço de Venda do Item)
    * `product_id` (ID do Produto)

* **`products`**:
    * `id` (ID do Produto)
    * `cost` (Custo do Produto)

