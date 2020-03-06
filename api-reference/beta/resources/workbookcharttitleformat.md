---
title: tipo de recurso workbookChartTitleFormat
description: Abrange as propriedades de formatação do título do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b7235e8b1d9d5867b47c66a462e9c94b86a528dd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519250"
---
# <a name="workbookcharttitleformat-resource-type"></a>tipo de recurso workbookChartTitleFormat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Abrange as propriedades de formatação do título do gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhuma

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fill|[workbookChartFill](workbookchartfill.md)|Representa o formato de preenchimento de um objeto, que inclui informações sobre a formatação da tela de fundo. Somente leitura.|
|font|[workbookChartFont](workbookchartfont.md)|Representa os atributos de fonte do objeto atual, como nome, tamanho, cor, dentre outros. Somente leitura.|



## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "fill",
    "font"
    ],
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
<!--
{
  "type": "#page.annotation",
  "description": "workbookChartTitleFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
