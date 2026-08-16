# 🛒 PavPlas — Gateway de Pagamento 

Sistema em desenvolvimento para **automação do processo de vendas e pagamentos da PavPlas**, desenvolvido como projeto acadêmico do curso de **Gestão da Tecnologia da Informação — Fatec Barueri**.

> 🚧 **Status: Em desenvolvimento**

## 📌 Sobre o projeto

O projeto tem como objetivo analisar e modernizar o processo de vendas da PavPlas.

Atualmente, o site da empresa funciona principalmente como um catálogo de produtos, enquanto o processo de compra é realizado manualmente por meio do **WhatsApp**, envolvendo consultas de estoque, negociação de valores, cálculo de frete e confirmação de pagamentos.

A proposta deste projeto é transformar esse fluxo em uma experiência de compra digital mais automatizada e integrada.

## 🎯 Objetivos

* Automatizar o processo de compra;
* Implementar um carrinho de compras;
* Realizar validação automática de estoque;
* Automatizar o cálculo de frete;
* Disponibilizar diferentes métodos de pagamento;
* Integrar o sistema a um Gateway de Pagamento;
* Atualizar automaticamente o status dos pedidos;
* Integrar informações entre os setores financeiro, comercial e logístico;
* Reduzir processos manuais e retrabalho;
* Melhorar a experiência do cliente.

## 💳 Fluxo proposto

O fluxo **To-Be** foi projetado para permitir que o cliente realize sua compra diretamente pela plataforma:

```text
Cliente
   │
   ▼
Catálogo de Produtos
   │
   ▼
Carrinho de Compras
   │
   ▼
Validação de Estoque
   │
   ▼
Cálculo de Frete
   │
   ▼
Checkout
   │
   ▼
Gateway de Pagamento
   │
   ├── PIX
   ├── Boleto
   └── Cartão
   │
   ▼
Pagamento Aprovado
   │
   ├── Atualização do Pedido
   ├── Baixa no Estoque
   ├── Faturamento
   ├── Logística
   └── Registro Financeiro
```

O modelo proposto prevê integração com estoque, serviços de frete, gateway de pagamento, ERP e processos de logística e financeiro.

## 🔎 Problemas identificados

Durante a análise do processo atual (**As-Is**), foram identificados alguns dos principais problemas:

* Dependência de atendimento humano para concluir vendas;
* Limitação de vendas fora do horário comercial;
* Conferência manual de pagamentos;
* Risco de erros e fraudes na validação de comprovantes;
* Falta de integração entre estoque, catálogo e faturamento;
* Retrabalho e redigitação de informações;
* Quebra da experiência do cliente ao sair do site para finalizar a compra pelo WhatsApp.

## 🚀 Funcionalidades planejadas

### 🛍️ E-commerce

* [ ] Catálogo de produtos
* [ ] Cadastro de usuários
* [ ] Carrinho de compras
* [ ] Checkout
* [ ] Consulta de estoque
* [ ] Cálculo de frete

### 💰 Pagamentos

* [ ] Integração com Gateway de Pagamento
* [ ] Pagamento via PIX
* [ ] Pagamento via boleto
* [ ] Pagamento via cartão de crédito
* [ ] Atualização automática do status do pagamento
* [ ] Conciliação financeira

## 🧩 Tecnologias

> As tecnologias abaixo podem ser atualizadas conforme o desenvolvimento do projeto evoluir.

* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Em desenvolvimento
* **Banco de dados:** Em definição
* **Integrações:** APIs
* **Pagamento:** Gateway de Pagamento
* **Versionamento:** Git / GitHub
* **Modelagem de processos:** BPMN

## 📊 As-Is x To-Be

| Processo atual (As-Is)           | Processo proposto (To-Be)       |
| -------------------------------- | ------------------------------- |
| Site utilizado como catálogo     | E-commerce completo             |
| Compra pelo WhatsApp             | Compra diretamente pelo sistema |
| Consulta manual de estoque       | Validação automática            |
| Frete calculado manualmente      | Cálculo integrado               |
| PIX/transferência manual         | Gateway de pagamento            |
| Comprovante enviado pelo cliente | Confirmação automática          |
| Atualização manual do pedido     | Atualização automática          |
| Processos separados              | Sistemas integrados             |

## 🎓 Projeto acadêmico

Este projeto está sendo desenvolvido como parte do curso de **Gestão da Tecnologia da Informação da Fatec Barueri**.

**Instituição:** Fatec Barueri — Padre Danilo José de Oliveira Ohl
**Curso:** Gestão da Tecnologia da Informação
**Ano:** 2026

### 👥 Stakeholders externos

* Rafael Thiengo Reis
* Gustavo Sirqueira Soares da Silva
* Stanley Sousa do Vale
* Cauã Azeredo Golden Rodrigues
* Nayara Teixeira da Silva
* Heitor Soares Tanan

**Orientador:** Prof. Vander Ribeiro Elme

## 📚 Documentação

A documentação do projeto apresenta as principais etapas de análise e desenvolvimento da solução para a PavPlas:

* **Levantamento de requisitos**;
* **Análise do processo atual (As-Is)**;
* **Identificação de problemas e gargalos**;
* **Proposta do processo futuro (To-Be)**;
* **Metodologia de desenvolvimento**;
* **Modelagem e arquitetura da solução**;
* **Gateway de pagamento e fluxo de pagamentos**;
* **Segurança e proteção de dados**;
* **Conclusões**.

[📄 Acessar Monografia](https://centropaulasouza-my.sharepoint.com/:w:/g/personal/stanley_vale_aluno_cps_sp_gov_br/IQAhXMxQcte2SLOiCvJrBqe2ASl8TQBpAwXTMBuRzbDCZqU?e=P8UXAK)

## 📄 Referências

O projeto acadêmico utiliza como referências materiais relacionados a **Gestão de Processos de Negócio (BPM)**, **mapeamento As-Is/To-Be** e **Gateways de Pagamento**.

---

### 🚧 Projeto em desenvolvimento

Este repositório acompanha a evolução do sistema **PavPlas — Gateway de Pagamento**, desde sua análise e modelagem dos processos até a futura implementação da solução automatizada.
