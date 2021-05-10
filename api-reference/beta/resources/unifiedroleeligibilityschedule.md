---
title: Tipo de recurso unifiedRoleEligibilitySchedule
description: Representa um cronograma para operações de atribuição de função qualificada por meio do Azure AD Privileged Identity Management.
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1593e819b3c57ee24dae0480aadcb7f532d2fbf4
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52299069"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Tipo de recurso unifiedRoleEligibilitySchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o cronograma de uma atribuição de função qualificada por meio do Azure AD Privileged Identity Management. A `roleEligibilitySchedule` é criado por e é usado para `roleEligibilityScheduleRequest` insinuar um `roleEligibilityInstance` . Damos suporte à lista e fazemos operações recuperarem o agendamento para fins de exibição de atribuições qualificadas atuais e futuras.

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) e suas propriedades.|
|[Obter unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Leia as propriedades e as relações de [um objeto unifiedRoleEligibilitySchedule.](../resources/unifiedroleeligibilityschedule.md)|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|ID do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use "/" para o escopo de todo o locatário. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|createdUsing|Cadeia de caracteres|ID do RoleEligibilityScheduleRequest que criou essa agenda. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScopeId|Cadeia de caracteres|ID do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleEligibilitySchedule. Chave, não anulada, somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|memberType|Cadeia de caracteres|Tipo de associação da atribuição qualificada. Pode ser `Inherited` , `Direct` ou `Group` .|
|modifiedDateTime|DateTimeOffset|Última vez que a agenda foi atualizada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principalId|Cadeia de caracteres| Objectid da entidade à qual a atribuição qualificada está sendo concedida. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinitionId|Cadeia de caracteres|ID do unifiedRoleDefinition para a atribuição qualificada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função qualificada.|
|status|Cadeia de caracteres|Status do `roleEligibilitySchedule` . Pode incluir mensagens relacionadas ao `Provisioned` estado, `Revoked` como , , `Pending Provisioning` e `Pending Approval` . Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Será preterido. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição qualificada. Fornecido para que os chamadores possam obter o objeto de diretório usando `$expand` ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função qualificada por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a funçãoDefinition para a qual a atribuição qualificada é. Fornecido para que os chamadores possam obter a definição de função usando `$expand` ao mesmo tempo que obter a atribuição de função qualificada. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilitySchedule",
  "baseType": "microsoft.graph.unifiedRoleScheduleBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilitySchedule",
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
  "memberType": "String"
}
```

