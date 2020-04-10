---
title: tipo de recurso expressionInputObject
description: Representa um objeto a ser usado como dados de teste de entrada quando a ação synchronizationSchema ParseName executa uma avaliação de expressão.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0756e14f9a35e1ff1b5a63d563d4bca742be566d
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218440"
---
# <a name="expressioninputobject-resource-type"></a>tipo de recurso expressionInputObject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto que será usado como dados de teste de entrada quando a ação [parsetable](../api/synchronization-synchronizationschema-parseexpression.md) executar uma avaliação de expressão.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|definir|[ObjectDefinition](synchronization-objectdefinition.md)|Definição do objeto Test.|
|properties|coleção [stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)|Valores de Propriedade do objeto Test.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
