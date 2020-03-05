---
title: tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bdba5af83357737c77e3b5c441703e404f971587
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521275"
---
# <a name="rankedemailaddress-resource-type"></a>tipo de recurso rankedEmailAddress

Namespace: Microsoft. Graph

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
