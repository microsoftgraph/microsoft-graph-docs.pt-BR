---
title: Tipo de recurso ChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: a24e993bce8688cedd059895ad0dcae8c4d79f55
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59118761"
---
# <a name="charttitleformat-resource-type"></a>Tipo de recurso ChartTitleFormat

Namespace: microsoft.graph

Abrange as propriedades de formatação do título do gráfico.


## <a name="methods"></a>Métodos
Nenhum(a)

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.|
|font|[WorkbookChartFont](chartfont.md)|Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.|



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartTitleFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAreaFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

