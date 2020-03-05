---
title: tipo de recurso stringKeyAttributeMappingSourceValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é attributeMappingSource.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f28b58b5f6bdadf33412a125a841d1c614285557
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520104"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a>tipo de recurso stringKeyAttributeMappingSourceValuePair

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é [attributeMappingSource](synchronization-attributemappingsource.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|String|O nome do parâmetro.|
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
