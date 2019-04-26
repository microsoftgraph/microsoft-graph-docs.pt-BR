---
title: tipo de recurso privilegedAccess
description: " por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure."
localization_priority: Normal
ms.openlocfilehash: 2dd131dd8f1ba5a2e7668949d2a03a9ab3321d1d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344253"
---
# <a name="privilegedaccess-resource-type"></a>tipo de recurso privilegedAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de funcionalidades fornecidas pelo serviço de gerenciamento de identidade privilegiado (PIM). Instâncias diferentes de `privilegedAccess` representar diferentes provedores gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.


`privilegedAccess`é somente leitura por enquanto. `POST` `DELETE` Nenhuma operação é suportada no conjunto de `privilegedAccess` `PUT` `PATCH`entidades.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A ID do provedor gerenciado pelo PIM.|
|displayName|String     |O nome de exibição do provedor gerenciado pelo PIM.|


## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|recursos       |coleção [entidadegovernanceresource](../resources/governanceresource.md)            |Uma coleção de recursos para o provedor.|
|roleAssignments |coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)|Uma coleção de atribuições de função para o provedor.|
|roleDefinitions |coleção [governanceRoleDefinition](../resources/governanceroledefinition.md)|Uma coleção de defintions de função para o provedor.|
|roleAssignmentRequests |coleção [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Uma coleção de solicitações de atribuição de função para o provedor.|
|roleSettings |coleção [governanceRoleSetting](../resources/governancerolesetting.md)|Uma coleção de configurações de função para o provedor.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
