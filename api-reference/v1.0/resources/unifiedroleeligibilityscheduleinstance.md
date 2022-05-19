---
title: Tipo de recurso unifiedRoleEligibilityScheduleInstance
description: Representa a instância de uma qualificação de função em seu locatário.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: e219bdce8f3cc5c2ec83d8cecf7b9b779a8ed782
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549292"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleInstance

Namespace: microsoft.graph

Representa a instância de uma qualificação de função em seu locatário.

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleInstances](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha as instâncias de eligibilidades de função.|
|[Obter unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obter a instância de uma qualificação de função.|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha as instâncias de funções qualificadas para a entidade de chamada.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. O escopo da qualificação de função determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da elegibilidade da função. O escopo da qualificação de função determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Dá `$filter` suporte (`eq`e `ne`em `null` valores).|
|endDateTime|DateTimeOffset|A data de término da instância de agendamento.|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de agendamento. Herdado da [entidade](../resources/entity.md).|
|Membertype|Cadeia de caracteres|Como a elegibilidade de função é herdada. Pode ser `Inherited`, `Direct`ou `Group`. Isso pode implicar ainda se **o unifiedRoleEligibilitySchedule** pode ser gerenciado pelo chamador. Suporta `$filter` (`eq`, `ne`).|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança qualificada para uma função. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`). |
|roleDefinitionId|Cadeia de caracteres|Identificador do [objeto unifiedRoleDefinition](unifiedroledefinition.md) para o qual a entidade de segurança está qualificada. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta `$filter` (`eq`, `ne`).|
|roleEligibilityScheduleId|String|O identificador do **objeto unifiedRoleEligibilitySchedule** do qual essa instância foi criada. Suporta `$filter` (`eq`, `ne`).|
|startDateTime|DateTimeOffset|Quando essa instância é iniciada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando a elegibilidade de função está no escopo de um aplicativo. Anulável. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta o `$expand`.|
|directoryScope|[directoryObject](../resources/directoryobject.md)|O objeto de diretório que é o escopo da qualificação de função. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta o `$expand`.|
|principal|[directoryObject](../resources/directoryobject.md)|A entidade de segurança que está obtendo uma qualificação de função por meio da solicitação. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta o `$expand`.|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Informações detalhadas para o objeto roleDefinition referenciado por meio da **propriedade roleDefinitionId** . Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md). Suporta o `$expand`.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "baseType": "microsoft.graph.unifiedRoleScheduleInstanceBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleEligibilityScheduleInstance",
  "id": "String (identifier)",
  "principalId": "String",
  "roleDefinitionId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "memberType": "String",
  "roleEligibilityScheduleId": "String"
}
```

