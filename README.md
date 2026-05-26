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

## 🧠 Insights Adquiridos
* **Centralização da Lógica:** Tirar a lógica de transição das funções Lambda e colocar no Step Functions deixa o código mais limpo e fácil de manter.
* **Resiliência:** O uso de blocos de captura de erro (Catch) evita que falhas em uma etapa derrubem todo o sistema.
* **Economia:** Integrações nativas (como salvar direto no DynamoDB ou enviar SNS) reduzem o uso de funções Lambda desnecessárias, diminuindo custos.

---
