---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523431"
---
# <a name="parseexpressionresponse-resource-type"></a>tipo de recurso parseExpressionResponse

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro|OData. Error|Detalhes do erro, se a avaliação da expressão resultar em um erro.|
|evaluationResult|Coleção de cadeias de caracteres|Uma coleção de valores produzidos pela avaliação da expressão.|
|evaluationSucceeded|Booliano|`true`se a avaliação tiver sido bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.|
|parsingSucceeded|Booliano|`true`se a expressão tiver sido analisada com êxito.|

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
