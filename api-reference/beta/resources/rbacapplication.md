---
title: Tipo de recurso rbacApplication
description: Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para Microsoft 365 provedores RBAC.
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e6157355fe71d0643c9fff354a4932fc020a9ffd
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58454182"
---
# <a name="rbacapplication-resource-type"></a>Tipo de recurso rbacApplication

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função para Microsoft 365 provedores RBAC. Atualmente, o gerenciamento de diretórios e direitos são os únicos aplicativos RBAC com suporte.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar unifiedRoleAssignment](../api/rbacapplication-post-roleassignments.md) | [unifiedRoleAssignment](unifiedroleassignment.md) | Crie um novo unifiedRoleAssignment postando na coleção roleAssignments. |
| [Listar roleAssignments](../api/rbacapplication-list-roleassignments.md) | [Coleção unifiedRoleAssignment](unifiedroleassignment.md) | Obter uma coleção de objetos unifiedRoleAssignment. Somente instâncias específicas podem ser consultadas, filtrando-se roleDefitionId ou principalId. |
| [Criar unifiedRoleDefinition](../api/rbacapplication-post-roledefinitions.md) | [unifiedRoleDefinition](unifiedroledefinition.md) | Crie um novo unifiedRoleDefinition postando na coleção roleDefinitions. |
| [Listar roleDefinitions](../api/rbacapplication-list-roledefinitions.md) | [Coleção unifiedRoleDefinition](unifiedroledefinition.md) | Obter uma coleção de objetos unifiedRoleDefinition. |
| [roleSchedules](../api/rbacapplication-roleschedules.md) | [Coleção unifiedRoleScheduleBase](unifiedroleschedulebase.md) | Função para recuperar uma coleção de objetos unifiedRoleScheduleBase. |
| [roleScheduleInstances](../api/rbacapplication-rolescheduleinstances.md) | [Coleção unifiedRoleScheduleInstanceBase](unifiedrolescheduleinstancebase.md) | Função para recuperar uma coleção de objetos unifiedRoleScheduleInstanceBase.  |

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|[Coleção unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Recurso para conceder acesso a usuários ou grupos. |
|roleDefinitions|[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Recurso que representa as funções permitidas pelos provedores RBAC e as permissões atribuídas às funções. |
|roleAssignmentApprovals|[coleção approval](../resources/approval.md)| Decisões associadas a uma aprovação de atribuição de função.|
|roleAssignmentScheduleInstances|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)| Instâncias para atribuições de função ativa por meio do Azure AD Privileged Identity Management.  |
|roleAssignmentScheduleRequests|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Solicitações de atribuições de função ativa por meio do Azure AD Privileged Identity Management. |
|roleAssignmentSchedules|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedRoleAssignmentSchedule.md)| Agendar atribuições de função ativa por meio do Azure AD Privileged Identity Management. |
|roleEligibilityScheduleInstances|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedRoleEligibilityScheduleInstance.md)| Instâncias de atribuições de função qualificadas por meio do Azure AD Privileged Identity Management. |
|roleEligibilityScheduleRequests|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedRoleEligibilityScheduleRequest.md)| Solicitações de atribuições de função qualificadas por meio do Azure AD Privileged Identity Management. |
|roleEligibilitySchedules|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedRoleEligibilitySchedule.md)| Agendar atribuições de função qualificadas por meio do Azure AD Privileged Identity Management. |



## <a name="json-representation"></a>Representação JSON

Nenhum

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rbacApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


