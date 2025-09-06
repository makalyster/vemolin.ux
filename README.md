# vemolin.ux

### **Requisitos funcionais**

| **Código** | **Descrição**                                                                                                  | **Ator**         | **Prioridade** | **Observações**                                        |
| ---------- | -------------------------------------------------------------------------------------------------------------- | ---------------- | -------------- | ------------------------------------------------------ |
| RF1.1      | Permitir login no sistema usando usuário e senha.                                                              | Todo funcionário | Alta           | Validação de credenciais obrigatória                   |
| RF1.2      | Permitir logout do sistema.                                                                                    | Todo funcionário | Alta           | Deve encerrar sessão corretamente                      |
| RF1.3      | Identificar cargo do funcionário ao autenticar e exibir funcionalidades correspondentes.                       | Todo funcionário | Alta           | Define permissões de acesso                            |
| RF2.1      | Consultar preço de produtos.                                                                                   | Caixa            | Alta           | Inclui consulta por código ou nome do produto          |
| RF2.2      | Abrir uma transação de venda.                                                                                  | Caixa            | Alta           | Inicia registro de itens e pagamentos                  |
| RF2.3.1    | Adicionar produtos à venda.                                                                                    | Caixa            | Alta           | Inclui produtos cadastrados no sistema                 |
| RF2.3.2    | Remover produtos da venda antes da finalização.                                                                | Caixa            | Alta           | Só permitido antes de registrar pagamento              |
| RF2.3.3    | Pesar produto adicionado quando aplicável.                                                                     | Caixa            | Média          | Para produtos vendidos por peso (ex.: frutas)          |
| RF2.3.4    | Cancelar a venda antes da finalização.                                                                         | Caixa            | Alta           | Deve registrar usuário que cancelou                    |
| RF2.3.5    | Registrar forma de pagamento (dinheiro, cartão, Pix).                                                          | Caixa            | Alta           | Permitir múltiplos meios no mesmo pagamento            |
| RF2.3.6    | Confirmar pagamento e calcular troco automaticamente, quando aplicável.                                        | Caixa            | Alta           | Troco calculado somente para pagamento em dinheiro     |
| RF2.4      | Registrar a venda no sistema após pagamento.                                                                   | Caixa            | Alta           | Atualiza estoque automaticamente                       |
| RF3.1      | Registrar entrada de produtos no estoque.                                                                      | Estoquista       | Alta           | Registrar quantidade, fornecedor e validade            |
| RF3.2      | Registrar saída de produtos do estoque.                                                                        | Estoquista       | Alta           | Registrar motivo (venda, perda, doação, etc.)          |
| RF3.3      | Editar registro de estoque, incluindo ajuste de quantidade.                                                    | Estoquista       | Média          | Ajustes devem ser auditáveis                           |
| RF3.4      | Consultar informações de produtos no estoque.                                                                  | Estoquista       | Média          | Inclui quantidade, validade e fornecedor               |
| RF4.1      | CRUD de produtos (criar, ler, atualizar, deletar).                                                             | Gerente          | Alta           | Define produtos disponíveis para venda                 |
| RF4.2      | CRUD de usuários, incluindo atribuição de cargo.                                                               | Gerente          | Alta           | Define permissões do sistema                           |
| RF4.3      | CRUD de fornecedores.                                                                                          | Gerente          | Média          | Inclui registro mesmo que fornecedor não use o sistema |
| RF4.4      | Sistema notifica automaticamente gerente quando produto estiver com estoque baixo.                             | Gerente          | Alta           | Notificação indica qual produto precisa ser comprado   |
| RF4.5      | Gerente entra em contato com fornecedor correspondente ao produto com estoque baixo.                           | Gerente          | Média          | Sistema registra informações de contato do fornecedor  |
| RF5.1      | Sistema exibe somente funcionalidades permitidas ao cargo do funcionário logado.                               | Todo funcionário | Alta           | Controle de permissões baseado em cargo                |
| RF5.2      | Registrar todas operações de estoque e vendas com data, hora e usuário responsável.                            | Todo funcionário | Alta           | Para auditoria                                         |
| RF5.3      | Manter histórico de vendas e movimentações de estoque para consulta futura.                                    | Todo funcionário | Média          | Inclui consulta por período, produto e usuário         |
| RF5.4      | Validar quantidade em estoque ao adicionar produto à venda ou registrar saída.                                 | Todo funcionário | Alta           | Evita vendas ou saídas acima do disponível             |
| RF5.5      | Validar dados obrigatórios antes de salvar registros (produto, usuário, fornecedor, entrada/saída de estoque). | Todo funcionário | Alta           | Impede salvar registros incompletos                    |

