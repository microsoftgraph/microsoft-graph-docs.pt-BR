---
title: Tipo de recurso keyValuePair
description: Par de valores de chave para parâmetros de ação.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 86a5415c20721f717947238838341345ec9a4250
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366935"
---
# <a name="keyvaluepair-resource-type"></a>Tipo de recurso keyValuePair

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Par de valores de chave para parâmetros de ação.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|name|String|Nome deste par chave-valor|
|valor|Cadeia de caracteres|Valor deste par chave-valor|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyValuePair",
  "baseType": null
}-->

```json
{
  "name": "String",
  "value": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->