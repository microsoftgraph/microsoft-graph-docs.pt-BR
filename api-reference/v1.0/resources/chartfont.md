---
title: Tipo de recurso ChartFont
description: Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.
ms.localizationpriority: medium
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 79e4e65846a51bfc0f0b91cace03d4ee9e8d7ecf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049680"
---
# <a name="chartfont-resource-type"></a>Tipo de recurso ChartFont

Namespace: microsoft.graph

Esse objeto representa os atributos de fonte do objeto Chart, como nome, tamanho, cor, dentre outros.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartFont](../api/chartfont-get.md) | [WorkbookChartFont](chartfont.md) |Leia as propriedades e os relacionamentos do objeto chartFont.|
|[Update](../api/chartfont-update.md) | [WorkbookChartFont](chartfont.md)   |Atualize o objeto ChartFont. |

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

