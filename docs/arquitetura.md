# Relatório de Arquitetura e Modelagem de Solução
**Projeto:** Sistema de Encomendas de Bolos  
**Disciplina:** Projeto Integrador II  
**Professor:** Clécio Sousa  

---

## 1. Visão Geral da Solução
O **Sistema de Encomendas de Bolos** é uma plataforma desenvolvida para facilitar a escolha, personalização e cálculo do valor total de pedidos de bolos personalizados em tempo real.

---

## 2. Fluxograma de Funcionamento

```mermaid
graph TD
    A[Cliente acessa a plataforma] --> B[Escolhe tamanho e tipo de massa]
    B --> C[Seleciona recheios e decoração]
    C --> D[Sistema calcula valor em tempo real]
    D --> E{Cliente possui cadastro?}
    E -- Não --> F[Realiza cadastro/login]
    E -- Sim --> G[Confirma a encomenda]
    F --> G
    G --> H[Pedido enviado com sucesso]
