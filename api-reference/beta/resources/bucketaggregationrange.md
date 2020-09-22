---
title: tipo de recurso bucketAggregationRange
description: 'Permite especificar alguns intervalos manuais na solicitação de agregação. Isso só é aplicável a refinadores não cadeias de caracteres: numéricos e datas.'
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 77f89503a8f19bd8b057575643ebf89e6dbc43a8
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193836"
---
# <a name="bucketaggregationrange-resource-type"></a>tipo de recurso bucketAggregationRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o limite inferior e superior para um intervalo de agregação de resultados de pesquisa. Aplica-se somente a refinadores da data ou tipo numérico.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|from|String| Define o limite inferior a partir do qual a agregação será calculada. Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato. Obrigatório.|
|para|String| Define o limite superior até o qual calcular a agregação. Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bucketAggregationRange",
  "baseType": null
}-->

```json
{
  "from": "String",
  "to": "String"
}
```
