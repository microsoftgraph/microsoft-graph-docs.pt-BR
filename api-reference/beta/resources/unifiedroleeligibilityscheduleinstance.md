---
title: Tipo de recurso unifiedRoleEligibilityScheduleInstance
description: Representa uma instância de agendamento para operações de atribuição de função qualificadas por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c5199cd5f0a21c8aaabcabb88435118722d0fbe8
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399128"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a instância de uma atribuição de função qualificada por meio Azure AD Privileged Identity Management. Uma **unifiedRoleEligibilityScheduleInstance** é criada por [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) e representa uma Atribuição de função qualificada real criada por meio de Privileged Identity Management. Esse recurso dá suporte às operações listar e obter com a finalidade de exibir atribuições atuais e futuras.

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleInstances](../api/unifiedroleeligibilityscheduleinstance-list.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) e suas propriedades.|
|[Obter unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Leia as propriedades e as relações de um [objeto unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityInstance](../resources/unifiedroleeligibilityscheduleinstance.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|Cadeia de caracteres|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|directoryScopeId|Cadeia de caracteres|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset|Hora em que a roleEligibilityScheduleInstance expirará.|
|id|Cadeia de caracteres|O identificador exclusivo para roleEligibilityScheduleInstance. Chave, não anulável, somente leitura.Herdada de [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|Membertype|Cadeia de caracteres|Tipo de associação da atribuição. Pode ser `Inherited`, `Direct`ou `Group`.|
|principalId|Cadeia de caracteres|Identificador da entidade de segurança à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|roleDefinitionId|Cadeia de caracteres|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).<br> Suporta `$filter` (`eq`).|
|roleEligibilityScheduleId|Cadeia de caracteres|Identificador da roleEligibilitySchedule pai para esta instância.|
|startDateTime|DateTimeOffset|Hora em que a roleEligibilityScheduleInstance será iniciada.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|Propriedade somente leitura com detalhes do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. Entidade de contenção. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|directoryScope|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência ao objeto de diretório que é o escopo da atribuição. Fornecido para que os chamadores possam obter o objeto de `$expand` diretório usando ao mesmo tempo que obter as atribuições de função qualificadas. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|principal|[directoryObject](../resources/directoryobject.md)|Propriedade que faz referência à entidade de segurança que está obtendo uma atribuição de função qualificada por meio da solicitação. Fornecido para que os chamadores possam obter a entidade `$expand` de segurança usando ao mesmo tempo que obter as atribuições de função qualificadas. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Propriedade que indica a roleDefinition para a atribuição. Fornecido para que os chamadores possam obter a definição de função `$expand` usando ao mesmo tempo que obter as atribuições de função qualificadas. roleDefinition.Id será expandido automaticamente. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md)|

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

