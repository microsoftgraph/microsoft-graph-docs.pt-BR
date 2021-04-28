---
title: tipo de recurso searchAlteration
description: Fornece os detalhes da alteração de pesquisa para correção ortográfica.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5caab3a3fbd8f8487e6893c5f5f530cc8471bb80
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067885"
---
# <a name="searchalteration-resource-type"></a>tipo de recurso searchAlteration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes da alteração de pesquisa para correção ortográfica.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|alteredQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta alterada com correção ortográfica.|
|alteredHighlightedQueryString|Cadeia de caracteres| Define a cadeia de caracteres de consulta realçada alterada com correção ortográfica. A anotação em torno do segmento corrigido é (\ue000, \ue001)|
|alteredQueryTokens|[Coleção alteredQueryToken](alteredquerytoken.md)| Representa segmentos alterados em relação à consulta original.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAlteration",
  "baseType": null
}-->

```json
{
  "alteredQueryString": "String",
  "alteredHighlightedQueryString": "String",
  "alteredQueryTokens": [{"@odata.type": "microsoft.graph.alteredQueryToken"}]
}
```