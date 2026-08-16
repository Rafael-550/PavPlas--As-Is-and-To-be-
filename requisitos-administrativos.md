# Requisitos Administrativos e de Gestão (Backoffice) - PavPlas

## 1. Identificação
* **Projeto:** Gateway de Pagamento e E-commerce PavPlas
* **Documento:** Levantamento de Requisitos Administrativos (Backoffice)
* **Status:** Levantamento preliminar (A validar)
* **Público-alvo interno:** Administradores, Operadores de Estoque, Equipe Fiscal/ERP, Financeiro e Atendimento.

---

## 2. Tabela de Requisitos Administrativos

| ID | Requisito Administrativo | Módulo / Setor | Descrição / Regra de Uso | Prioridade |
|---|---|---|---|---|
| **RAD-01** | O sistema deve permitir o controle de acesso baseado em perfis (RBAC). | Segurança / Acesso | Diferenciar permissões entre Administrador, Financeiro, Fiscal, Estoque e Atendimento. | Alta |
| **RAD-02** | O sistema deve permitir a autenticação segura com registro de logs de auditoria. | Segurança / Auditoria | Registrar ações críticas (ex: alterações de preços, cancelamento de pedidos, estornos manuais). | Alta |
| **RAD-03** | O sistema deve permitir o cadastro, edição e inativação de produtos e categorias. | Catálogo / Produtos | Gestão de fotos, descrições, preços, dimensões, peso e status de visibilidade na loja. | Alta |
| **RAD-04** | O sistema deve permitir o ajuste manual e o controle de saldo de estoque. | Estoque / Inventário | Ajustar quantidades por entrada de mercadoria, perda, avaria ou inventário periódico. | Alta |
| **RAD-05** | O sistema deve emitir alerta administrativo quando o estoque atingir o nível mínimo configurado. | Estoque / Alertas | Notificar os operadores sobre a necessidade de reposição de itens em baixa quantidade. | Média |
| **RAD-06** | O sistema deve permitir a visualização e gestão centralizada do ciclo de vida dos pedidos. | Gestão de Pedidos | Filtrar e consultar pedidos por status: *Pendente, Pago, Em Separação, Faturado, Enviado, Concluído, Cancelado*. | Alta |
| **RAD-07** | O sistema deve permitir a alteração manual justificada de status do pedido por operadores autorizados. | Gestão de Pedidos | Possibilitar intervenções operacionais (ex: cancelamento por solicitação do cliente). | Alta |
| **RAD-08** | O sistema deve permitir a configuração e parametrização das taxas e regras do gateway de pagamento. | Financeiro / Gateway | Configurar credenciais de API, número máximo de parcelas sem juros, desconto para PIX/boleto e prazos de expiração. | Alta |
| **RAD-09** | O sistema deve exibir o painel de conciliação financeira de vendas. | Financeiro / Relatórios | Comparar valores brutos, taxas do gateway, valores líquidos a receber e status de liquidação. | Alta |
| **RAD-10** | O sistema deve permitir o reenvio manual de notificações (e-mail/WhatsApp) e links de pagamento. | Atendimento / Suporte | Gerar novamente e reenviar links de PIX, boleto ou segunda via de comprovante ao cliente. | Média |
| **RAD-11** | O sistema deve permitir a integração e sincronização manual/automática com o sistema ERP. | Integração Fiscal/ERP | Monitorar a fila de envio de pedidos para faturamento e status da emissão de NF-e. | Alta |
| **RAD-12** | O sistema deve disponibilizar relatórios gerenciais e dashboards operacionais. | Gestão / BI | Relatórios de vendas por período, produtos mais vendidos, ticket médio, abandono de carrinho e faturamento por modalidade. | Média |
| **RAD-13** | O sistema deve permitir o gerenciamento de tabelas de frete e regras de envio. | Logística / Expedição | Parametrizar transportadoras parceiras, prazos adicionais de manuseio e taxas de frete fixo/regional. | Média |
