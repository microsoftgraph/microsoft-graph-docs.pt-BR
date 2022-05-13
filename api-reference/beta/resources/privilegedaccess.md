---
title: Tipo de recurso privilegedAccess
description: " por exemplo, representa `privilegedAccess/azureResources` o PIM gerenciando o acesso privilegiado aos recursos do Azure."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 408f3fe7e6b0b8c05dfbb27599bc5fa7b048d869
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397941"
---
# <a name="privilegedaccess-resource-type"></a>Tipo de recurso privilegedAccess

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um grupo de funcionalidades fornecido pelo serviço Privileged Identity Management (PIM). Diferentes instâncias de representam `privilegedAccess` provedores diferentes gerenciados pelo PIM; por exemplo, `privilegedAccess/azureResources` representa o PIM que gerencia o acesso privilegiado aos recursos do Azure.


`privilegedAccess` é somente leitura por enquanto. Não `POST`, `PUT`, `PATCH`ou operações `DELETE` têm suporte no conjunto `privilegedAccess` de entidades.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     |A ID do provedor gerenciado pelo PIM.|
|displayName|Cadeia de caracteres     |O nome de exibição do provedor gerenciado pelo PIM.|


## <a name="relationships"></a>Relações
| Relação   | Tipo                                         |Descrição|
|:---------------|:---------------------------------------------|:----------|
|recursos       |[Coleção governanceResource](../resources/governanceresource.md)            |Uma coleção de recursos para o provedor.|
|roleAssignments |[coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|Uma coleção de atribuições de função para o provedor.|
|roleDefinitions |[coleção governanceRoleDefinition](../resources/governanceroledefinition.md)|Uma coleção de definições de função para o provedor.|
|roleAssignmentRequests |[coleção governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Uma coleção de solicitações de atribuição de função para o provedor.|
|roleSettings |[coleção governanceRoleSetting](../resources/governancerolesetting.md)|Uma coleção de configurações de função para o provedor.|


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


