---
title: Tipo de recurso unifiedRoleEligibilitySchedule
description: Representa um cronograma para uma operação de atribuição de função qualificada por meio do Azure AD Privileged Identity Management.
author: japere
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f446c5bed547fc4697c535b57f271e998c8ebfab
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510580"
---
# <a name="unifiedroleeligibilityschedule-resource-type"></a>Tipo de recurso unifiedRoleEligibilitySchedule

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o cronograma de uma atribuição de função qualificada por meio do Azure AD Privileged Identity Management. Um **unifiedRoleEligibilitySchedule** é criado por [unifiedRoleEligibilityScheduleRequest](unifiedroleeligibilityschedulerequest.md) e é usado para insinuar uma [unifiedRoleEligibilityScheduleInstance](unifiedroleeligibilityscheduleinstance.md). Esse recurso dá suporte às operações Lista e Obter para recuperar a agenda para fins de exibição de atribuições elegíveis atuais e futuras.

Herda de [unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilitySchedules](../api/unifiedroleeligibilityschedule-list.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) e suas propriedades.|
|[Obter unifiedRoleEligibilitySchedule](../api/unifiedroleeligibilityschedule-get.md)|[unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Leia as propriedades e as relações de [um objeto unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityschedule-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md)|Obter uma lista dos [objetos unifiedRoleEligibilitySchedule](../resources/unifiedroleeligibilityschedule.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|String|Identificador do escopo específico do aplicativo quando o escopo de atribuição for específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos do aplicativo são escopos definidos e compreendidos somente por esse aplicativo. Use `/` para escopos de aplicativos de todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdDateTime|DateTimeOffset|Hora em que a agenda foi criada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|createdUsing|Cadeia de caracteres|Identificador da funçãoEligibilityScheduleRequest que criou essa agenda. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto directory que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos para os quais a entidade foi concedida acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|id|Cadeia de caracteres|O identificador exclusivo para unifiedRoleEligibilitySchedule. Chave, não anulada, somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|memberType|Cadeia de caracteres|Tipo de associação da atribuição qualificada. Pode ser `Inherited`, `Direct`ou `Group`.|
|modifiedDateTime|DateTimeOffset|Última vez que a agenda foi atualizada. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).|
|principalId|String| Identificador da entidade à qual a atribuição qualificada está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se destina. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|
|scheduleInfo|[requestSchedule](../resources/requestschedule.md)|O objeto schedule da solicitação de atribuição de função qualificada.|
|status|Cadeia de caracteres|Status do `roleEligibilitySchedule`. Pode incluir mensagens relacionadas ao estado, `Provisioned`como , `Revoked`, `Pending Provisioning`e `Pending Approval`. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md).<br> Suporta `$filter` (`eq`).|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|activeInstance|[unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|Será preterido. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência ao objeto de diretório que é o escopo da atribuição qualificada. Fornecido para que os chamadores possam obter o objeto de diretório `$expand` usando ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade fazendo referência à entidade que está recebendo uma atribuição de função qualificada por meio da solicitação. Fornecido para que os chamadores possam obter a entidade principal `$expand` usando ao mesmo tempo que obter a atribuição de função qualificada. Somente leitura. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a funçãoDefinition para a qual a atribuição qualificada é. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter a atribuição de função qualificada. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleBase](../resources/unifiedroleschedulebase.md)|

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

