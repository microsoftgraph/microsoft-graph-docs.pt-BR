---
title: Tipo de recurso rbacApplication
description: Contêiner para definições de função e atribuições de função Microsoft 365 provedores de RBAC (controle de acesso baseado em função)
ms.localizationpriority: medium
author: abhijeetsinha
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9949ea7f219cee7e92f2c1406fe140469d67ad8c
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133780"
---
# <a name="rbacapplication-resource-type"></a>Tipo de recurso rbacApplication

Namespace: microsoft.graph

Contêiner de gerenciamento de função para definições de função unificadas e atribuições de função Microsoft 365 provedores de RBAC (controle de acesso baseado em função). As atribuições de função dão suporte apenas a uma única entidade de segurança e um único escopo. Atualmente, **o diretório** **e o direitoManagement** são os dois provedores RBAC com suporte.

Herda de [entidade](../resources/entity.md).

## <a name="methods"></a>Methods

Nenhum

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do objeto. Herdado da [entidade](../resources/entity.md).|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|roleAssignments|[Coleção unifiedRoleAssignment](../resources/unifiedroleassignment.md)| Recurso para conceder acesso a usuários ou grupos. |
|roleAssignmentScheduleInstances|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)| Instâncias para atribuições de função ativas.  |
|roleAssignmentScheduleRequests|[Coleção unifiedRoleAssignmentScheduleRequest](../resources/unifiedroleassignmentschedulerequest.md)| Solicitações de atribuições de função ativas para entidades de segurança por meio do PIM. |
|roleAssignmentSchedules|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Agendamentos para operações de atribuição de função ativa.|
|roleDefinitions|[Coleção unifiedRoleDefinition](../resources/unifiedroledefinition.md)| Recurso que representa as funções permitidas pelos provedores RBAC e as permissões atribuídas às funções. |
|roleEligibilityScheduleInstances|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Instâncias para solicitações de elegibilidade de função.|
|roleEligibilityScheduleRequests|[Coleção unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md)| Solicitações de eligibilidades de função para entidades de segurança por meio do PIM.|
|roleEligibilitySchedules|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Agendamentos para operações de elegibilidade de função. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rbacApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "String (identifier)"
}
```
