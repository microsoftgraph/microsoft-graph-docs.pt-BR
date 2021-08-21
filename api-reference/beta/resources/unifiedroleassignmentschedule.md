---
title: Tipo de recurso unifiedRoleAssignmentSchedule
description: Representa um cronograma para operações de atribuição de função ativa por meio do Azure AD Privileged Identity Management.
author: shauliu1
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8e528fe7fd6508d8cc5c3eac23f1796731c50d5f
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453209"
---
# <a name="unifiedroleassignmentschedule-resource-type"></a>Tipo de recurso unifiedRoleAssignmentSchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o cronograma de uma atribuição de função ativa por meio do Azure AD Privileged Identity Management. Um **unifiedRoleAssignmentSchedule** é criado por [um unifiedRoleAssignmentScheduleRequest](unifiedroleassignmentschedulerequest.md) e é usado para insinciar um [unifiedRoleAssignmentScheduleInstance](unifiedroleassignmentscheduleinstance.md). Esse recurso dá suporte à lista e obter operações para recuperar a agenda para fins de exibição de atribuições atuais e futuras.

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleAssignmentSchedules](../api/unifiedroleassignmentschedule-list.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades.|
|[Obter unifiedRoleAssignmentSchedule](../api/unifiedroleassignmentschedule-get.md)|[unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Leia as propriedades e as relações de [um objeto unifiedRoleAssignmentSchedule.](../resources/unifiedroleassignmentschedule.md)|
|[filterByCurrentUser](../api/unifiedroleassignmentschedule-filterbycurrentuser.md)|[Coleção unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md)|Obter uma lista dos [objetos unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|assignmentType|Cadeia de caracteres|Tipo da atribuição. Pode ser `Assigned` ou `Activated` .|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|Cadeia de caracteres|ID da roleAssignmentScheduleRequest que criou essa agenda. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleAssignmentSchedule. Chave, não anulada, somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|Cadeia de caracteres|Tipo de associação da atribuição. Pode ser `Inherited` , `Direct` ou `Group` .|
|modifiedDateTime|DateTimeOffset|Última vez que a agenda foi atualizada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|Cadeia de caracteres| Objectid da entidade à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Suporta `$filter` (`eq`).|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para o que a atribuição se destina. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md). <br> Suporta `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função.|
|status|Cadeia de caracteres|Status do `roleAssignmentSchedule` . Pode incluir mensagens relacionadas ao `Provisioned` estado, `Revoked` como , , `Pending Provisioning` e `Pending Approval` . Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activatedUsing|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Se a funçãoAssignmentSchedule for ativada por uma roleEligibilitySchedule, este será o link para esse agendamento.|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Será preterido. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade indicando a funçãoDefinition para a qual a atribuição se destina. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

