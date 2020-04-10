---
title: tipo de recurso stringKeyAttributeMappingSourceValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 88dd652e12a8ba7d5d866e2817685e0ad3a732eb
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217574"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>tipo de recurso stringKeyAttributeMappingSourceValuePair

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é [attributeMappingSource](synchronization-attributemappingsource.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|Cadeia de Caracteres|O nome do parâmetro.|
|valor|[attributeMappingSource](synchronization-attributemappingsource.md)|O valor do parâmetro.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
