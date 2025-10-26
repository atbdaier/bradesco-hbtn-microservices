# Projeto de Microsserviços

Este projeto consiste em uma arquitetura de microsserviços que implementa um sistema de gerenciamento de pedidos, produtos e clientes.

---

## Visão Geral

A arquitetura foi projetada para permitir autonomia, escalabilidade e manutenção fácil dos componentes. Cada microsserviço é responsável por uma funcionalidade específica do sistema.

---

## Serviços implementados

- **Serviço de Clientes**  
  Gerencia informações de clientes, incluindo cadastro, atualização e busca.

- **Serviço de Produtos**  
  Gerencia o catálogo de produtos disponíveis, incluindo detalhes, preços e estoque.

- **Serviço de Pedidos**  
  Controla os pedidos realizados pelos clientes, incluindo criação, atualização e consulta de pedidos.

- **API Gateway**  
  Encaminha as requisições dos clientes para os microsserviços adequados, centralizando as rotas e agregando funcionalidades.

---

## Benefícios

- **Independência**: cada serviço funciona de forma autônoma, facilitando manutenção e atualizações.
- **Escalabilidade**: serviços podem ser escalados individualmente conforme a demanda.
- **Resiliência**: falhas em um serviço não impactam o funcionamento geral do sistema.

---

## Comunicação entre microsserviços

- **Modo Síncrono**: via requisições HTTP/REST ou gRPC.
- **Modo Assíncrono**: usando filas de mensagens (exemplo: RabbitMQ, Kafka).

---

## Como rodar o projeto

1. Clone o repositório:
   ```bash
   git clone <URL_DO_REPOSITÓRIO>