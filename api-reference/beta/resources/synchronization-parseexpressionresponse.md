---
title: tipo de recurso de parseExpressionResponse
description: 'Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.'
localization_priority: Normal
ms.openlocfilehash: fc37c963e9c9588241d84570edc73a933eec49fc
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29572875"
---
# <a name="parseexpressionresponse-resource-type"></a>tipo de recurso de parseExpressionResponse

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) ação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro| publicError |Detalhes do erro, se a avaliação da expressão resultou em um erro.|
|evaluationResult|String collection|Uma coleção de valores gerados pela avaliação da expressão.|
|evaluationSucceeded|Boolean|`true`Se a avaliação foi bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um objeto de [attributeMappingSource](synchronization-attributemappingsource.md) representando a expressão analisada.|
|parsingSucceeded|Boolean|`true`Se a expressão foi analisada com êxito.|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
