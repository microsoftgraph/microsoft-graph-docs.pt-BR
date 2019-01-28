---
title: Azure AD Privileged Identity Management
description: Aqui está a lista de métodos fornecidos pelo serviço Privileged Identity Management.
localization_priority: Priority
ms.openlocfilehash: 59a049a299faf0b90baefef8eb44f0365fafa35e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515052"
---
# <a name="azure-ad-privileged-identity-management"></a>Azure AD Privileged Identity Management

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Aqui está a lista de métodos fornecidos pelo serviço [Privileged Identity Management](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-privileged-identity-management-configure/).

O serviço é criado com base no OData. Para filtrar os resultados da consulta, use as expressões ``$filter`` padrão do OData nos URIs.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedidentitymanagement-root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
