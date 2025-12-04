# Lab – Solução Serverless com Logic Apps, Functions e Service Bus

## Objetivo

Criar um fluxo serverless integrando:

- **Logic Apps** para orquestração
- **Azure Functions** para regras de negócio
- **Service Bus** para comunicação assíncrona
- Banco de dados para persistir informações

## Fluxo resumido

1. Evento dispara um Logic App (HTTP, fila, agenda etc.)
2. Logic App chama uma Azure Function com dados de entrada
3. Function processa e grava em banco ou envia mensagem para Service Bus
4. Outro componente consome a mensagem e continua o fluxo

## Aprendizados

- Como montar fluxo event-driven sem gerenciar servidores
- Integração entre múltiplos serviços Azure
- Vantagens de desacoplar componentes usando Service Bus
