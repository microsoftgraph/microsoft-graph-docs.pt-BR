---
title: Tipo de recurso unifiedRoleAssignmentScheduleInstance
description: Representa uma instância de agendamento para operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff3f2553c08098d118aa1391ab33ab63c5bd784f
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299111"
---
# <a name="unifiedroleassignmentscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleAssignmentScheduleInstance

Namespace: microsoft.graph 

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a instância de uma atribuição de função ativa por meio do Azure AD Privileged Identity Management. Um `roleAssignmentInstance` é criado por e representa uma função `roleAssignmentSchedule` realAssignment criada por Privileged Identity Management. Suportamos lista e fazemos operações na funçãoAssignmentInstance com o objetivo de exibir atribuições atuais e futuras.

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
|appScopeId|Cadeia de caracteres|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|assignmentType|Cadeia de caracteres|Tipo da atribuição. Pode ser `Assigned` ou `Activated` .|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada.|
|directoryScopeId|Cadeia de caracteres|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|endDateTime|DateTimeOffset|Tempo em que a roleAssignmentInstance expirará|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentScheduleInstance. Chave, não anulada, somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|memberType|Cadeia de caracteres|Tipo de associação da atribuição. Pode ser `Inherited` , `Direct` ou `Group` .|
|principalId|Cadeia de caracteres|Objectid da entidade à qual a atribuição está sendo concedida. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleAssignmentOriginId|Cadeia de caracteres|ID do roleAssignment no diretório|
|roleAssignmentScheduleId|Cadeia de caracteres|ID da função paiAssignmentSchedule para esta instância|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|startDateTime|DateTimeOffset|Hora em que a roleAssignmentInstance será iniciar|

## <a name="relationships"></a>Relações
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

