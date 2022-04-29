---
title: Tipo de recurso unifiedRoleAssignmentScheduleInstance
description: Representa a instância de uma atribuição de função ativa em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb05f82d9f6cfc2ef88ee0104875caa88cd5a9ba
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133904"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleInstance

Namespace: microsoft.graph

Representa a instância de uma atribuição de função ativa em seu locatário. A atribuição ativa pode ter sido feita por meio de atribuições [de PIM e](../api/rbacapplication-post-roleassignmentschedulerequests.md) solicitações de ativação ou diretamente por meio da [API de atribuições de função](../resources/unifiedroleassignment.md).

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleInstances](../api/rbacapplication-list-roleassignmentscheduleinstances.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obtenha as instâncias de atribuições de função ativas.|
|[Obter unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obter a instância de uma atribuição de função ativa.|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obtenha as instâncias de atribuições de função ativas para a entidade de chamada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|assignmentType|Cadeia de caracteres|Tipo da atribuição que pode ser `Assigned` ou `Activated`. Suporta `$filter` (`eq`, `ne`).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset| A data de término da instância de agendamento.|
|id|Cadeia de caracteres|O identificador exclusivo do **objeto unifiedRoleAssignmentScheduleInstance** . Herdado da [entidade](../resources/entity.md).|
|Membertype|Cadeia de caracteres|Como as atribuições são herdadas. Pode ser `Inherited`, `Direct`ou `Group`. Isso pode implicar ainda se **o unifiedRoleAssignmentSchedule** pode ser gerenciado pelo chamador. Suporta `$filter` (`eq`, `ne`).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança que recebeu a atribuição de função. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`). |
|roleAssignmentOriginId|Cadeia de caracteres|O identificador da atribuição de função no Azure AD.|
|roleAssignmentScheduleId|Cadeia de caracteres|O identificador do **objeto unifiedRoleAssignmentSchedule** do qual essa instância foi criada.|
|roleDefinitionId|Cadeia de caracteres|O identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`).|
|startDateTime|DateTimeOffset|Quando essa instância é iniciada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Se a solicitação for de um administrador qualificado para ativar uma função, esse parâmetro mostrará a atribuição qualificada relacionada para essa ativação. Caso contrário, será `null`. Suporta o `$expand`.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. Anulável. Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da atribuição. Somente leitura. Oferece suporte para `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma atribuição de função por meio da solicitação. Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** . Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentType": "String",
  "memberType": "String",
  "roleAssignmentOriginId": "String",
  "roleAssignmentScheduleId": "String"
}
```

