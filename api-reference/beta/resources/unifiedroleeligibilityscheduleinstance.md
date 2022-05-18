---
title: Tipo de recurso unifiedRoleEligibilityScheduleInstance
description: Representa uma instância de agendamento para operações de atribuição de função qualificadas por meio Azure AD Privileged Identity Management.
author: rkarim-ms
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0875c1a4e4c87805e6193265321ca9cd3b61c16d
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461356"
---
# <a name="unifiedroleeligibilityscheduleinstance-resource-type"></a>Tipo de recurso unifiedRoleEligibilityScheduleInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a instância de uma atribuição de função qualificada por meio Azure AD Privileged Identity Management. Uma **unifiedRoleEligibilityScheduleInstance** é criada por [unifiedRoleEligibilitySchedule](unifiedroleeligibilityschedule.md) e representa uma Atribuição de função qualificada real criada por meio de Privileged Identity Management. Esse recurso dá suporte às operações listar e obter com a finalidade de exibir atribuições atuais e futuras.

Herda [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar unifiedRoleEligibilityScheduleInstances](../api/rbacapplication-list-roleeligibilityscheduleinstances.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) e suas propriedades.|
|[Obter unifiedRoleEligibilityScheduleInstance](../api/unifiedroleeligibilityscheduleinstance-get.md)|[unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Leia as propriedades e as relações de um [objeto unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md) .|
|[filterByCurrentUser](../api/unifiedroleeligibilityscheduleinstance-filterbycurrentuser.md)|[Coleção unifiedRoleEligibilityScheduleInstance](../resources/unifiedroleeligibilityscheduleinstance.md)|Obtenha uma lista dos [objetos unifiedRoleEligibilityInstance](../resources/unifiedroleeligibilityscheduleinstance.md) e suas propriedades concedidas a um usuário específico.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|appScopeId|String|Identificador do escopo específico do aplicativo quando o escopo de atribuição é específico do aplicativo. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos do aplicativo são escopos definidos e compreendidos apenas por esse aplicativo. Use `/` para escopos de aplicativo em todo o locatário. Use **directoryScopeId** para limitar o escopo a objetos de diretório específicos, por exemplo, unidades administrativas. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|directoryScopeId|String|Identificador do objeto de diretório que representa o escopo da atribuição. O escopo de uma atribuição determina o conjunto de recursos aos quais a entidade de segurança recebeu acesso. Os escopos de diretório são escopos compartilhados armazenados no diretório que são compreendidos por vários aplicativos. Use `/` para escopo de todo o locatário. Use **appScopeId** para limitar o escopo somente a um aplicativo. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|endDateTime|DateTimeOffset|Hora em que a roleEligibilityScheduleInstance expirará.|
|id|String|O identificador exclusivo para roleEligibilityScheduleInstance. Chave, não anulável, somente leitura.Herdada de [unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|Membertype|String|Tipo de associação da atribuição. Pode ser `Inherited`, `Direct`ou `Group`.|
|principalId|String|Identificador da entidade de segurança à qual a atribuição está sendo concedida. Pode ser um grupo ou um usuário. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).|
|roleDefinitionId|String|Identificador do unifiedRoleDefinition para o que a atribuição se aplica. Somente leitura. Herdado [de unifiedRoleScheduleInstanceBase](../resources/unifiedrolescheduleinstancebase.md).<br> Suporta `$filter` (`eq`).|
|roleEligibilityScheduleId|String|Identificador da roleEligibilitySchedule pai para esta instância.|
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

