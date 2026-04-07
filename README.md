# PUC-SP - Ciência da Computação
## Banco de Dados II: Stored Procedures & Functions no PostgreSQL

Este repositório contém o desenvolvimento de um sistema de backend para E-commerce utilizando **PL/pgSQL**. O projeto foi realizado no ambiente **PostgreSQL (Neon Cloud)** integrado ao **Google Colab**.

### Objetivo do Projeto
O objetivo principal é demonstrar o domínio de lógica de programação dentro do banco de dados, automatizando regras de negócio complexas, garantindo a integridade dos dados e otimizando a performance através de processos que rodam diretamente no servidor.

### O que foi implementado?

#### Parte 1: Fundamentos (Exercícios 1 ao 5)
* **Gestão de Preços:** Procedimentos para reajustes globais e descontos por categoria com logs de auditoria.
* **Processamento de Pedidos:** Implementação de lógica transacional (`ROLLBACK`/`COMMIT`) para processar carrinhos de compras via **JSON**, garantindo que o estoque só seja baixado se o pedido for concluído.
* **Alertas de Estoque:** Automação de notificações para produtos com baixo inventário.

#### Parte 2: BI e Automação (Exercícios 6 ao 10)
* **Exercício 6 (Top Sellers):** Função que retorna uma tabela com o ranking dos 10 produtos mais vendidos, facilitando a criação de dashboards.
* **Exercício 7 (Customer LTV):** Cálculo do *Lifetime Value* do cliente para identificar os perfis que mais geram receita.
* **Exercício 8 (Promoção por Validade):** Rotina que aplica descontos automáticos de 20% em produtos próximos ao vencimento.
* **Exercício 9 (Manutenção de Logs):** Procedimento de limpeza para remover registros de auditoria antigos e manter a performance do banco.
* **Exercício 10 (Fechamento Diário):** Projeto integrado que consolida vendas, bonifica clientes com pontos de fidelidade e gera relatórios de sistema.

> **Nota Técnica:** As rotinas de agendamento automático (`pg_cron`) foram validadas logicamente no código, mas sua ativação depende de permissões de superusuário no ambiente de nuvem utilizado.

### Equipe
* Caroline Campos
* Isabela Gomes 
