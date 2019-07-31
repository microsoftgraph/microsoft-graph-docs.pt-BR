---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3ec55eee1f6b5f60e8936f906390d5343fbafbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007827"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>tipo de recurso stringKeyObjectValuePair

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|String|Chave.|
|valor|Json|Objeto JSON arbitrário.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyObjectValuePair"
}-->

```json
{
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "stringKeyObjectValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
