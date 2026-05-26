# Orquestração de Workflows com AWS Step Functions ☁️🤖

O objetivo é criar e documentar uma arquitetura de microsserviços serverless utilizando o AWS Step Functions.

## 📌 Cenário Prático
O fluxo desenvolvido simula um **Processamento de Pedidos de E-commerce** que integra os seguintes serviços:
* **AWS Step Functions:** Orquestração visual e lógica do fluxo.
* **AWS Lambda:** Validação e processamento de pagamento.
* **Amazon DynamoDB:** Persistência do pedido aprovado.
* **Amazon SNS:** Envio de notificações de sucesso ou falha.

## 📐 Design do Workflow
Aqui está o gráfico gerado no Workflow Studio que valida as decisões de estoque e faz o tratamento de erros:

![Workflow Graph](./Sem%20título.png)


---
