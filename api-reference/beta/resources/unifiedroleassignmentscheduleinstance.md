---
title: Tipo de recurso unifiedRoleAssignmentScheduleInstance
description: Representa a instância de uma atribuição de função ativa em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ea3ca59ac20369069d5a32fd554c29783db3e3f8
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898375"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleInstance

Namespace: microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a instância de uma atribuição de função ativa em seu locatário. A atribuição ativa pode ter sido feita por meio de atribuições [de PIM e](../api/rbacapplication-post-roleassignmentschedulerequests.md) solicitações de ativação ou diretamente por meio da [API de atribuições de função](../resources/unifiedroleassignment.md).

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleInstances](../api/rbacapplication-list-roleassignmentscheduleinstances.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obtenha as instâncias de atribuições de função ativas.|
|[Obter unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obter a instância de uma atribuição de função ativa.|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obtenha as instâncias de atribuições de função ativas para a entidade de chamada.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de Caracteres|Identificador do escopo específico do aplicativo quando a atribuição está no escopo de um aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|assignmentType|Cadeia de Caracteres|Tipo da atribuição que pode ser `Assigned` ou `Activated`. Suporta `$filter` (`eq`, `ne`).|
|directoryScopeId|String|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Dá `$filter` suporte (`eq`e `ne`em `null` valores). Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset| A data de término da instância de agendamento.|
|id|String|O identificador exclusivo do **objeto unifiedRoleAssignmentScheduleInstance** . Herdado da [entidade](../resources/entity.md).|
|Membertype|String|Como as atribuições são herdadas. Pode ser `Inherited`, `Direct`ou `Group`. Isso pode implicar ainda se **o unifiedRoleAssignmentSchedule** pode ser gerenciado pelo chamador. Suporta `$filter` (`eq`, `ne`).|
|principalId|Cadeia de Caracteres|Identificador da entidade de segurança que recebeu a atribuição de função. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`). |
|roleAssignmentOriginId|Cadeia de Caracteres|O identificador da atribuição de função no Azure AD.|
|roleAssignmentScheduleId|Cadeia de Caracteres|O identificador do **objeto unifiedRoleAssignmentSchedule** do qual essa instância foi criada.|
|roleDefinitionId|Cadeia de Caracteres|O identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) que está sendo atribuído à entidade de segurança. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`).|
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

