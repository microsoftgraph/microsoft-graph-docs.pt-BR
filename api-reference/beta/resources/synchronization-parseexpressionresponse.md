---
title: Tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação synchronizationSchema: parseExpression.'
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: e564cb2ad7a80c91fec7d6298254fa19bde4537c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133144"
---
# <a name="parseexpressionresponse-resource-type"></a>Tipo de recurso parseExpressionResponse

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta da [ação parseExpression.](../api/synchronization-synchronizationschema-parseexpression.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro|publicError|Detalhes do erro, se a avaliação de expressão tiver resultado em um erro.|
|evaluationResult|Coleção de cadeias de caracteres|Uma coleção de valores produzidos pela avaliação da expressão.|
|evaluationSucceeded|Boolean|`true` se a avaliação foi bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um [objeto attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisado.|
|parsingSucceeded|Boolean|`true` se a expressão foi analisado com êxito.|

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


