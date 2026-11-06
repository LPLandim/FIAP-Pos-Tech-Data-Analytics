# 📁 Diretório de Dados | Fase 1 - Data Analytics

Este diretório contém os dados e especificações utilizadas na análise de e-commerce da Olist para o **Tech Challenge - Fase 1**.

---

## 📌 Origem dos Dados Brutos
A base de dados pública utilizada é o **Brazilian E-Commerce Public Dataset by Olist**, cobrindo o histórico de cerca de 100.000 pedidos realizados no Brasil entre setembro de 2016 e agosto de 2018.

* **[Kaggle - Brazilian E-Commerce Public Dataset by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)**

---

## 📊 Dados Tratados Disponíveis no Repositório
* **`analise_regional_olist.xlsx`**: Arquivo com os **dados consolidados e tratados** resultantes do pipeline de análise. Contém a distribuição regional por estado (UF), consolidando:
  * Contagem e participação percentual de clientes;
  * Volume total de pedidos entregues;
  * Quantidade e taxa percentual de pedidos entregues com atraso;
  * Classificação de prioridade estratégica por volume e criticidade operacional.

---

## 🗂️ Estrutura Relacional da Base Olist (Dados de Entrada):
1. **Orders (`olist_orders_dataset`)**: Informações de compra, status do pedido e carimbos de data/hora (compra, aprovação, envio, entrega efetiva e previsão estimada).
2. **Order Items (`olist_order_items_dataset`)**: Identificação dos produtos por pedido, vendedor, valor de frete e preço unitário.
3. **Payments (`olist_order_payments_dataset`)**: Meios de pagamento (cartão de crédito, boleto, voucher, débito), valor pago e parcelamento.
4. **Reviews (`olist_order_reviews_dataset`)**: Notas de satisfação (1 a 5 estrelas), data e comentários de avaliação.
5. **Customers (`olist_customers_dataset`)**: Associação de `customer_id` (por pedido) e `customer_unique_id` (identificador único do cliente para cálculo de recompra), cidade e estado.
6. **Sellers (`olist_sellers_dataset`)**: Localização geográfica dos lojistas parceiros.
7. **Products (`olist_products_dataset`)**: Categoria do produto, dimensões e peso.
8. **Geolocation (`olist_geolocation_dataset`)**: Coordenadas geográficas por prefixo de CEP.
