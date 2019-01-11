---
title: tipo de recurso de rankedEmailAddress
description: Representa um endereço de email classificados.
localization_priority: Normal
ms.openlocfilehash: bb3b906929bddcb52a57a478647000e7e16fa0be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818512"
---
# <a name="rankedemailaddress-resource-type"></a>tipo de recurso de rankedEmailAddress

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um endereço de email classificados.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|string|O endereço de email.|
|rank|double|A classificação do endereço de email. Uma classificação é usada como uma chave de classificação, em relação as outros resultados retornados. Um valor de classificação mais alto corresponde a um resultado mais relevante. A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.|

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
<!-- {
  "type": "#page.annotation",
  "description": "rankedEmailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
