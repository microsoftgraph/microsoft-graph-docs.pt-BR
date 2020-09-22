---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação synchronizationSchema: ParseName.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9bd675b079f42856e85f54b7da84a091a0f57f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988811"
---
# <a name="parseexpressionresponse-resource-type"></a>tipo de recurso parseExpressionResponse

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro|publicError|Detalhes do erro, se a avaliação da expressão resultar em um erro.|
|evaluationResult|Coleção de cadeias de caracteres|Uma coleção de valores produzidos pela avaliação da expressão.|
|evaluationSucceeded|Boolean|`true` se a avaliação tiver sido bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.|
|parsingSucceeded|Boolean|`true` se a expressão tiver sido analisada com êxito.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


