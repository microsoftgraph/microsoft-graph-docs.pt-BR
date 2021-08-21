---
title: Tipo de recurso unifiedRoleAssignmentScheduleInstance
description: Representa uma instância de agendamento para operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 64ccc65b7daf312ee79bbc5bed032ceaafd956f8
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453181"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleInstance

Namespace: microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a instância de uma atribuição de função ativa por meio do Azure AD Privileged Identity Management. Uma **unifiedRoleAssignmentScheduleInstance** é criada por [unifiedRoleAssignmentSchedule](unifiedroleassignmentschedule.md) e representa uma atribuição de função real criada por meio de Privileged Identity Management. Esse recurso dá suporte às operações Lista e Obter para fins de exibição de atribuições atuais e futuras.

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentScheduleInstances](../api/unifiedroleassignmentscheduleinstance-list.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obter uma lista dos [objetos unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md) e suas propriedades.|
|[Obter unifiedRoleAssignmentScheduleInstance](../api/unifiedroleassignmentscheduleinstance-get.md)|[unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentScheduleInstance.](../resources/unifiedroleassignmentscheduleinstance.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentScheduleInstance](../resources/unifiedroleassignmentscheduleinstance.md)|Obter uma lista dos objetos [unifiedRoleAssignmentScheduleInstance](../resources/unifiedRoleAssignmentScheduleInstance.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|assignmentType|Cadeia de caracteres|Tipo da atribuição. Pode ser `Assigned` ou `Activated` .|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada.|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|Tempo em que a roleAssignmentInstance expirará|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulada, somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|Cadeia de caracteres|Tipo de associação da atribuição. Pode ser `Inherited` , `Direct` ou `Group` .|
|principalId|Cadeia de caracteres|Identificador da entidade à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleAssignmentOriginId|Cadeia de caracteres|ID do roleAssignment no diretório|
|roleAssignmentScheduleId|Cadeia de caracteres|ID da função paiAssignmentSchedule para esta instância|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).  <br> Suporta `$filter` (`eq`).|
|startDateTime|DateTimeOffset|Hora em que a roleAssignmentInstance será iniciar|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Se a roleAssignmentScheduleInstance for ativada por uma roleEligibilityScheduleRequest, este será o link para a instância de agendamento relacionada.|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

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

