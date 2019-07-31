---
title: tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: e29d5b2f2116050f9cea036df35ed6cc012c0e36
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965520"
---
# <a name="rankedemailaddress-resource-type"></a>tipo de recurso rankedEmailAddress

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um endereço de email classificado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|cadeia de caracteres|O endereço de email.|
|classificação|double|A classificação do endereço de email. Uma classificação é usada como uma chave de classificação, em relação aos outros resultados retornados. Um valor de classificação mais alto corresponde a um resultado mais relevante. A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rankedEmailAddress"
}-->

```json
{
  "address": "string",
  "rank": 1024
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
