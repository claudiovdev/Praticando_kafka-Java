# Projeto: Cadastro de usuario ultilizando kafka e serviço de notificação

Este projeto é uma aplicação Java/Spring que utiliza **Kafka** para gerenciar um fluxo de **cadastro de usuários**. Ele envia os dados de registro para o Kafka, onde um **Producer** serializa os dados do usuário e um **Consumer** os consome. Se houver erros durante o processamento da mensagem, um sistema de tratamento de erros com **retries** (tentativas) e **DLT (Dead Letter Topic)** é implementado para garantir que as mensagens com falhas sejam armazenadas para análise posterior.

## Tecnologias usadas
- **Java 11**
- **Spring boot**
- **Apache Kafka**
- **Jackson (para serialização/deserialização)**
- **Docker (opcional, para rodar o Kafka localmente)**
