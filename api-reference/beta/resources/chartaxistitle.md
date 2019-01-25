---
title: Tipo de recurso ChartAxisTitle
description: Representa o título de um eixo do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 25a5daf571f7533bd1682974adecad1cfd984894
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513120"
---
# <a name="chartaxistitle-resource-type"></a>Tipo de recurso ChartAxisTitle

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o título de um eixo do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|Get ChartAxisTitle | [chartAxisTitle](chartaxistitle.md) |Recupere as propriedades e os relacionamentos do objeto chartAxisTitle.|
|[Update](../api/chartaxistitle-update.md) | ChartAxisTitle    |Atualize o objeto ChartAxisTitle. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|texto|string|Representa o título do eixo.|
|visible|booliano|Um booliano que especifica a visibilidade de um título do eixo.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartAxisTitleFormat](chartaxistitleformat.md)|Representa a formatação do título do eixo do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartAxisTitle"
}-->

```json
{
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartAxisTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chartaxistitle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
