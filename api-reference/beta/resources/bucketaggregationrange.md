---
title: Tipo de recurso bucketAggregationRange
description: Especifica o limite inferior e superior para um intervalo para agregar resultados de pesquisa. Aplica-se somente a refinadores da data ou tipo numérico
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8a101262dddd859e3c28ef0a32e117dee7546903
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767486"
---
# <a name="bucketaggregationrange-resource-type"></a>Tipo de recurso bucketAggregationRange

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica o limite inferior e superior para um intervalo para agregar resultados de pesquisa. Aplica-se somente a refinadores da data ou tipo numérico.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|from|Cadeia de caracteres| Define o limite inferior do qual calcular a agregação. Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato. Obrigatório.|
|para|Cadeia de caracteres| Define o limite superior para o qual calcular a agregação. Pode ser um valor numérico ou uma representação de cadeia de caracteres de uma data usando o `YYYY-MM-DDTHH:mm:ss.sssZ` formato. Obrigatório.|

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
