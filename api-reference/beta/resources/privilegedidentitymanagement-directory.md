---
title: Privileged Identity Management - Azure AD
description: APIs do Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory.
ms.localizationpriority: high
author: carolinetempleton
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 900038e9c68517ac42ade68218b55d7cc52450f9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688777"
---
# <a name="privileged-identity-management---azure-ad-deprecated"></a>Privileged Identity Management - Azure AD (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Os métodos a seguir são fornecidos pelo PIM para funções do Microsoft Azure Active Directory. O serviço é criado com base no OData. Para filtrar os resultados de uma consulta, use as expressões OData `$filter` padrão nos URIs.

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
