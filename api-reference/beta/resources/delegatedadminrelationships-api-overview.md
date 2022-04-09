---
title: Visão geral da API de DAP (privilégios de administrador delegado)
description: Os privilégios de administrador delegado permitem que os parceiros da Microsoft configurem e solicitem acesso granular e com limite de tempo aos ambientes de seus clientes, permitindo que os clientes apliquem um acesso menos privilegiado para parceiros da Microsoft.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 2c59e78f1b8f2da00eaf56b4d24c09cbad397941
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733259"
---
# <a name="delegated-admin-privileges-dap-api-overview"></a>Visão geral da API de DAP (privilégios de administrador delegado)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Como parte do ecossistema do Microsoft Partner Center, os parceiros da Microsoft nos programas Provedor de Soluções na Nuvem, Revendedor de Valor Agregado ou Assistente podem executar operações administrativas em seus locatários de clientes para ajudar a gerenciar os serviços do cliente, por exemplo, o Azure AD e o Microsoft 365. Essa funcionalidade anteriormente permitia que os parceiros assumiam uma função de Administrador Global no locatário do cliente indefinidamente, criando possíveis exposições de segurança e limitando o potencial do mercado.

**Os DAP (privilégios** de administrador delegado) fornecem aos parceiros acesso menos privilegiado aos locatários do cliente seguindo o [Confiança Zero de segurança cibernética.](/security/zero-trust/) Por meio do DAP, os parceiros configuram e solicitam acesso granular e com limite de tempo aos ambientes de seus clientes, e os clientes devem conceder explicitamente esse acesso menos privilegiado aos parceiros. Além disso, os parceiros devem solicitar funções específicas para a administração de locatários do cliente por um período definido. Esse controle elimina a necessidade de que os parceiros tenham a função de Administrador Global no locatário do cliente, mas, em vez disso, eles agora têm permissões menos privilegiadas de que precisam absolutamente para tarefas administrativas delegadas.

Para obter mais informações sobre o DAP, consulte:
+ [Introdução aos privilégios de administrador delegado granular (GDAP)](/partner-center/gdap-introduction)
+ [Funções com privilégios mínimos por tarefa](/partner-center/gdap-least-privileged-roles-by-task)

## <a name="use-cases-for-delegated-admin-apis"></a>Casos de uso para APIs de administrador delegado

Esta seção descreve as maneiras pelas quais os parceiros da Microsoft podem gerenciar programaticamente as relações de administrador delegado para seus clientes.

### <a name="delegated-admin-relationship"></a>Relação de administrador delegado

| Casos de uso | APIs |
|--|--|
| Criar uma nova relação de administrador delegado para aprovação por qualquer cliente <br/> Criar uma nova relação de administrador delegado para aprovação por um cliente específico | [Criar delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md) |
| Listar todas as relações de administrador delegado de um parceiro <br/> Listar todas as relações de administrador delegado para um cliente específico | [Listar delegatedAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md) |
| Obter uma relação de administrador delegado por ID | [Obter delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)  |
| Excluir relação de administrador delegado | [Excluir delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md) |

### <a name="delegated-admin-relationship-request"></a>Solicitação de relação de administrador delegado

| Casos de uso | APIs |
|--|--|
| Crie uma solicitação de relação de administrador delegado para bloquear uma relação para aprovação do cliente ou encerrar uma relação existente. | [Criar solicitações](../api/delegatedadminrelationship-post-requests.md) |
| Obter uma solicitação de relação de administrador delegado por ID | [Obter delegatedAdminRelationshipRequest](../api/delegatedadminrelationshiprequest-get.md) |
| Listar todas as solicitações de relação de administrador delegado para uma determinada relação | [Listar solicitações](../api/delegatedadminrelationship-list-requests.md) |


### <a name="role-assignments"></a>Atribuições de função

| Casos de uso | APIs |
|--|--|
| Criar nova atribuição de acesso de administrador delegado para uma relação de administrador delegado | [Criar accessAssignments](../api/delegatedadminrelationship-post-accessassignments.md) |
| Listar atribuições de acesso para uma relação de administrador delegado | [Listar accessAssignments](../api/delegatedadminrelationship-list-accessassignments.md) |
| Obter uma atribuição de acesso de relação de administrador delegado por ID | [Obter delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-get.md) |
| Excluir uma atribuição de acesso de uma relação de administrador delegado | [Excluir delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-delete.md) |
| Atualizar atribuições de função para uma atribuição de acesso de relação de administrador delegado | [Atualizar delegatedAdminAccessAssignment](../api/delegatedadminaccessassignment-update.md) |

### <a name="long-running-operations"></a>Operações de execução longa

| Casos de uso | APIs |
|--|--|
| Listar todas as operações de execução longa de uma relação de administrador delegado | [Listar operações](../api/delegatedadminrelationship-list-operations.md) |
| Obter uma operação de execução longa de uma relação de administrador delegado | [Obter delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md) |


### <a name="delegated-admin-customers"></a>Clientes administradores delegados

| Casos de uso | APIs |
|--|--|
| Listar todos os clientes administradores delegados | [Listar delegatedAdminCustomers](../api/tenantrelationship-list-delegatedadmincustomers.md)|
| Obter um único cliente administrador delegado por ID | [Obter delegatedAdminCustomer](../api/delegatedadmincustomer-get.md) |
| Obter detalhes de gerenciamento de serviços para um cliente administrador delegado | [Listar serviceManagementDetails](../api/delegatedadmincustomer-list-servicemanagementdetails.md) |

## <a name="permissions"></a>Permissões

Para gerenciar relações de administrador delegado, a entidade de chamada deve estar no locatário do parceiro e receber as permissões [apropriadas](/graph/permissions-reference#delegated-admin-relationship-permissions) de privilégios de administrador delegado.
