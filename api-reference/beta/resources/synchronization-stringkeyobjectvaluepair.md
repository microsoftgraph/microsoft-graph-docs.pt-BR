---
title: tipo de recurso stringKeyObjectValuePair
description: Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9a04df77ee010368b73abfe5a2d8d78cfe99b0b4
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217560"
---
# <a name="stringkeyobjectvaluepair-resource-type"></a>tipo de recurso stringKeyObjectValuePair

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um par chave-valor onde a chave é uma cadeia de caracteres e o valor é um objeto JSON arbitrário. Este é um tipo de OData aberto que espera ter uma propriedade chamada `value` que seja um objeto JSON válido.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|key|Cadeia de Caracteres|Chave.|
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
