---
title: tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 403b97dc335e57dfd2d4f2fe2aa75c4f6fd07682
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319516"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>tipo de recurso accessPackageAssignmentResourceRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma função de recurso de atribuição de pacote do Access indica a função específica do recurso que foi atribuída a um assunto por meio de uma atribuição de pacote do Access.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um objeto accessPackageAssignmentResourceRole. |
| [Listar accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de objetos accessPackageAssignmentResourceRole. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|originid|Cadeia de caracteres|Um identificador exclusivo relativo ao sistema de origem, correspondente à propriedade originid do [accessPackageResourceRole](accesspackageresourcerole.md). |
|originSystem|Cadeia de caracteres|O sistema em que a atribuição de função deve ser criada ou criada para uma atribuição de pacote de acesso, como `SharePointOnline` , `AadGroup` ou `AadApplication` , correspondente à propriedade originSystem do [accessPackageResourceRole](accesspackageresourcerole.md).|
|status|String|O valor é `PendingFulfillment` quando a atribuição de pacote de acesso ainda não foi entregue ao sistema de origem e `Fulfilled` quando a atribuição de pacote de acesso foi entregue ao sistema de origem.|

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
