---
title: tipo de recurso searchAggregation
description: Fornece os detalhes da agregação de pesquisa na resposta de pesquisa.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 480a6f70a2815a174697ff22fc217057053e1f4b
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193828"
---
# <a name="searchaggregation-resource-type"></a>tipo de recurso searchAggregation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece os detalhes da agregação de pesquisa na resposta de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String| O nome amigável da agregação. Esse valor foi fornecido na entrada.|
|campo|String| Define em qual campo a agregação foi calculada.|
|buckets|coleção [searchBucket](searchbucket.md)| Define os buckets reais da agregação calculada.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchAggregation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "field": "String",  
  "buckets": [{"@odata.type": "microsoft.graph.searchBucket"}]
}
```