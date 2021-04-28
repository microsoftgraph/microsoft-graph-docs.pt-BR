---
title: Tipo de recurso de alterationResponse
description: Fornece informações relacionadas a correções ortográficas na resposta à alteração.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e23b94b4e35776b2278c7818efc71f14edcc6cbb
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067883"
---
# <a name="alterationresponse-resource-type"></a>Tipo de recurso de alterationResponse

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações relacionadas a correções ortográficas na resposta à alteração.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|originalQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta do usuário original.|
|queryAlteration|[searchAlteration](searchalteration.md)| Define os detalhes das informações de alteração para a correção ortográfica.|
|queryAlterationType|searchAlterationType| Define o tipo de correção ortográfica. Os valores possíveis `suggestion` são , `modification` .|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alterationResponse",
  "baseType": null
}-->

```json
{
  "originalQueryString": "String",
  "queryAlteration": "String",
  "queryAlterationType": "suggestion"
}
```
