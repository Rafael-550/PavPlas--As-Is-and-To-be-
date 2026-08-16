# Requisitos Funcionais - PavPlas

## 1. Identificação do Documento
* **Projeto:** Gateway de Pagamento PavPlas
* **Documento:** Levantamento de Requisitos Funcionais
* **Status:** Levantamento preliminar (A validar)
* **Técnica:** Análise documental dos processos As-Is e To-Be

---

## 2. Tabela de Requisitos Funcionais

| ID | Requisito Funcional | Origem / Justificativa no Processo | Prioridade | Status |
|---|---|---|---|---|
| **RF-01** | O sistema deve permitir o cadastro e a autenticação de clientes. | Área do cliente e identificação no checkout | Alta | A validar |
| **RF-02** | O sistema deve exibir o catálogo de produtos com informações atualizadas. | Catálogo virtual da PavPlas | Alta | A validar |
| **RF-03** | O sistema deve permitir adicionar, alterar e remover produtos do carrinho. | Carrinho de compras proposto | Alta | A validar |
| **RF-04** | O sistema deve consultar e exibir a disponibilidade dos produtos em estoque. | Validação automática do inventário | Alta | A validar |
| **RF-05** | O sistema deve impedir a finalização de pedidos sem estoque suficiente. | Redução de erros e vendas indisponíveis | Alta | A validar |
| **RF-06** | O sistema deve coletar e validar o endereço de entrega do cliente. | Etapa de entrega no checkout | Alta | A validar |
| **RF-07** | O sistema deve calcular automaticamente o valor do frete. | Integração com tabelas/API logística | Alta | A validar |
| **RF-08** | O sistema deve apresentar a previsão de entrega. | Retorno da integração logística | Média | A validar |
| **RF-09** | O sistema deve permitir a seleção da modalidade de entrega disponível. | Definição do frete antes do pagamento | Média | A validar |
| **RF-10** | O sistema deve apresentar o resumo do pedido antes da confirmação. | Checkout integrado | Alta | A validar |
| **RF-11** | O sistema deve permitir pagamento por PIX. | Método previsto no modelo To-Be | Alta | A validar |
| **RF-12** | O sistema deve gerar QR Code e código PIX Copia e Cola. | Automação do pagamento por PIX | Alta | A validar |
| **RF-13** | O sistema deve permitir pagamento por boleto bancário. | Método previsto no modelo To-Be | Alta | A validar |
| **RF-14** | O sistema deve gerar o boleto e disponibilizá-lo ao cliente. | Processamento automatizado do boleto | Alta | A validar |
| **RF-15** | O sistema deve permitir pagamento por cartão de crédito. | Método previsto no modelo To-Be | Alta | A validar |
| **RF-16** | O sistema deve apresentar as opções de parcelamento configuradas pela empresa. | Parcelamento parametrizado | Média | A validar |
| **RF-17** | O sistema deve enviar a transação ao gateway de pagamento. | Integração central da proposta | Alta | A validar |
| **RF-18** | O sistema deve receber e registrar o resultado da transação retornado pelo gateway. | Aprovação ou recusa do gateway | Alta | A validar |
| **RF-19** | O sistema deve informar ao cliente se o pagamento foi aprovado, recusado ou está pendente. | Retorno sistêmico do pagamento | Alta | A validar |
| **RF-20** | O sistema deve atualizar automaticamente o status do pedido após a confirmação do pagamento. | Alteração para o estado "Pago" | Alta | A validar |
| **RF-21** | O sistema deve enviar uma confirmação do pagamento e do pedido por e-mail. | Notificação automática ao cliente | Média | A validar |
| **RF-22** | O sistema deve efetuar a baixa do produto no estoque após a confirmação do pagamento. | Integração com inventário | Alta | A validar |
| **RF-23** | O sistema deve enviar os dados do pedido e do cliente ao ERP. | Integração com faturamento | Alta | A validar |
| **RF-24** | O sistema deve solicitar a emissão automática da NF-e. | Emissão fiscal proposta | Alta | A validar |
| **RF-25** | O sistema deve disponibilizar ou enviar a NF-e ao cliente. | Entrega do documento fiscal | Alta | A validar |
| **RF-26** | O sistema deve gerar uma ordem de separação para o setor logístico. | Automação do backoffice | Alta | A validar |
| **RF-27** | O sistema deve gerar a etiqueta de postagem ou transporte. | Preparação automatizada da expedição | Média | A validar |
| **RF-28** | O sistema deve atualizar o pedido conforme o andamento da expedição. | Integração com logística | Média | A validar |
| **RF-29** | O sistema deve permitir que o cliente acompanhe o status do pedido. | Rastreabilidade na área do cliente | Média | A validar |
| **RF-30** | O sistema deve registrar a entrada financeira da venda confirmada. | Integração com o setor financeiro | Alta | A validar |
| **RF-31** | O sistema deve realizar a conciliação automática dos pagamentos. | Eliminação da conferência manual | Alta | A validar |
| **RF-32** | O sistema deve disponibilizar informações das vendas para relatórios financeiros. | Controle financeiro e contábil | Média | A validar |
| **RF-33** | O sistema deve manter o histórico de pedidos do cliente. | Rastreabilidade na área do cliente | Média | A validar |
| **RF-34** | O sistema deve permitir o gerenciamento de produtos, preços e estoque por usuários autorizados. | Manutenção do e-commerce | Alta | A validar |
| **RF-35** | O sistema deve permitir a consulta administrativa dos pedidos e de seus respectivos status. | Controle operacional integrado | Alta | A validar |

---

## 3. Regras de Negócio Associadas (A validar)

* **RN-01:** A baixa definitiva do estoque ocorrerá somente após o pagamento aprovado.
* **RN-02:** Pedidos com pagamento pendente poderão reservar estoque por um prazo determinado.
* **RN-03:** O pedido só poderá seguir para separação após a confirmação do pagamento.
* **RN-04:** As opções de parcelamento serão definidas e parametrizadas pela PavPlas.
* **RN-05:** O valor e prazo do frete dependerão do CEP de entrega, peso/dimensões dos produtos e tabela da transportadora.
* **RN-06:** Pagamentos recusados não gerarão ordem de separação nem emissão de NF-e.
