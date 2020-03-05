---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c9eddff042af5b2cd724e87e3438f398e8d68c19
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508538"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>tipo de recurso accessPackageAssignmentResourceRole

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de objetos accessPackageAssignmentResourceRole. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|originid|String|Um identificador exclusivo relativo ao sistema de origem. |
|originSystem|String|O sistema em que a atribuição de função deve ser criada para uma atribuição de pacote de acesso.|
|status|String|O valor é `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageAssignments|coleção [accessPackageAssignment](accesspackageassignment.md)| As atribuições de pacote de acesso que resultam nessa atribuição de função. Somente leitura. Anulável.|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|
|accessPackageSubject|[accessPackageSubject](accesspackagesubject.md)| Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
