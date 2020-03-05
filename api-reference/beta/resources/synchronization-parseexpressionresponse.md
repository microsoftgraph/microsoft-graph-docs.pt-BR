---
title: tipo de recurso parseExpressionResponse
description: 'Representa a resposta da ação [synchronizationSchema: ParseName](../api/synchronization_synchronizationschema_parseexpression.md) .'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c752d5c021418dd4a3154a539a61c6ab3bae8a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520132"
---
# <a name="parseexpressionresponse-resource-type"></a>tipo de recurso parseExpressionResponse

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a resposta da ação [parsery](../api/synchronization-synchronizationschema-parseexpression.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro|publicError|Detalhes do erro, se a avaliação da expressão resultar em um erro.|
|evaluationResult|String collection|Uma coleção de valores produzidos pela avaliação da expressão.|
|evaluationSucceeded|Boolean|`true`se a avaliação tiver sido bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um objeto [attributeMappingSource](synchronization-attributemappingsource.md) que representa a expressão analisada.|
|parsingSucceeded|Boolean|`true`se a expressão tiver sido analisada com êxito.|

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
