---
title: Privileged Identity Management - Azure AD
description: APIs do Privileged Identity Management do Azure AD para gerenciar as funções do Azure Active Directory.
localization_priority: Priority
author: shauliu1
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 1d9b84b5f3ab8831204888b4a8946da5e64bb5db
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453888"
---
# <a name="privileged-identity-management---azure-ad"></a>Privileged Identity Management - Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!IMPORTANT]
> A API para gerenciar as funções do Azure Active Directory foi preterida para a maioria dos locatários, exceto para poucos que usam uma versão mais antiga da Gestão de Identidade Privilegiada (PIM). Para obter mais informações sobre as versões do PIM, confira [Determinar sua versão do PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?tabs=new#determine-your-version-of-pim). Se estiver usando a nova versão e recebendo o erro **TenantEnabledInAadRoleMigration**, você pode aguardar até que uma nova API esteja disponível para a funcionalidade PIM na API [unifiedRoleManagement](/graph/api/resources/unifiedroledefinition?view=graph-rest-beta) para funções do Azure Active Directory ou você pode use a API de [Recursos do Azure](/graph/api/resources/privilegedidentitymanagement-resources?view=graph-rest-beta) para suas funções do Azure Active Directory. Para usar a API de **recurso do Azure**, substitua `azureResources` por `aadRoles` para `provider_id` e use o seu ID de locatário para `resource_id`. Recomendamos que você aguarde a nova API. Você poderá continuar usando a API de **recursos do Azure** depois que a nova API estiver disponível. Quaisquer novos recursos disponibilizados no portal do Azure também serão disponibilizados exclusivamente por meio da nova API. 

Os métodos a seguir são fornecidos pelo PIM para funções do Microsoft Azure Active Directory. O serviço é criado com base no OData. Para filtrar os resultados de uma consulta, use as expressões OData ``$filter`` padrão nos URIs.

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
