---
title: Gerenciamento de identidade privilegiada do Azure AD
description: Aqui está a lista dos métodos fornecidos pelo serviço de gerenciamento de identidade privilegiado.
localization_priority: Priority
ms.openlocfilehash: c1108711c96dd253f784a418a396ca30507c5f7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884060"
---
# <a name="azure-ad-privileged-identity-management"></a>Gerenciamento de identidade privilegiada do Azure AD

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Aqui está a lista dos métodos fornecidos pelo serviço de [Gerenciamento de identidade privilegiado](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) .

O serviço é criado na parte superior de OData. Para filtrar os resultados da consulta, use o OData standard ``$filter`` expressões nos URIs.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista privilegedOperationEvent](../api/privilegedoperationevent-list.md) | coleção [privilegedOperationEvent](privilegedoperationevent.md) |Obtenha a coleção de objetos privilegedOperationEvent. |
|[Obter privilegedRole](../api/privilegedrole-get.md) |[privilegedRole](privilegedrole.md)| Obtenha um objeto privilegedRole.|
|[Lista privilegedRole](../api/privilegedrole-list.md) | coleção [privilegedRole](privilegedrole.md) |Obtenha a coleção de objetos privilegedRole. |
|[Atribuições de função de lista](../api/privilegedrole-list-assignments.md) | coleção [privilegedRoleAssignment](privilegedroleassignment.md) |Obter a coleção de privilegedRoleAssignment para a função específica. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário.|
|[selfActivate](../api/privilegedrole-selfactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Ative a função que é atribuída ao solicitante.|
|[selfDeactivate](../api/privilegedrole-selfdeactivate.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Desative a função que é atribuída ao solicitante.|
|[Criar privilegedRoleAssignment](../api/privilegedroleassignment-post-privilegedroleassignments.md) |[privilegedRoleAssignment](privilegedroleassignment.md)| Crie um novo privilegedRoleAssignment (atribuição de função) pelo lançamento à coleção privilegedRoleAssignments.|
|[Lista privilegedRoleAssignment](../api/privilegedroleassignment-list.md) | coleção [privilegedRoleAssignment](privilegedroleassignment.md) |Obtenha a coleção de objetos privilegedRoleAssignment. A coleção contém todas as atribuições de função para a organização. Cada privilegedRoleAssignment representa uma atribuição de função a um usuário. |
|[Obter privilegedRoleAssignment](../api/privilegedroleassignment-get.md) | [privilegedRoleAssignment](privilegedroleassignment.md)|Obtenha o objeto privilegedRoleAssignment com a id de atribuição especificada. |
|[Excluir privilegedRoleAssignment](../api/privilegedroleassignment-delete.md) | Nenhum. |Exclua objeto privilegedRoleAssignment. |
|[makePermanent](../api/privilegedroleassignment-makepermanent.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Fazer a atribuição de função como permanente. |
|[makeEligible](../api/privilegedroleassignment-makeeligible.md) | [privilegedRoleAssignment](privilegedroleassignment.md) |Fazer a atribuição de função como qualificado. |
|[Minha](../api/privilegedroleassignment-my.md) | coleção [privilegedRoleAssignment](privilegedroleassignment.md)|Obtenha as atribuições de função do solicitador. |
|[Obter privilegedRoleSettings](../api/privilegedrolesettings-get.md) | [privilegedRoleSettings](../resources/privilegedrolesettings.md)|Recupere as propriedades do objeto privilegedRoleSettings. |
|[Obter privilegedRoleSummary](../api/privilegedrolesummary-get.md) | [privilegedRoleSummary](../resources/privilegedrolesummary.md)|Recupere o objeto privilegedRoleSummary. |
|[Obter privilegedApproval](../api/privilegedapproval-get.md) |[privilegedApproval](privilegedapproval.md)| Obtenha um objeto privilegedApproval.|
|[Lista privilegedApproval](../api/privilegedapproval-list.md) | coleção [privilegedApproval](privilegedapproval.md) |Obtenha a coleção de objetos privilegedApproval. |
|[Criar privilegedApproval](../api/privilegedapproval-post-privilegedapproval.md) | [privilegedApproval](privilegedapproval.md)    |Crie objeto privilegedApproval. |
|[Atualizar privilegedApproval](../api/privilegedapproval-update.md) | [privilegedApproval](privilegedapproval.md) |Atualize o objeto privilegedApproval. |
|[myrequests](../api/privilegedapproval-myrequests.md) | coleção [privilegedApproval](privilegedapproval.md)|Obtenha as solicitações de aprovação do solicitador. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
