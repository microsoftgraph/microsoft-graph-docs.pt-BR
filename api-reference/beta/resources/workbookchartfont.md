---
title: tipo de recurso workbookChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2fcf382f967687b49e114be2b4db1e022eebb0c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979270"
---
# <a name="workbookchartfont-resource-type"></a>tipo de recurso workbookChartFont

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookChartFont](../api/chartfont-get.md) | [workbookChartFont](workbookchartfont.md) |Leia as propriedades e os relacionamentos do objeto chartFont.|
|[Update](../api/chartfont-update.md) | [workbookChartFont](workbookchartfont.md)   |Atualize o objeto ChartFont. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bold|booliano|Representa o status da fonte em negrito.|
|color|cadeia de caracteres|Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.|
|italic|booliano|Representa o status da fonte em itálico.|
|nome|string|Nome da fonte (por exemplo, "Calibri")|
|size|Double|Tamanho da fonte, por exemplo, 11.|
|underline|string|Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None` , `Single` .|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


