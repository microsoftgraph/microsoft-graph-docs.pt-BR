---
title: Tipo de recurso alteredQueryToken
description: Representa segmentos alterados em relação à consulta de usuário original.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 03e6f010fdcd77e07fc6ce3cc7e8c8c285fde73f
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067834"
---
# <a name="alteredquerytoken-resource-type"></a>Tipo de recurso alteredQueryToken

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa segmentos alterados em relação à consulta de usuário original.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|offset|Int32| Define o deslocamento de um segmento alterado.|
|length|Int32| Define o comprimento de um segmento alterado.|
|suggestion|Cadeia de caracteres| Representa a cadeia de caracteres de segmento corrigido.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alteredQueryToken",
  "baseType": null
}-->

```json
{
  "offset": 0,
  "length": 6,
  "suggestion": "String"
}
```
