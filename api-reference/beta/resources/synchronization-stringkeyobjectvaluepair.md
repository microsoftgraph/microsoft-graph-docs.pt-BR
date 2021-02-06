---
title: Tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Esse é um tipo aberto OData que espera ter uma propriedade chamada `value` que é um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 535e9f104f42771e6f6c182769f0a5e1f68169b6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137062"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>Tipo de recurso stringKeyObjectValuePair

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Esse é um tipo aberto OData que espera ter uma propriedade chamada `value` que é um objeto JSON válido.

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


