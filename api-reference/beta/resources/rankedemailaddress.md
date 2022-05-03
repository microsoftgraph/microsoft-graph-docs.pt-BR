---
title: Tipo de recurso rankedEmailAddress
description: Representa um endereço de email classificado.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: AAmatino
ms.openlocfilehash: 2723009cc44680e98b9c8b5a685c06846bb9abd7
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176311"
---
# <a name="rankedemailaddress-resource-type"></a>Tipo de recurso rankedEmailAddress

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um endereço de email classificado.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|address|cadeia de caracteres|O endereço de email.|
|classificação|double|A classificação do endereço de email. Uma classificação é usada como uma chave de classificação em relação aos outros resultados retornados. Um valor de classificação mais alto corresponde a um resultado mais relevante. A relevância é determinada por sinais de comunicação, colaboração e relacionamento comercial.|

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


