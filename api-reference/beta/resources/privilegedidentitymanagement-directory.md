---
title: Privileged Identity Management - Azure AD
description: APIs do Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory.
localization_priority: Priority
ms.openlocfilehash: 6002b0cdd3ba177d5a3b236a28c9fe1937ae5de8
ms.sourcegitcommit: f80282ff00d5aafc3e575bce447543d7dd23963d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2019
ms.locfileid: "34425135"
---
# <a name="privileged-identity-management---azure-ad"></a>Privileged Identity Management - Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> A API para que o [Privileged Identity Management (PIM) do Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) gerencie funções do Azure AD sofrerá alterações entre junho e novembro de 2019 para acompanhar o namespace e a convenção da [API de recursos do Azure](privilegedidentitymanagement-resources.md). O PIM do Azure AD se tornará um recurso na convenção de recursos do Azure. Se essa alteração afetar diretamente seu locatário, preencha o [formulário de Mudança da API do Graph para PIM do Azure AD](https://forms.office.com/Pages/ResponsePage.aspx?id=v4j5cvGGr0GRqy180BHbRzfBSoy7dT5DqNLWwotW3OFUNFFMRlRLSUtRNEdDWEZHN05LT09IWjkyTS4u) para obter informações adicionais, suporte e a capacidade de agendar um horário para essa alteração da API.

Aqui está a lista de métodos fornecidos pelo PIM para funções do Azure AD. O serviço é criado com base no OData. Para filtrar os resultados de uma consulta, use as expressões OData ``$filter`` padrão nos URIs.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [privilegedOperationEvent](privilegedoperationevent.md) collection |Obtenha a coleção de objeto privilegedOperationEvent. |
|[Get privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Recupere um objeto privilegedRole.|
|[List privilegedRole](../api/privilegedrole-list.md) | [privilegedRole](privilegedrole.md) collection |Obtenha coleção de objeto privilegedRole. |
|[List role assignments](../api/privilegedrole-list-assignments.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection |Obtenha a coleção privilegedRoleAssignment para a função em particular. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Ative a função que é atribuída ao solicitante.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Desative a função que é atribuída ao solicitante.|
|[Create privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie uma nova privilegedRoleAssignment (atribuição de função) postando-a na coleção privilegedRoleAssignments.|
|[List privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection |Obtenha a coleção de objeto privilegedRoleAssignment. A coleção contém todas as atribuições de função da organização. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário. |
|[Get privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Obtenha o objeto privilegedRoleAssignment com a id da tarefa especificada. |
|[Delete privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | Nenhum. |Exclua um objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Torne a atribuição de função como permanente. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Tornar a atribuição de função como qualificada. |
|[my](../api/privilegedroleassignment-my.md) | [privilegedRoleAssignment](privilegedroleassignment.md) collection|Obtenha as atribuições de função do solicitante. |
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Recupere as propriedades do objeto privilegedRoleSettings. |
|[Get privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Recupere o objeto privilegedRoleSummary. |
|[Get privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Obtenha um objeto privilegedApproval.|
|[List privilegedApproval](../api/privilegedapproval-list.md) | [privilegedApproval](privilegedapproval.md) collection |Obtenha uma coleção de objeto privilegedApproval. |
|[Create privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Crie um objeto privilegedApproval. |
|[Update privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Atualize um objeto privilegedApproval. |
|[myrequests](../api/privilegedapproval-myrequests.md) | [privilegedApproval](privilegedapproval.md) collection|Receba solicitações de aprovação do solicitante. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
