---
title: Tipo de recurso accessPackageAssignmentResourceRole
description: Uma função de recurso de atribuição de pacote de acesso indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 686413addb62dd304d75a25fd475d35f29ffae90
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651523"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>Tipo de recurso accessPackageAssignmentResourceRole

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)uma função de recurso de atribuição de pacote de acesso indica a função específica do recurso que um assunto foi atribuído por meio de uma atribuição de pacote de acesso.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Obter accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Recupere um objeto accessPackageAssignmentResourceRole. |
| [Listar accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md) | [Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Recupere uma lista de objetos accessPackageAssignmentResourceRole. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String| Somente leitura.|
|originId|String|Um identificador exclusivo em relação ao sistema de origem, correspondente à propriedade originId do [accessPackageResourceRole](accesspackageresourcerole.md). |
|originSystem|String|O sistema onde a atribuição de função deve ser criada ou foi criada para uma atribuição de pacote de acesso, como , ou , correspondente à propriedade originSystem do `SharePointOnline` `AadGroup` `AadApplication` [accessPackageResourceRole](accesspackageresourcerole.md).|
|status|String|O valor é quando a atribuição do pacote de acesso ainda não foi entregue ao sistema de origem e quando a atribuição do pacote de acesso foi entregue `PendingFulfillment` `Fulfilled` ao sistema de origem.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageAssignments|[Coleção accessPackageAssignment](accesspackageassignment.md)| As atribuições do pacote de acesso resultantes dessa atribuição de função. Somente leitura. Anulável.|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Somente leitura. Anulável.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Somente leitura. Anulável.|
|accessPackageSubject|[accessPackageSubject](accesspackagesubject.md)| Somente leitura. Anulável. Dá `$filter` suporte a ( ) em `eq` **parâmetros objectId** e `$expand` query.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
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


