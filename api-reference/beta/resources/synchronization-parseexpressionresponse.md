---
title: tipo de recurso de parseExpressionResponse
description: 'Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832945"
---
# <a name="parseexpressionresponse-resource-type"></a>tipo de recurso de parseExpressionResponse

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a resposta do [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) ação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|erro|OData.Error|Detalhes do erro, se a avaliação da expressão resultou em um erro.|
|evaluationResult|String collection|Uma coleção de valores gerados pela avaliação da expressão.|
|evaluationSucceeded|Booliano|`true`Se a avaliação foi bem-sucedida.|
|parsedExpression|[attributeMappingSource](synchronization-attributemappingsource.md)|Um objeto de [attributeMappingSource](synchronization-attributemappingsource.md) representando a expressão analisada.|
|parsingSucceeded|Booliano|`true`Se a expressão foi analisada com êxito.|

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
