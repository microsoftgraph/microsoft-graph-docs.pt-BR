---
title: Tipo de recurso unifiedRoleAssignmentSchedule
description: Representa um agendamento para uma atribuição de função ativa em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7294918800c68857ca11ac41a7baf8fab7e4da5e
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133861"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>Tipo de recurso unifiedRoleAssignmentSchedule

Namespace: microsoft.graph

Representa um agendamento para uma atribuição de função ativa em seu locatário e é usado para instanciar [um unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). A atribuição ativa pode ter sido feita por meio de atribuições [de PIM e](../api/rbacapplication-post-roleassignmentschedulerequests.md) solicitações de ativação ou diretamente por meio da [API de atribuições de função](../resources/unifiedroleassignment.md).

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentSchedules](../api/rbacapplication-list-roleassignmentschedules.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Obtenha os agendamentos para operações de atribuição de função ativa.|
|[Obter unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Recupere o agendamento de uma operação de atribuição de função ativa.|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Recupere os agendamentos para operações de atribuição de função ativas para as quais o usuário conectado é a entidade de segurança.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|assignmentType|Cadeia de caracteres|Tipo da atribuição que pode ser `Assigned` ou `Activated`. Suporta `$filter` (`eq`, `ne`).|
|createdDateTime|DateTimeOffset|Quando a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Cadeia de caracteres|Identificador do **objeto unifiedRoleAssignmentScheduleRequest por** meio do qual essa agenda foi criada. Anulável. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|Cadeia de caracteres|O identificador exclusivo do **objeto unifiedRoleAssignmentScheduleRequest** . Suporta `$filter` (`eq`). Herdado da [entidade](../resources/entity.md).|
|Membertype|Cadeia de caracteres|Como as atribuições são herdadas. Pode ser `Inherited`, `Direct`ou `Group`. Isso pode implicar ainda se **o unifiedRoleAssignmentSchedule** pode ser gerenciado pelo chamador. Suporta `$filter` (`eq`, `ne`).|
|modifiedDateTime|DateTimeOffset|Quando a agenda foi modificada pela última vez. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a atribuição de função. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Suporta `$filter` (`eq`, `ne`).|
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Suporta `$filter` (`eq`, `ne`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O período da atribuição de função. Ele pode representar uma única ocorrência ou várias recorrências.|
|status|Cadeia de caracteres|O status do **objeto unifiedRoleAssignmentScheduleRequest** . Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). Os valores possíveis são: `Canceled`, `Denied`, `Failed`, `Granted`, `PendingAdminDecision`, , `PendingApproval`, `PendingProvisioning`, `PendingScheduleCreation`, `Provisioned`, , `Revoked`e `ScheduleCreated`. Não anulável. Suporta `$filter` (`eq`, `ne`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação. Caso contrário, será `null`. Suporta o `$expand`.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. Anulável. Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição. Somente leitura. Oferece suporte para `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** . Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "createdUsing": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "status": "String",
  "scheduleInfo": {
    "@odata.type": "microsoft.graph.requestSchedule"
  },
  "assignmentType": "String",
  "memberType": "String"
}
```

